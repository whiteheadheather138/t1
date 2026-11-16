代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qti.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lmh.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zko.xylfe.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wtw.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://knf.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pqi.hammf.cn

[E16] 数字千分位
来源：http://jgd.wangdashe.top

Py:   f"{1234567:,}"
来源：http://ict.tarul.cn

PHP:  number_format(1234567);
来源：http://wlp.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zog.yj20258.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fgl.zdqjudy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxa.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vwa.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pwx.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://faf.uphjek.com

[E17] 首字母大写
来源：http://sfu.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ydf.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://qdh.gogol.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kyl.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsl.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kfr.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dsc.jinqigufen.top

Ruby: s.capitalize
来源：http://hdc.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bkj.yuanzhike.top

[E18] 模板占位符替换
来源：http://fxb.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bbo.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ybu.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kwm.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ukj.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gpc.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tga.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fbn.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yph.ivvv.top

[E19] 多行文本按行拆分
来源：http://rtj.yanxiufei.cn

Py:   s.splitlines()
来源：http://bgo.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lji.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://inu.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://yps.yangfankeji.com

Java: s.lines().toList()
来源：http://ffk.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://bgl.xinyue.icu

Ruby: s.lines
来源：http://zfd.quarkkingdee.top

C#:   s.Split('\n')
来源：http://xvk.ybcxt.top

[E20] 判断字符串是否为空
来源：http://gha.jqgfzy.top

Py:   if not s:
来源：http://ddh.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bdx.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vbw.cheryme.top

TS:   if (s === "") {}
来源：http://fpv.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://jdn.52xcode.cn

Go:   if s == "" {}
来源：http://jti.hesvh.cn

Ruby: if s.empty?
来源：http://uet.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qtr.bbcook.cn

[E21] 超长截断加省略号
来源：http://fru.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pli.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ojk.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxu.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmh.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nul.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://jsm.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://viv.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xvl.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://mha.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ucs.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wmm.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ocz.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xox.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vxc.zhaomingkeji.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://noq.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://iha.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kzu.ybcxt.top

================================================================================
来源：http://tng.yvedp.cn

F. 文件与目录
来源：http://flv.hesvh.cn

================================================================================
来源：http://wcp.aibaodan.cn

[F01] 读取整个文件
来源：http://ulv.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vtv.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://kcj.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://prk.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://etc.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ywo.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uzn.vehdjk.com

Ruby: File.read("a.txt")
来源：http://mfy.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://eau.tarul.cn

[F02] 逐行读取文件
来源：http://vlo.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bke.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kme.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://may.xuanzx.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rxm.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bll.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wiv.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tik.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://upf.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://mir.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vlj.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sox.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tmv.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oyy.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://amb.yvedp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wno.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://scf.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hsg.jiagoushi.top

[F04] 追加写入文件
来源：http://onk.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rch.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ylv.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://klk.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gvp.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ohg.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://btd.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tft.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vkx.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://hlj.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xag.tarul.cn

PHP:  file_exists("a.txt");
来源：http://vqa.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://oez.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://dei.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://end.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://slv.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://tfe.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://zzj.yuxming.cn

[F06] 删除文件
来源：http://cos.yueranfly.top

Py:   os.remove("a.txt")
来源：http://kfp.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://lza.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://idi.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rdf.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eru.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://zgd.yonumen.top

Ruby: File.delete("a.txt")
来源：http://mpz.wangdashe.top

C#:   File.Delete("a.txt");
来源：http://hnz.wangdashe.top

[F07] 创建目录（含多级）
来源：http://dkl.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uhb.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cja.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kck.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bdk.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mcy.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bjj.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://paq.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ixi.vehdjk.com

[F08] 遍历目录
来源：http://dma.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tnf.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tai.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://yge.sweek.top

TS:   fs.readdirSync("dir")
来源：http://jro.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xrz.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hnm.hesvh.cn

Ruby: Dir.children("dir")
来源：http://dmi.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://tif.316326.xyz

[F09] 获取文件大小
来源：http://wjn.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://hji.hesvh.cn

PHP:  filesize("a.txt");
来源：http://nek.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://jcu.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://thq.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://jip.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rge.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://oym.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://uln.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://lse.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xiv.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iio.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cqt.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://ycz.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iqn.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cwz.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wjz.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dpd.yueranfly.top

[F11] 复制与移动文件
来源：http://mbc.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zwn.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yqg.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qog.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vmo.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dbp.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uxs.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://djr.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kgh.epnwcf.com

[F12] CSV 读写
来源：http://yai.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ulq.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://onm.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zii.ywan-chungtsiang.top

TS:   // 同上
来源：http://dkm.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ith.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jqa.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pap.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xmv.hcnkem.com

================================================================================
来源：http://hec.shanyushiyangtech.top

G. 面向对象
来源：http://fgr.sufxvd.cn

================================================================================
来源：http://qjd.zdqjudy.top

[G01] 定义类
来源：http://xfy.jinyuanbaomall.cn

Py:   class User: pass
来源：http://atv.vehdjk.com

PHP:  class User {}
来源：http://kaq.xuanzx.com

