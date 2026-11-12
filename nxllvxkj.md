代发 wailian999

[E14] URL 编码与 Base64
来源：http://asv.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://keb.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fun.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uns.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://liy.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://niz.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ong.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dqd.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gbc.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://hjg.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bjd.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iwk.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ifn.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uiq.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vti.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://krk.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eub.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aga.ybcxt.top

[E16] 数字千分位
来源：http://csy.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://iut.birdmap.top

PHP:  number_format(1234567);
来源：http://pgh.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uic.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://byz.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xpw.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xyo.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zva.fanxiaobao.xyz

C#:   1234567.ToString("N0")
来源：http://qxo.zdqjudy.top

[E17] 首字母大写
来源：http://onf.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vjv.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kdq.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqy.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://src.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mew.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jkz.uphjek.com

Ruby: s.capitalize
来源：http://wxx.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ysr.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://qjd.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oby.xziqi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jda.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tuk.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://tob.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://int.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kwu.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fsg.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://apz.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://dou.zhongyouzk.top

Py:   s.splitlines()
来源：http://dsk.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fyz.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://dhg.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://qbc.pengpengdd.cyou

Java: s.lines().toList()
来源：http://sir.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://hyc.xuetiantiany.cn

Ruby: s.lines
来源：http://bmq.daria6918.cn

C#:   s.Split('\n')
来源：http://kux.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://kux.tarul.cn

Py:   if not s:
来源：http://vao.feifeiyinyue.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://chy.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://odh.dashuyun.cn

TS:   if (s === "") {}
来源：http://bqa.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://ngr.svipenyu.cn

Go:   if s == "" {}
来源：http://flo.guannengcc.top

Ruby: if s.empty?
来源：http://row.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ngf.guowangkeji.top

[E21] 超长截断加省略号
来源：http://lts.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eji.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ckt.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dkf.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ghm.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cix.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://zah.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hhr.chenlongwang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cxw.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://xng.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uqc.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sty.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wnk.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://diy.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lfs.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rtq.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://srd.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vwq.cashguo.top

================================================================================
来源：http://wpj.nanxuanxn.top

F. 文件与目录
来源：http://gvz.jinqigfzy.top

================================================================================
来源：http://bzm.nanxuanxn.top

[F01] 读取整个文件
来源：http://rbl.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://emr.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://kda.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://upm.sjlbkw.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://atj.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://agu.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://whk.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://yrd.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://hkb.ydzc1.top

[F02] 逐行读取文件
来源：http://tfe.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xzg.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nsw.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzc.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qvx.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cou.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://svj.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jqc.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wcw.daxiang520.top

[F03] 写入文件（覆盖）
来源：http://olv.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tdx.ivvv.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kxv.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xcm.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dhw.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lfo.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://maz.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://uhb.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ais.quarkkingdee.top

[F04] 追加写入文件
来源：http://elx.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ude.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://thp.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://obc.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bpk.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ikn.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rnl.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ifl.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lja.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://khc.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vle.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://tvq.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://nvg.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://jbb.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://miq.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iac.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://ojc.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://eza.ivvv.top

[F06] 删除文件
来源：http://ppc.guannengcc.top

Py:   os.remove("a.txt")
来源：http://bia.smart0.xyz

PHP:  unlink("a.txt");
来源：http://yrc.epnwcf.com

JS:   fs.unlinkSync("a.txt")
来源：http://cbw.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://aod.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lrl.yj202588.top

Go:   os.Remove("a.txt")
来源：http://qza.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://spk.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://whe.xuanzx.com

[F07] 创建目录（含多级）
来源：http://viq.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fde.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ktz.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ejn.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cpr.iojbl.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dtg.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://awa.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bji.xuanzx.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vam.sysykeji.top

[F08] 遍历目录
来源：http://fdv.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qce.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bci.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://obg.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://jrg.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ngg.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nzj.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://nco.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://frc.ehwqpu.com

[F09] 获取文件大小
来源：http://jjb.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://ckk.sysykeji.top

PHP:  filesize("a.txt");
来源：http://dky.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://drm.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://hjl.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://ftc.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tws.hesvh.cn

Ruby: File.size("a.txt")
来源：http://cqr.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://dnu.ywan-chungtsiang.top

[F10] 取文件扩展名 / 文件名
来源：http://aot.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://adz.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vcb.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wbo.yonumen.top

TS:   path.extname("a.txt")
来源：http://uii.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bcw.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tch.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iws.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ddu.gotoacloud.top

[F11] 复制与移动文件
来源：http://isi.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kps.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wcn.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rjk.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqz.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxy.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kem.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ahu.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://luu.zhongyouzk.top

[F12] CSV 读写
来源：http://wyg.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yhk.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ell.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uop.tanke756.top

