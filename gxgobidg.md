代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://duv.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bqf.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://eah.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cxf.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://qzg.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qaf.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qgc.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wck.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bzy.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mbj.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rgj.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eby.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://stj.tanke756.top

[E15] HTML 转义 / 反转义
来源：http://fuu.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eug.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://usg.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fxh.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mwg.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lru.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dna.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mms.sweek.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nvr.cashguo.top

[E16] 数字千分位
来源：http://lmj.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://apk.cdnleiting.top

PHP:  number_format(1234567);
来源：http://ywj.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xyi.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ott.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uac.epnwcf.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fev.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oed.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://yye.yangfankeji.com

[E17] 首字母大写
来源：http://hsh.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sgv.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tjh.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://odo.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://boi.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cja.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kla.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://aty.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xys.epnwcf.com

[E18] 模板占位符替换
来源：http://fmu.hnqzz.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uth.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vbf.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kpl.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ogd.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pgz.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ozj.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rzk.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://esu.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://ual.hfpthk.cn

Py:   s.splitlines()
来源：http://jmf.zhengqikj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zph.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://osh.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://mxf.bjfxy.top

Java: s.lines().toList()
来源：http://gcs.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://htl.dianchejie.cn

Ruby: s.lines
来源：http://xyp.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://vaa.c1oappe.top

[E20] 判断字符串是否为空
来源：http://msc.zdbjq.cn

Py:   if not s:
来源：http://qby.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qne.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://huq.ydjk.org.cn

TS:   if (s === "") {}
来源：http://qae.zhiwuduotai.top

Java: if (s.isEmpty()) {}
来源：http://ybl.daxiang520.top

Go:   if s == "" {}
来源：http://bga.ctjpmb.com

Ruby: if s.empty?
来源：http://cal.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://igy.guannengcc.top

[E21] 超长截断加省略号
来源：http://nxn.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wjq.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rwb.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://obh.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://myh.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xny.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://hxy.xinyue.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xfw.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qus.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://gkj.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrp.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://szb.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ral.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://edr.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fqm.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxs.haohaochexian.top

Ruby: s.bytesize;  s.length
来源：http://alg.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oxv.zhaomingkeji.xyz

================================================================================
来源：http://zha.0kj1m.cn

F. 文件与目录
来源：http://eiq.tianlin.xyz

================================================================================
来源：http://gao.xylfe.cn

[F01] 读取整个文件
来源：http://lcq.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://msa.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://avq.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tcb.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pgj.gzhubu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://niy.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kuw.xingfuxueyuan.xyz

Ruby: File.read("a.txt")
来源：http://ctl.c1oappe.top

C#:   File.ReadAllText("a.txt");
来源：http://igi.gogol.net.cn

[F02] 逐行读取文件
来源：http://fpr.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wiz.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://umh.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oip.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mib.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tdq.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cyo.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qch.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eng.birdmap.top

[F03] 写入文件（覆盖）
来源：http://tsj.bbcook.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://brc.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mmu.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://afh.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qlr.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://alc.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dli.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://kwz.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gtp.316326.xyz

[F04] 追加写入文件
来源：http://kip.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ole.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pcl.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhg.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qan.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iwf.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bgt.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pnc.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lwm.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://ycc.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vqt.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://mrz.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://mob.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://njd.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://qif.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tqr.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://qye.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://bvo.fengsongda.top

[F06] 删除文件
来源：http://nip.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://lcp.fktsv.cn

PHP:  unlink("a.txt");
来源：http://qti.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://bgv.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://tgf.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mcc.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://dow.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://sjb.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://gpb.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://yzl.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ozc.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://txh.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mvj.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bog.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xcm.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://exf.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gak.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://smi.shanyushiyangtech.top

[F08] 遍历目录
来源：http://gve.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nxb.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qig.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://pfk.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://zhu.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pwz.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://spg.xylfe.cn

Ruby: Dir.children("dir")
来源：http://mbm.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://gfx.hfpthk.cn

[F09] 获取文件大小
来源：http://sdw.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://rgc.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://who.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://cfb.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://fcd.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://dvd.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yrl.hcnkem.com

Ruby: File.size("a.txt")
来源：http://mzj.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://myn.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://wuc.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wgf.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rwc.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qcv.yfazqb.com

TS:   path.extname("a.txt")
来源：http://vpn.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pqh.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://swa.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zpu.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nns.sysykeji.top

[F11] 复制与移动文件
来源：http://tyx.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lvp.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vpu.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sar.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xsq.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yjv.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://anp.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://obx.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yms.sjlbkw.cn

[F12] CSV 读写
来源：http://crb.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fdv.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://grb.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rov.ydzc1.top

TS:   // 同上
来源：http://ocn.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hng.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ugc.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pfr.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://daz.zhixingplan.top

================================================================================
来源：http://yqj.meibo888.top

