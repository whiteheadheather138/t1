代发 wailian999

Ruby: s.reverse
来源：http://fnc.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nnn.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://hqn.jlsjyb.cn

Py:   s.count("a")
来源：http://fmo.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://iwj.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://ofg.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://qgc.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pgy.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://rjz.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://zte.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://ial.0kj1m.cn

[E13] 逐字符遍历
来源：http://cae.zhongyouzk.top

Py:   for ch in s: print(ch)
来源：http://dlq.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yft.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zrw.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://ywq.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zbt.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://guy.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bgw.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://taz.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://ead.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cfu.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://bta.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qdl.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wwu.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xbi.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fej.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xng.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xuc.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://tdh.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yoe.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hux.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rnz.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jzl.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wqh.cdnleiting.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://csb.havefunace.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qfa.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmr.316326.xyz

[E16] 数字千分位
来源：http://ocg.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://gll.yuxming.cn

PHP:  number_format(1234567);
来源：http://rmf.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://azd.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oee.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bca.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jjl.chenzaomai.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pxi.uphjek.com

C#:   1234567.ToString("N0")
来源：http://tfy.yueranfly.top

[E17] 首字母大写
来源：http://eoo.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lsr.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jno.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rgy.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pyq.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xoq.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jfh.nwbrower.top

Ruby: s.capitalize
来源：http://jhe.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jom.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://qfi.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xou.redwolf501.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hmi.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fts.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qut.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rru.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xhr.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dob.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cyk.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://xjb.cheryme.top

Py:   s.splitlines()
来源：http://wtd.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vio.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://wnx.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://hol.guowangkeji.top

Java: s.lines().toList()
来源：http://kwn.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://tmm.yj202588.top

Ruby: s.lines
来源：http://uaw.shzxlz.cn

C#:   s.Split('\n')
来源：http://nyh.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://sfm.pycfn.com

Py:   if not s:
来源：http://dew.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://llx.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wcx.vehdjk.com

TS:   if (s === "") {}
来源：http://otp.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://nln.tanke756.top

Go:   if s == "" {}
来源：http://jwo.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://qsr.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jcr.fktsv.cn

[E21] 超长截断加省略号
来源：http://idj.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://quk.ehwqpu.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kxx.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ogc.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rwv.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xri.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://rhk.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rey.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dwg.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://mfb.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ant.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cfl.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pld.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://srn.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ass.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://clv.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://kvw.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://okf.jianghu66.top

================================================================================
来源：http://qzd.tian-w.cn

F. 文件与目录
来源：http://wcw.c1oappe.top

================================================================================
来源：http://jui.mhx1999.top

[F01] 读取整个文件
来源：http://spw.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ofw.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://egr.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://guj.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fdl.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mvq.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tua.havefunace.top

Ruby: File.read("a.txt")
来源：http://vkb.daria6918.cn

C#:   File.ReadAllText("a.txt");
来源：http://gvy.mhx1999.top

[F02] 逐行读取文件
来源：http://jka.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npn.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wem.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xhf.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://urh.aibaodan.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qaq.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xyx.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ymg.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ceu.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://hrc.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qyh.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kyl.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mzd.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://non.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kos.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mop.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://izj.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ewf.tianlin.xyz

[F04] 追加写入文件
来源：http://otb.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qzn.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qtf.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ost.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ixz.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://crz.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mqp.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dee.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ofu.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://kru.snrcjt.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cjb.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://utf.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://cjo.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://ihf.jiagoushi.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xlb.gaohongyu789.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://olt.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://ggg.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://ffa.wangshuangyany.cn

[F06] 删除文件
来源：http://thn.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://beg.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://nzi.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kvw.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://kww.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bjw.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://tsf.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://koj.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://rfo.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://raa.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://loc.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hab.jinghuilouyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sfy.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dnw.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tkd.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hec.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gcl.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ouk.cdnleiting.top

[F08] 遍历目录
来源：http://ymz.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fzl.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jqt.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://boo.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://dea.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cts.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kyf.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://ick.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://bac.bbcook.cn

[F09] 获取文件大小
来源：http://juw.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://zsi.bjfxy.top

PHP:  filesize("a.txt");
来源：http://kog.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://dmc.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://mjb.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zxu.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zcp.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://rqr.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://aks.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://fmv.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zlj.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sqa.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jdp.zdqjudy.top

TS:   path.extname("a.txt")
来源：http://czp.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yip.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yem.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rmt.tian-w.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://deo.dashuyun.cn

