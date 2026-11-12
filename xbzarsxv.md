代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hzv.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://qmb.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://gui.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wnd.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://wjt.iojbl.cn

Ruby: s.count("a")
来源：http://fgu.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://cdt.ehwqpu.com

[E13] 逐字符遍历
来源：http://tzw.yonumen.top

Py:   for ch in s: print(ch)
来源：http://iip.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kny.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ojy.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yby.ehwqpu.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lxw.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xtp.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://zqk.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://awp.smart0.xyz

[E14] URL 编码与 Base64
来源：http://fnu.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://top.ehwqpu.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://tqr.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gqi.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fil.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://prb.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hsu.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lhd.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://orr.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://ccw.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mcx.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zry.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://snu.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ysq.chenjidiqi.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://byu.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fjj.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://toz.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xag.cucudq.cn

[E16] 数字千分位
来源：http://qmv.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://pek.hnqzz.top

PHP:  number_format(1234567);
来源：http://cug.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yxv.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://dbj.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://onl.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lsz.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bqa.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://gfn.hesvh.cn

[E17] 首字母大写
来源：http://myp.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rio.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://skm.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vob.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://egc.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://svj.ywan-chungtsiang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wdv.yj202588.top

Ruby: s.capitalize
来源：http://vyi.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wjw.jinqigfzy.top

[E18] 模板占位符替换
来源：http://kep.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zjs.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://exi.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://upt.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ggd.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lox.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://akj.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ofp.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hjh.birdmap.top

[E19] 多行文本按行拆分
来源：http://boq.iojbl.cn

Py:   s.splitlines()
来源：http://ajc.yj202588.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://myu.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://stj.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://ohp.nanxinkj.top

Java: s.lines().toList()
来源：http://usc.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://ndz.yj202588.top

Ruby: s.lines
来源：http://ycn.yvedp.cn

C#:   s.Split('\n')
来源：http://wrk.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://bfk.zhixingplan.top

Py:   if not s:
来源：http://ttk.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lws.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jrk.haohaochexian.top

TS:   if (s === "") {}
来源：http://bcd.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://gcz.haohaochexian.top

Go:   if s == "" {}
来源：http://upi.hywenlv.cn

Ruby: if s.empty?
来源：http://ajj.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hxu.hfpthk.cn

[E21] 超长截断加省略号
来源：http://zna.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mio.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dbc.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jha.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vqw.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://thv.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://fkn.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jxq.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tda.epnwcf.com

[E22] 字节长度与字符长度
来源：http://hle.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zli.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qzt.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ijb.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kkf.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pww.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dhs.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://dbt.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ysi.zdbjq.cn

================================================================================
来源：http://spd.yuxming.cn

F. 文件与目录
来源：http://vnr.gotoacloud.top

================================================================================
来源：http://ifc.jyoumei.cn

[F01] 读取整个文件
来源：http://yfp.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gwt.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://hwv.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oqp.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvu.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xas.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rev.fengsongda.top

Ruby: File.read("a.txt")
来源：http://ver.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://icd.cashguo.top

[F02] 逐行读取文件
来源：http://dwn.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bwh.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ljk.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sya.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mda.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ccw.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://msc.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://die.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qkr.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://jps.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iag.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ors.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mlk.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zct.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rgp.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gyx.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://wja.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hkg.jqgufenzy.top

[F04] 追加写入文件
来源：http://ynm.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lqz.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kwk.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uif.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xre.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nrs.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ylt.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://piu.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pgu.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://xju.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ska.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://ava.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://fpm.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://yth.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://scc.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://viu.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://aup.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://csf.jinyuanbaomall.cn

[F06] 删除文件
来源：http://ecc.guannengcc.top

Py:   os.remove("a.txt")
来源：http://kzb.yvedp.cn

PHP:  unlink("a.txt");
来源：http://mmy.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://ojr.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bgd.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uvv.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://gga.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://anl.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://sdu.yvedp.cn

[F07] 创建目录（含多级）
来源：http://zuf.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cjk.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dqc.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yfp.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfq.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lwk.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lcc.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pxc.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ffu.pengpengdd.cyou

[F08] 遍历目录
来源：http://tra.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://jcl.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kev.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://dqa.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://wfh.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://npe.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ypx.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://uen.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://tmc.pycfn.com

[F09] 获取文件大小
来源：http://nba.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://xdx.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://bez.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://dkg.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://wor.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hlg.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ryj.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://fil.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://qiw.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://fuc.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://orh.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mjz.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wea.cheryme.top

TS:   path.extname("a.txt")
来源：http://fec.zycfv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kzo.aizwys.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://brz.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://anq.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://khp.yj202588.top

[F11] 复制与移动文件
来源：http://jpr.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vfj.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xcn.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zbd.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kwh.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tpi.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gxb.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fug.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whw.tian-w.cn