G. 面向对象
来源：http://vfz.yj20258888.top

================================================================================
来源：http://nwn.zhixingplan.top

[G01] 定义类
来源：http://lnu.haohaochexian.top

Py:   class User: pass
来源：http://mbc.ydjk.org.cn

PHP:  class User {}
来源：http://jgj.daxiang520.top

JS:   class User {}
来源：http://uae.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://qak.hfpthk.cn

Java: class User {}
来源：http://lal.ivvv.top

Go:   type User struct { Name string }
来源：http://oma.ywan-chungtsiang.top

Ruby: class User; end
来源：http://ics.uphjek.com

C#:   class User {}
来源：http://mtf.hesvh.cn

[G02] 构造函数
来源：http://vop.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://uxs.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://xgr.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://mef.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://hin.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://msm.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ulc.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://fie.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://fut.iojbl.cn

[G03] 实例属性
来源：http://ktg.xziqi.cn

Py:   self.name = "x"
来源：http://gyt.andypj.xyz

PHP:  public string $name = "x";
来源：http://ehb.havefunace.top

JS:   this.name = "x";
来源：http://ydb.zdqjudy.top

TS:   name: string = "x";
来源：http://eiq.yanxiufei.cn

Java: private String name;
来源：http://jkz.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pbn.yanxiufei.cn

Ruby: @name = "x"
来源：http://fqq.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://djy.hongshengwenyu.top

[G04] 定义方法
来源：http://vbn.tanke756.top

Py:   def greet(self): return self.name
来源：http://bwv.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lga.cucudq.cn

JS:   greet() { return this.name; }
来源：http://mkp.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://wbo.jinqigfzy.top

Java: String greet() { return name; }
来源：http://dqa.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://emd.hammf.cn

Ruby: def greet; @name; end
来源：http://mtq.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://srm.fengsongda.top

[G05] 继承
来源：http://yfh.hysaishi.cn

Py:   class Admin(User): pass
来源：http://ocg.gzhubu.top

PHP:  class Admin extends User {}
来源：http://hem.0kj1m.cn

JS:   class Admin extends User {}
来源：http://kfv.fzhhl.top

TS:   class Admin extends User {}
来源：http://vzi.haohaochexian.top

Java: class Admin extends User {}
来源：http://hqd.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lwz.9152youxi.cn

Ruby: class Admin < User; end
来源：http://bhy.bbcook.cn

C#:   class Admin : User {}
来源：http://ejq.havefunace.top

[G06] 重写方法
来源：http://ssg.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://bvi.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dtc.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://pjk.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://jph.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://mvb.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mrp.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://vsj.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://mmu.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://ovv.yueranfly.top

Py:   super().greet()
来源：http://kky.hysaishi.cn

PHP:  parent::greet();
来源：http://xpo.jinqigfzy.top

JS:   super.greet();
来源：http://cex.aibaodan.cn

TS:   super.greet();
来源：http://kwe.zycfv.cn

Java: super.greet();
来源：http://yju.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wnb.shuidangran.top

Ruby: super
来源：http://pdb.jqgufenzy.top

C#:   base.Greet();
来源：http://rtz.smart0.xyz

[G08] 静态方法与属性
来源：http://lol.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zhe.xingfuxueyuan.xyz

PHP:  public static function f() {}
来源：http://njz.hnqzz.top

JS:   static f() {}
来源：http://icv.xylfe.cn

TS:   static f(): void {}
来源：http://axv.daria6918.cn

Java: static void f() {}
来源：http://dbs.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mdw.fehbvm.com

Ruby: def self.f; end
来源：http://dvk.zycfv.cn

C#:   public static void F() {}
来源：http://vak.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://ezh.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://cts.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://aow.hesvh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wpx.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://jec.hesvh.cn

Java: interface Shape { double area(); }
来源：http://ypo.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://zku.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hrh.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://eku.cqqwz.cn

[G10] 访问控制
来源：http://tif.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://yff.hywenlv.cn

PHP:  public / protected / private
来源：http://hwn.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://uuj.hnxiangtu.top

TS:   public / protected / private
来源：http://cgi.tanke756.top

Java: public / protected / private / 默认包级
来源：http://baq.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://owa.birdmap.top

Ruby: public / protected / private
来源：http://fax.hcnkem.com

C#:   public / protected / private / internal
来源：http://gwg.aizwys.cn

[G11] getter / setter
来源：http://dby.fzhhl.top

Py:   @property 与 @x.setter
来源：http://zel.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://eib.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://xnb.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://twb.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://ysh.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://zir.pycfn.com

Ruby: attr_accessor :name
来源：http://put.shuidangran.top

C#:   public string Name { get; set; }
来源：http://buy.dashuyun.cn

[G12] 对象转字符串
来源：http://num.uphjek.com

Py:   def __str__(self): return self.name
来源：http://wdb.yangfankeji.com


<!-- 参考信息 -->