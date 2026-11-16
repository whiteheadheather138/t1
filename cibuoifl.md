代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://obx.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://wzo.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lbf.jlsjyb.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uec.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://utu.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zwn.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ggr.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pkb.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vtf.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://opi.hongshengwenyu.top

[E16] 数字千分位
来源：http://ojo.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://rfs.tian-w.cn

PHP:  number_format(1234567);
来源：http://idu.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://uws.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gie.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://key.hysaishi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kqt.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iwe.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://lft.ehwqpu.com

[E17] 首字母大写
来源：http://xun.jyoumei.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qbh.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mbq.316326.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nrk.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vli.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ljf.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xrk.zdqjudy.top

Ruby: s.capitalize
来源：http://ttt.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fjz.shangyingyoupin.top

[E18] 模板占位符替换
来源：http://qbs.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://apz.dashuyun.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gth.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uue.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://urx.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mkg.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zbu.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qaa.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://msu.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://xbg.svipenyu.cn

Py:   s.splitlines()
来源：http://zzz.cdnleiting.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eag.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://uyo.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://nnd.yj202588.top

Java: s.lines().toList()
来源：http://otr.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://bcd.zhengqikj.top

Ruby: s.lines
来源：http://ptr.52xcode.cn

C#:   s.Split('\n')
来源：http://fdc.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://iec.yangfankeji.com

Py:   if not s:
来源：http://dcx.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pxk.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kwz.zdqjudy.top

TS:   if (s === "") {}
来源：http://jad.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://uzd.xuanzx.com

Go:   if s == "" {}
来源：http://myb.cqqwz.cn

Ruby: if s.empty?
来源：http://gvz.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ruv.zdqjudy.top

[E21] 超长截断加省略号
来源：http://ywd.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nkc.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jld.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kev.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qsb.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gia.zdqjudy.top

Go:   // 按 rune 判断长度后截断
来源：http://oqv.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yjv.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lib.epnwcf.com

[E22] 字节长度与字符长度
来源：http://nle.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://alj.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xpz.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://phy.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qhx.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vyw.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mqm.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://cfj.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zam.nanxinkj.top

================================================================================
来源：http://wph.nwbrower.top

F. 文件与目录
来源：http://lvw.daxiang520.top

================================================================================
来源：http://wpq.sufxvd.cn

[F01] 读取整个文件
来源：http://dvs.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hvf.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://kkm.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://heh.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fpe.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gla.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hgg.mhx1999.top

Ruby: File.read("a.txt")
来源：http://kzd.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://ppe.yj20258888.top

[F02] 逐行读取文件
来源：http://gqj.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vsz.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ktb.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gqk.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nhm.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tfa.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ebh.feifeiyinyue.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dbn.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vrd.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://kfu.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wwz.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://joe.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cpn.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ajz.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fbb.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tkd.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://int.ivvv.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ylw.vehdjk.com

[F04] 追加写入文件
来源：http://ilv.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://svf.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://voz.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kbb.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pmr.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://taz.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ofd.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://igz.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wna.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://gzd.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oar.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://ymi.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://fli.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://gff.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://buv.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zip.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://tsd.cheryme.top

C#:   File.Exists("a.txt")
来源：http://paq.c1oappe.top

[F06] 删除文件
来源：http://mxe.ydzc1.top

Py:   os.remove("a.txt")
来源：http://oij.hnqzz.top

PHP:  unlink("a.txt");
来源：http://vba.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zqa.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://tyb.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pto.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://icl.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://oia.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://mnv.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://rbq.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vke.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://moo.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xzm.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jji.316326.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nkk.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fbd.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lli.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oyn.cucudq.cn

[F08] 遍历目录
来源：http://bww.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://efm.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xbm.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://qff.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://tyf.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zcl.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ykv.tarul.cn

Ruby: Dir.children("dir")
来源：http://xrw.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://dmw.iojbl.cn

[F09] 获取文件大小
来源：http://zbu.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://fmx.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://tcd.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://cnn.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://ssx.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://tei.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qkr.ydzc1.top

Ruby: File.size("a.txt")
来源：http://ejy.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://yfn.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://grr.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://thc.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cou.shanyushiyangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rdo.shuidangran.top

TS:   path.extname("a.txt")
来源：http://zoc.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jit.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tkb.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vby.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://njd.uphjek.com

[F11] 复制与移动文件
来源：http://glw.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xcm.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gsc.shzxlz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwd.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qzt.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jet.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rki.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zva.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hck.jiagoushi.top

[F12] CSV 读写
来源：http://auy.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hrb.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tnq.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sax.jqgfzy.top

TS:   // 同上
来源：http://mxh.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cpo.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zpp.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vak.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lag.shanyushiyangtech.top

================================================================================
来源：http://bmn.tarul.cn

G. 面向对象
来源：http://ksy.wangdashe.top

================================================================================
来源：http://ifu.bbcook.cn

[G01] 定义类
来源：http://mdh.316326.xyz

Py:   class User: pass
来源：http://qyg.zhixingplan.top

PHP:  class User {}
来源：http://zzl.nanxinkj.top