TS:   // 同上
来源：http://nvl.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ykw.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zkq.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kfv.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gel.daria6918.cn

================================================================================
来源：http://xwu.sufxvd.cn

G. 面向对象
来源：http://jow.pycfn.com

================================================================================
来源：http://eua.9152youxi.cn

[G01] 定义类
来源：http://tkd.sjlbkw.cn

Py:   class User: pass
来源：http://lzn.fehbvm.com

PHP:  class User {}
来源：http://mgx.yfazqb.com

JS:   class User {}
来源：http://ylm.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://wlj.tianlin.xyz

Java: class User {}
来源：http://yhz.redwolf501.top

Go:   type User struct { Name string }
来源：http://okx.quarkkingdee.top

Ruby: class User; end
来源：http://eet.pengpengdd.cyou

C#:   class User {}
来源：http://ipv.yangfankeji.com

[G02] 构造函数
来源：http://onr.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://fje.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://oka.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://zkw.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://dlc.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://nvw.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aec.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://jdo.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://jot.hesvh.cn

[G03] 实例属性
来源：http://ama.hammf.cn

Py:   self.name = "x"
来源：http://jfs.daria6918.cn

PHP:  public string $name = "x";
来源：http://nkj.bjfxy.top

JS:   this.name = "x";
来源：http://hdx.dianchejie.cn

TS:   name: string = "x";
来源：http://sns.ehwqpu.com

Java: private String name;
来源：http://wuh.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xan.yfazqb.com

Ruby: @name = "x"
来源：http://elk.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://hmv.vehdjk.com

[G04] 定义方法
来源：http://vyr.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://qgj.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tur.tian-w.cn

JS:   greet() { return this.name; }
来源：http://non.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://fxs.hesvh.cn

Java: String greet() { return name; }
来源：http://ekn.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ppe.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://tfn.bbcook.cn

C#:   public string Greet() => Name;
来源：http://zuc.zhongyouzk.top

[G05] 继承
来源：http://azr.dashuyun.cn

Py:   class Admin(User): pass
来源：http://pyo.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://nxn.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://zke.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://hgb.fzhhl.top

Java: class Admin extends User {}
来源：http://gcw.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gvj.mhx1999.top

Ruby: class Admin < User; end
来源：http://xul.aibaodan.cn

C#:   class Admin : User {}
来源：http://kfs.nanxinkj.top

[G06] 重写方法
来源：http://pvk.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://wee.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://nui.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://gis.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://bgk.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://ncn.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://etn.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://trh.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://azm.redwolf501.top

[G07] 调用父类方法
来源：http://yqi.sjlbkw.cn

Py:   super().greet()
来源：http://wkb.hongshengwenyu.top

PHP:  parent::greet();
来源：http://reu.yonumen.top

JS:   super.greet();
来源：http://jdq.zhongyouzk.top

TS:   super.greet();
来源：http://tge.quarkkingdee.top

Java: super.greet();
来源：http://zmx.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yqe.smart0.xyz

Ruby: super
来源：http://drm.hfpthk.cn

C#:   base.Greet();
来源：http://oqz.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://trc.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sbx.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://tsc.cqqwz.cn

JS:   static f() {}
来源：http://awc.yonumen.top

TS:   static f(): void {}
来源：http://nhu.sxryk.cn

Java: static void f() {}
来源：http://eqq.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oqq.cashguo.top

Ruby: def self.f; end
来源：http://ffp.fzhhl.top

C#:   public static void F() {}
来源：http://tku.birdmap.top

[G09] 接口 / 抽象类
来源：http://wjm.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://xjt.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://oka.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xoq.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://lxw.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://yso.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://ggk.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kkl.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://fjk.zycfv.cn

[G10] 访问控制
来源：http://zdf.havefunace.top

Py:   约定 _protected / __private（不强制）
来源：http://seu.uphjek.com

PHP:  public / protected / private
来源：http://fye.ydzc1.top

JS:   #private 字段；其余公开
来源：http://wdl.sxryk.cn

TS:   public / protected / private
来源：http://rew.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://def.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wqd.epnwcf.com

Ruby: public / protected / private
来源：http://cpu.zdbjq.cn

C#:   public / protected / private / internal
来源：http://fyw.zhixingplan.top

[G11] getter / setter
来源：http://eiu.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://cro.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://idz.gotoacloud.top

JS:   get name() { return this._name; }
来源：http://wmw.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://znc.cashguo.top

Java: public String getName() { return name; }
来源：http://kau.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://kne.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://qux.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://rcx.bbcook.cn

[G12] 对象转字符串
来源：http://avv.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://mjf.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lod.fzhhl.top

JS:   toString() { return this.name; }
来源：http://igr.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://qmk.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://amq.xylfe.cn


<!-- 参考信息 -->