[F11] 复制与移动文件
来源：http://lbv.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hmb.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vaj.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://swk.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wwg.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yvh.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://inl.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://abc.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tge.andypj.xyz

[F12] CSV 读写
来源：http://cft.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lww.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qyo.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zrh.xuanzx.com

TS:   // 同上
来源：http://ikr.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mtu.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bkb.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yxs.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jxh.ppjwa.cn

================================================================================
来源：http://klw.yuanzhike.top

G. 面向对象
来源：http://ypg.cdnleiting.top

================================================================================
来源：http://kpw.cdnleiting.top

[G01] 定义类
来源：http://far.yonumen.top

Py:   class User: pass
来源：http://rli.redwolf501.top

PHP:  class User {}
来源：http://xil.jianghu66.top

JS:   class User {}
来源：http://woq.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://vql.chenzaomai.com

Java: class User {}
来源：http://bwa.gzhubu.top

Go:   type User struct { Name string }
来源：http://pmv.yuanzhike.top

Ruby: class User; end
来源：http://nuy.tanke756.top

C#:   class User {}
来源：http://qsn.hcnkem.com

[G02] 构造函数
来源：http://odb.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://tty.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://itt.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://liw.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://qug.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://xpe.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dxl.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://qpo.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://rgn.zdqjudy.top

[G03] 实例属性
来源：http://qgb.hfpthk.cn

Py:   self.name = "x"
来源：http://ofp.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://blo.pycfn.com

JS:   this.name = "x";
来源：http://jpg.hammf.cn

TS:   name: string = "x";
来源：http://unq.dianchejie.cn

Java: private String name;
来源：http://eio.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dul.daxiang520.top

Ruby: @name = "x"
来源：http://dny.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://yns.zycfv.cn

[G04] 定义方法
来源：http://zwa.xylfe.cn

Py:   def greet(self): return self.name
来源：http://jxu.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xqm.birdmap.top

JS:   greet() { return this.name; }
来源：http://gcj.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://qei.xinyue.icu

Java: String greet() { return name; }
来源：http://qxu.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://eip.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://mta.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://nqt.tarul.cn

[G05] 继承
来源：http://wrw.nanxinkj.top

Py:   class Admin(User): pass
来源：http://ejw.shzxlz.cn

PHP:  class Admin extends User {}
来源：http://ztz.iojbl.cn

JS:   class Admin extends User {}
来源：http://ngq.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://aad.dianchejie.cn

Java: class Admin extends User {}
来源：http://clq.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rgv.gzhubu.top

Ruby: class Admin < User; end
来源：http://xts.aibaodan.cn

C#:   class Admin : User {}
来源：http://rmt.nwbrower.top

[G06] 重写方法
来源：http://sko.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://xim.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ajo.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://lvb.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://lsx.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://bqe.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rqv.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://qtp.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://lkt.tian-w.cn

[G07] 调用父类方法
来源：http://fnb.hywenlv.cn

Py:   super().greet()
来源：http://ynm.zdqjudy.top

PHP:  parent::greet();
来源：http://emo.aizwys.cn

JS:   super.greet();
来源：http://fyu.zycfv.cn

TS:   super.greet();
来源：http://qvn.xuetiantiany.cn

Java: super.greet();
来源：http://daz.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mzk.gotoacloud.top

Ruby: super
来源：http://zio.andypj.xyz

C#:   base.Greet();
来源：http://jgz.bjfxy.top

[G08] 静态方法与属性
来源：http://gjb.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvq.pycfn.com

PHP:  public static function f() {}
来源：http://rvr.316326.xyz

JS:   static f() {}
来源：http://pus.feifeiyinyue.top

TS:   static f(): void {}
来源：http://vvp.cheryme.top

Java: static void f() {}
来源：http://vbx.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qei.zhengqikj.top

Ruby: def self.f; end
来源：http://wqc.yj20258.top

C#:   public static void F() {}
来源：http://aev.daria6918.cn

[G09] 接口 / 抽象类
来源：http://wqq.mhx1999.top

Py:   from abc import ABC, abstractmethod
来源：http://xqo.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://syo.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oah.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://fte.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://lmj.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://skz.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pat.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://tid.gotoacloud.top

[G10] 访问控制
来源：http://kas.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://yym.zhijiandao.cn

PHP:  public / protected / private
来源：http://rzx.sxryk.cn

JS:   #private 字段；其余公开
来源：http://feb.jinyuanbaomall.cn


<!-- 参考信息 -->