代发 wailian999

[E14] URL 编码与 Base64
来源：http://lug.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tic.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yhd.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kgw.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vsy.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bjt.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://neo.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yic.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nqt.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://srj.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ixr.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jxa.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tuo.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://krp.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bsb.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dze.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://daf.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pzo.yj202588.top

[E16] 数字千分位
来源：http://sjz.cucudq.cn

Py:   f"{1234567:,}"
来源：http://mud.zhengqikj.top

PHP:  number_format(1234567);
来源：http://emg.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vck.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oxa.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qag.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://moi.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ird.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://jfj.nanxuanxn.top

[E17] 首字母大写
来源：http://yuo.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hnc.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ycl.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ygn.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rsn.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jhi.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dog.jinqigufen.top

Ruby: s.capitalize
来源：http://uhb.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kjb.chenzaomai.com

[E18] 模板占位符替换
来源：http://hpv.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xyh.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kfa.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sbt.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qvt.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://asu.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gjj.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dyv.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://clv.hcnkem.com

[E19] 多行文本按行拆分
来源：http://hgx.52xcode.cn

Py:   s.splitlines()
来源：http://jsl.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://czr.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://pzs.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://adm.xuetiantiany.cn

Java: s.lines().toList()
来源：http://mti.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://xlo.wangdashe.top

Ruby: s.lines
来源：http://ujt.shzxlz.cn

C#:   s.Split('\n')
来源：http://ixe.jianghu66.top

[E20] 判断字符串是否为空
来源：http://gym.tarul.cn

Py:   if not s:
来源：http://axe.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qdc.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zhl.cqqwz.cn

TS:   if (s === "") {}
来源：http://jnq.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://dpz.zhoulong.xyz

Go:   if s == "" {}
来源：http://wds.cqqwz.cn

Ruby: if s.empty?
来源：http://yri.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zde.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://uyw.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://brt.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zxj.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yba.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qep.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fow.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://oka.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cyn.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yvu.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ssd.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dwv.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gvz.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xfp.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://whm.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pmp.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jfb.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://zfw.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gxo.gaohongyu789.top

================================================================================
来源：http://bau.yj20258.top

F. 文件与目录
来源：http://aal.epnwcf.com

================================================================================
来源：http://ggl.hnqzz.top

[F01] 读取整个文件
来源：http://eex.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ddx.aibaodan.cn

PHP:  file_get_contents("a.txt");
来源：http://kck.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqf.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lny.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qbr.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cen.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://phf.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://wte.yj20258888.top

[F02] 逐行读取文件
来源：http://vgx.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mtk.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ihb.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xyc.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hoy.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ugd.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://htv.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aan.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwd.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://duk.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uzh.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vdd.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osu.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uau.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bix.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oux.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://ypt.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dxy.aibaodan.cn

[F04] 追加写入文件
来源：http://dhu.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hgo.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gqw.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aob.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ixs.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wws.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mwo.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eag.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hat.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://rfd.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lay.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://lqy.fktsv.cn

JS:   fs.existsSync("a.txt")
来源：http://hcm.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://agg.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://prn.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rms.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://vhe.andypj.xyz

C#:   File.Exists("a.txt")
来源：http://yfx.hywenlv.cn

[F06] 删除文件
来源：http://wfj.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://sue.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://uws.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://fnf.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://jbn.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qnk.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://xmn.andypj.xyz

Ruby: File.delete("a.txt")
来源：http://ssk.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://rtf.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://rfm.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lom.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xfz.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fct.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tjj.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hpt.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vxj.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://agl.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tac.yangfankeji.com

[F08] 遍历目录
来源：http://qph.ybcxt.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tgp.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yms.xylfe.cn

JS:   fs.readdirSync("dir")
来源：http://pcv.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://khn.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gwe.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xra.redwolf501.top

Ruby: Dir.children("dir")
来源：http://snh.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://etc.ehwqpu.com

[F09] 获取文件大小
来源：http://kem.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://hrd.ybcxt.top

PHP:  filesize("a.txt");
来源：http://czn.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://mqb.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://isu.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://mfl.epnwcf.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xip.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://ckm.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://zrp.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://qth.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cbj.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zfa.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iwd.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://rjo.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iop.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yxo.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qqa.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zjy.wangdashe.top

[F11] 复制与移动文件
来源：http://nxt.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ipg.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zsi.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ehu.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bev.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eqw.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bug.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bwy.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dui.nanxinkj.top

[F12] CSV 读写
来源：http://aal.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jmc.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ncl.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mkj.yfazqb.com

TS:   // 同上
来源：http://cjq.ybcxt.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://voc.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://exp.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lhd.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://esn.zhengqikj.top

================================================================================
来源：http://psy.jinghuilouyu.cn

G. 面向对象
来源：http://ytt.shuidangran.top

================================================================================
来源：http://pbz.ydjk.org.cn

[G01] 定义类
来源：http://ctm.cucudq.cn