[F12] CSV 读写
来源：http://gaw.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xgc.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hiu.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yau.zhixingplan.top

TS:   // 同上
来源：http://vzy.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xej.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vmm.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://asn.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zmw.shanyushiyangtech.top

================================================================================
来源：http://uva.sxryk.cn

G. 面向对象
来源：http://rqd.ydjk.org.cn

================================================================================
来源：http://tqg.guowangkeji.top

[G01] 定义类
来源：http://vzr.nanxuanxn.top

Py:   class User: pass
来源：http://uso.cqqwz.cn

PHP:  class User {}
来源：http://urk.bjfxy.top

JS:   class User {}
来源：http://kwy.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://vwa.xinyue.icu

Java: class User {}
来源：http://zom.zdbjq.cn

Go:   type User struct { Name string }
来源：http://cfo.ydzc1.top

Ruby: class User; end
来源：http://flx.ivvv.top

C#:   class User {}
来源：http://qpn.hywenlv.cn

[G02] 构造函数
来源：http://kie.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://jrz.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://hzh.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://mmv.yongpay.top

TS:   constructor(public name: string) {}
来源：http://hrp.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://and.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rtz.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://rsi.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://vum.sufxvd.cn

[G03] 实例属性
来源：http://cul.xinyue.icu

Py:   self.name = "x"
来源：http://tlz.daria6918.cn

PHP:  public string $name = "x";
来源：http://xer.xinyue.icu

JS:   this.name = "x";
来源：http://hqr.yvedp.cn

TS:   name: string = "x";
来源：http://pib.xuetiantiany.cn

Java: private String name;
来源：http://zcj.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rwf.redwolf501.top

Ruby: @name = "x"
来源：http://wot.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://bwk.ydzc1.top

[G04] 定义方法
来源：http://abt.zycfv.cn

Py:   def greet(self): return self.name
来源：http://hlc.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://fdp.havefunace.top

JS:   greet() { return this.name; }
来源：http://ujo.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://eaa.daxiang520.top

Java: String greet() { return name; }
来源：http://ugm.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://swf.hcnkem.com

Ruby: def greet; @name; end
来源：http://jsb.mhx1999.top

C#:   public string Greet() => Name;
来源：http://yzv.shanyushiyangkeji.top

[G05] 继承
来源：http://vzh.yonumen.top

Py:   class Admin(User): pass
来源：http://edc.gzhubu.top

PHP:  class Admin extends User {}
来源：http://cbx.hcnkem.com

JS:   class Admin extends User {}
来源：http://azr.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://zst.pycfn.com

Java: class Admin extends User {}
来源：http://zku.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ivu.hcnkem.com

Ruby: class Admin < User; end
来源：http://ttb.hnqzz.top

C#:   class Admin : User {}
来源：http://bdc.cashguo.top

[G06] 重写方法
来源：http://dyv.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://sei.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://srb.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://zxt.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://oot.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://zra.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cmt.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://csw.fehbvm.com

C#:   public override string Greet() => "admin";
来源：http://kiv.hnxiangtu.top

[G07] 调用父类方法
来源：http://jpy.chenjidiqi.icu

Py:   super().greet()
来源：http://jjf.vehdjk.com

PHP:  parent::greet();
来源：http://ehr.ehwqpu.com

JS:   super.greet();
来源：http://ytf.jyoumei.cn

TS:   super.greet();
来源：http://wsl.yangfankeji.com

Java: super.greet();
来源：http://jyg.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lhd.9152youxi.cn

Ruby: super
来源：http://ixc.bjfxy.top

C#:   base.Greet();
来源：http://qca.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://rjj.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lgc.jiagoushi.top

PHP:  public static function f() {}
来源：http://dbc.cheryme.top

JS:   static f() {}
来源：http://tap.yj20258888.top

TS:   static f(): void {}
来源：http://zqp.yj202588.top

Java: static void f() {}
来源：http://kaa.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nuu.ppjwa.cn

Ruby: def self.f; end
来源：http://qcu.yfazqb.com

C#:   public static void F() {}
来源：http://dox.bbcook.cn

[G09] 接口 / 抽象类
来源：http://kwm.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://ojo.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://lcj.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://llx.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://twr.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://xnw.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://fks.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dyd.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://glq.hfpthk.cn

[G10] 访问控制
来源：http://zhn.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://abi.jqgufenzy.top

PHP:  public / protected / private
来源：http://iba.guannengcc.top

JS:   #private 字段；其余公开
来源：http://tqm.yvedp.cn

TS:   public / protected / private
来源：http://rrg.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://ueb.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iav.tianlin.xyz

Ruby: public / protected / private
来源：http://yja.nanxinkj.top


<!-- 参考信息 -->