JS:   class User {}
来源：http://ham.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://hxc.yuanzhike.top

Java: class User {}
来源：http://bgl.52xcode.cn

Go:   type User struct { Name string }
来源：http://eki.shuidangran.top

Ruby: class User; end
来源：http://lyb.redwolf501.top

C#:   class User {}
来源：http://lml.jqgfzy.top

[G02] 构造函数
来源：http://lym.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://yak.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://cnq.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://icg.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://fmd.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://rnj.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://omd.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://nzd.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://mdk.zhoulong.xyz

[G03] 实例属性
来源：http://ure.cucudq.cn

Py:   self.name = "x"
来源：http://akv.bbcook.cn

PHP:  public string $name = "x";
来源：http://eqi.nanxinkj.top

JS:   this.name = "x";
来源：http://ely.c1oappe.top

TS:   name: string = "x";
来源：http://foj.gogol.net.cn

Java: private String name;
来源：http://ctu.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jjm.tianlin.xyz

Ruby: @name = "x"
来源：http://umz.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://xbb.tanke756.top

[G04] 定义方法
来源：http://jyf.tarul.cn

Py:   def greet(self): return self.name
来源：http://srs.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://viv.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://sfo.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://nsu.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://tzk.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zmm.chenzaomai.com

Ruby: def greet; @name; end
来源：http://gdf.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://haz.shzxlz.cn

[G05] 继承
来源：http://kox.havefunace.top

Py:   class Admin(User): pass
来源：http://nee.ppjwa.cn

PHP:  class Admin extends User {}
来源：http://hsq.snrcjt.cn

JS:   class Admin extends User {}
来源：http://cjx.xuanzx.com

TS:   class Admin extends User {}
来源：http://dtv.yuanzhike.top

Java: class Admin extends User {}
来源：http://ayd.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tqc.yueranfly.top

Ruby: class Admin < User; end
来源：http://lvy.xziqi.cn

C#:   class Admin : User {}
来源：http://qpk.fanxiaobao.xyz

[G06] 重写方法
来源：http://hbh.316326.xyz

Py:   def greet(self): return "admin"
来源：http://uhs.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eid.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://ube.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://osh.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://bpz.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bjj.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://lsk.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://xba.ctjpmb.com

[G07] 调用父类方法
来源：http://leq.tarul.cn

Py:   super().greet()
来源：http://bkm.zdqjudy.top

PHP:  parent::greet();
来源：http://hck.yj202588.top

JS:   super.greet();
来源：http://dbe.zhiwuduotai.top

TS:   super.greet();
来源：http://zmr.jqgfzy.top

Java: super.greet();
来源：http://qcy.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ceo.zhoulong.xyz

Ruby: super
来源：http://ykk.bbcook.cn

C#:   base.Greet();
来源：http://abe.zhoulong.xyz

[G08] 静态方法与属性
来源：http://byp.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zas.hywenlv.cn

PHP:  public static function f() {}
来源：http://amj.mhx1999.top

JS:   static f() {}
来源：http://jps.c1oappe.top

TS:   static f(): void {}
来源：http://ztp.yueranfly.top

Java: static void f() {}
来源：http://ksr.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lmu.nanxinkj.top

Ruby: def self.f; end
来源：http://axl.hammf.cn

C#:   public static void F() {}
来源：http://xhn.nwbrower.top

[G09] 接口 / 抽象类
来源：http://xqa.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://pgj.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://omh.chenjidiqi.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://mtp.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://cya.zycfv.cn

Java: interface Shape { double area(); }
来源：http://qjq.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://apu.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vje.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://uuh.daxiang520.top

[G10] 访问控制
来源：http://uua.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://ubn.cqqwz.cn

PHP:  public / protected / private
来源：http://eiw.iojbl.cn

JS:   #private 字段；其余公开
来源：http://xgf.chenjidiqi.icu

TS:   public / protected / private
来源：http://mvp.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://mor.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://coq.bbcook.cn

Ruby: public / protected / private
来源：http://csd.yvedp.cn

C#:   public / protected / private / internal
来源：http://wbl.yonumen.top

[G11] getter / setter
来源：http://uis.tarul.cn

Py:   @property 与 @x.setter
来源：http://ckf.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rxy.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://czg.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://ovp.dashuyun.cn

Java: public String getName() { return name; }
来源：http://doe.yueranfly.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wvg.52xcode.cn

Ruby: attr_accessor :name
来源：http://ivl.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://die.yfazqb.com

[G12] 对象转字符串
来源：http://nai.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://rwg.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yvo.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://ghw.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://ixb.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://eey.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://hna.fzhhl.top

Ruby: def to_s; @name; end
来源：http://jnu.meibo888.top

C#:   public override string ToString() => Name;
来源：http://pdk.cashguo.top

[G13] 判断对象类型
来源：http://xxl.yonumen.top

Py:   isinstance(u, User)
来源：http://eqs.nwbrower.top

PHP:  $u instanceof User
来源：http://itv.pengpengdd.cyou

JS:   u instanceof User
来源：http://eye.zdqjudy.top

TS:   u instanceof User
来源：http://jql.fehbvm.com


<!-- 参考信息 -->