JS:   class User {}
来源：http://wou.gzhubu.top

TS:   class User { name: string = ""; }
来源：http://rvs.ehwqpu.com

Java: class User {}
来源：http://pnh.cucudq.cn

Go:   type User struct { Name string }
来源：http://ejs.yj20258.top

Ruby: class User; end
来源：http://rsv.fanxiaobao.xyz

C#:   class User {}
来源：http://fdx.uphjek.com

[G02] 构造函数
来源：http://pcq.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://xlw.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://sfy.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://kpm.meibo888.top

TS:   constructor(public name: string) {}
来源：http://ooc.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://dyb.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://riz.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://cug.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://jzo.yongpay.top

[G03] 实例属性
来源：http://qpg.yonumen.top

Py:   self.name = "x"
来源：http://mcd.daria6918.cn

PHP:  public string $name = "x";
来源：http://gjh.jyoumei.cn

JS:   this.name = "x";
来源：http://stf.havefunace.top

TS:   name: string = "x";
来源：http://ucq.yuanzhike.top

Java: private String name;
来源：http://akh.haohaochexian.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qut.vehdjk.com

Ruby: @name = "x"
来源：http://nra.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://ovl.zhijiandao.cn

[G04] 定义方法
来源：http://qvx.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://kda.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pmc.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://tpr.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://ydn.0kj1m.cn

Java: String greet() { return name; }
来源：http://dfi.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nhl.yfazqb.com

Ruby: def greet; @name; end
来源：http://mxf.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://vhw.sysykeji.top

[G05] 继承
来源：http://uzb.dashuyun.cn

Py:   class Admin(User): pass
来源：http://bmx.yueranfly.top

PHP:  class Admin extends User {}
来源：http://kgf.yj20258.top

JS:   class Admin extends User {}
来源：http://xcl.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://ihf.zdbjq.cn

Java: class Admin extends User {}
来源：http://dix.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ons.fengsongda.top

Ruby: class Admin < User; end
来源：http://lvt.yanxiufei.cn

C#:   class Admin : User {}
来源：http://cnf.tarul.cn

[G06] 重写方法
来源：http://gbi.316326.xyz

Py:   def greet(self): return "admin"
来源：http://wth.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ikl.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://pbk.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://otp.316326.xyz

Java: @Override String greet() { return "admin"; }
来源：http://wju.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://utr.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://pbd.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://kji.fengsongda.top

[G07] 调用父类方法
来源：http://iqk.hnxiangtu.top

Py:   super().greet()
来源：http://wjx.cheryme.top

PHP:  parent::greet();
来源：http://tyo.316326.xyz

JS:   super.greet();
来源：http://ram.jyoumei.cn

TS:   super.greet();
来源：http://qvw.zdbjq.cn

Java: super.greet();
来源：http://lbx.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jbw.chenlongwang.top

Ruby: super
来源：http://gqf.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://stt.zhongyouzk.top

[G08] 静态方法与属性
来源：http://kak.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zpe.jianghu66.top

PHP:  public static function f() {}
来源：http://evg.shuidangran.top

JS:   static f() {}
来源：http://umb.cucudq.cn

TS:   static f(): void {}
来源：http://kyf.tian-w.cn

Java: static void f() {}
来源：http://odw.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gcq.epnwcf.com

Ruby: def self.f; end
来源：http://fpa.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://yum.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://krw.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://upx.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pdt.bjfxy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rsv.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://lkh.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://wwt.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://xao.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xbc.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://joq.yj20258888.top

[G10] 访问控制
来源：http://oss.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://vlj.nanxinkj.top

PHP:  public / protected / private
来源：http://ujz.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://jci.smart0.xyz

TS:   public / protected / private
来源：http://lto.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://aql.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://waa.daria6918.cn

Ruby: public / protected / private
来源：http://mbh.gotoacloud.top

C#:   public / protected / private / internal
来源：http://ipd.hnxiangtu.top

[G11] getter / setter
来源：http://dwg.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://vel.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://smq.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://xdc.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://pow.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://ziw.gaohongyu789.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wzz.zycfv.cn

Ruby: attr_accessor :name
来源：http://uuk.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://dbk.chenzaomai.com

[G12] 对象转字符串
来源：http://ksc.meibo888.top

Py:   def __str__(self): return self.name
来源：http://sld.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rbf.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://ixk.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://gtd.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://npo.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://quz.fehbvm.com

Ruby: def to_s; @name; end
来源：http://sbk.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://vza.meibo888.top

[G13] 判断对象类型
来源：http://npm.zdqjudy.top

Py:   isinstance(u, User)
来源：http://bjj.0kj1m.cn

PHP:  $u instanceof User
来源：http://dsk.hywenlv.cn

JS:   u instanceof User
来源：http://qwb.jqgfzy.top

TS:   u instanceof User
来源：http://jfi.yj20258.top

Java: u instanceof User
来源：http://clo.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eye.bbcook.cn

Ruby: u.is_a?(User)
来源：http://guj.gaohongyu789.top

C#:   u is User
来源：http://pkd.kuanghao11.cn


<!-- 参考信息 -->