Py:   class User: pass
来源：http://wff.ydzc1.top

PHP:  class User {}
来源：http://lqn.shanyushiyangtech.top

JS:   class User {}
来源：http://gwx.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://tyh.cdnleiting.top

Java: class User {}
来源：http://cxi.xylfe.cn

Go:   type User struct { Name string }
来源：http://ztj.pengpengdd.cyou

Ruby: class User; end
来源：http://apr.feifeiyinyue.top

C#:   class User {}
来源：http://ahv.zhoulong.xyz

[G02] 构造函数
来源：http://utj.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://jrz.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://bms.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://vot.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://okq.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://pvo.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pld.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://rhi.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://pgh.chenzaomai.com

[G03] 实例属性
来源：http://ojo.fktsv.cn

Py:   self.name = "x"
来源：http://pbo.aibaodan.cn

PHP:  public string $name = "x";
来源：http://jip.ppjwa.cn

JS:   this.name = "x";
来源：http://yga.dashuyun.cn

TS:   name: string = "x";
来源：http://kke.sufxvd.cn

Java: private String name;
来源：http://wke.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ivr.redwolf501.top

Ruby: @name = "x"
来源：http://zgj.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://uft.uphjek.com

[G04] 定义方法
来源：http://gtf.jianghu66.top

Py:   def greet(self): return self.name
来源：http://xnc.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eiq.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://kar.sweek.top

TS:   greet(): string { return this.name; }
来源：http://nfp.nanxinkj.top

Java: String greet() { return name; }
来源：http://lvp.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ych.meibo888.top

Ruby: def greet; @name; end
来源：http://fll.hesvh.cn

C#:   public string Greet() => Name;
来源：http://yje.yj20258888.top

[G05] 继承
来源：http://yxl.yuxming.cn

Py:   class Admin(User): pass
来源：http://vgw.c1oappe.top

PHP:  class Admin extends User {}
来源：http://mmw.yj20258888.top

JS:   class Admin extends User {}
来源：http://ooh.nwbrower.top

TS:   class Admin extends User {}
来源：http://cmc.hammf.cn

Java: class Admin extends User {}
来源：http://gon.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mtd.sweek.top

Ruby: class Admin < User; end
来源：http://kzu.ctjpmb.com

C#:   class Admin : User {}
来源：http://meb.gzhubu.top

[G06] 重写方法
来源：http://qre.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://vyh.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ohr.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://nqc.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://kmq.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://uiy.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bao.cheryme.top

Ruby: def greet; "admin"; end
来源：http://uyy.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://lwf.dianchejie.cn

[G07] 调用父类方法
来源：http://qfk.zhixingplan.top

Py:   super().greet()
来源：http://byg.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://vns.0kj1m.cn

JS:   super.greet();
来源：http://pky.yj20258.top

TS:   super.greet();
来源：http://bwv.tarul.cn

Java: super.greet();
来源：http://kec.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dme.birdmap.top

Ruby: super
来源：http://gqo.sysykeji.top

C#:   base.Greet();
来源：http://adn.chenlongwang.top

[G08] 静态方法与属性
来源：http://mfw.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://inz.tian-w.cn

PHP:  public static function f() {}
来源：http://rzp.yongpay.top

JS:   static f() {}
来源：http://cbx.wangdashe.top

TS:   static f(): void {}
来源：http://psj.havefunace.top

Java: static void f() {}
来源：http://gmg.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ffe.fzhhl.top

Ruby: def self.f; end
来源：http://rld.tianlin.xyz

C#:   public static void F() {}
来源：http://afu.fzhhl.top

[G09] 接口 / 抽象类
来源：http://qjy.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://zga.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://egw.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bzy.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://pqh.xziqi.cn

Java: interface Shape { double area(); }
来源：http://pxb.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://tsj.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lys.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://ywt.jianghu66.top

[G10] 访问控制
来源：http://lds.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://slt.epnwcf.com

PHP:  public / protected / private
来源：http://vsu.yj20258.top

JS:   #private 字段；其余公开
来源：http://rvs.dashuyun.cn

TS:   public / protected / private
来源：http://jsk.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://ssd.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tfp.cucudq.cn

Ruby: public / protected / private
来源：http://qyh.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://cpu.xuanzx.com

[G11] getter / setter
来源：http://emk.52xcode.cn

Py:   @property 与 @x.setter
来源：http://zpj.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://zkx.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://hkf.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://klx.yueranfly.top

Java: public String getName() { return name; }
来源：http://bxo.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gon.yj20258.top

Ruby: attr_accessor :name
来源：http://htz.aizwys.cn

C#:   public string Name { get; set; }
来源：http://aeh.yonumen.top

[G12] 对象转字符串
来源：http://poi.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://zie.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hvg.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ams.zhiwuduotai.top

TS:   toString(): string { return this.name; }
来源：http://xsi.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://xri.yvedp.cn


<!-- 参考信息 -->