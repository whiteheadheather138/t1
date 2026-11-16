代发 wailian999

Ruby: s.reverse
来源：http://rql.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://ttv.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://amh.haohaochexian.top

Py:   s.count("a")
来源：http://yyc.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://vkl.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://zgk.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://vvw.hammf.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rtb.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://mod.hnxiangtu.top

Ruby: s.count("a")
来源：http://snt.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://dyp.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://tke.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://jiq.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zkt.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnp.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cyy.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://erm.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iqf.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://jiw.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mjl.yj202588.top

[E14] URL 编码与 Base64
来源：http://uew.ehwqpu.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dbp.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lio.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qff.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://obf.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ucz.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ozm.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rhj.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cvu.xylfe.cn

[E15] HTML 转义 / 反转义
来源：http://qbm.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jpu.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jdg.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rzf.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aww.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rpy.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cqc.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vuz.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nkh.epnwcf.com

[E16] 数字千分位
来源：http://mdf.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://kbd.tanke756.top

PHP:  number_format(1234567);
来源：http://ptv.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hki.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://suu.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pme.ybcxt.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bxa.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iec.hammf.cn

C#:   1234567.ToString("N0")
来源：http://idu.yj20258.top

[E17] 首字母大写
来源：http://cgn.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kcr.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tsq.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://snj.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://znu.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mxg.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eiu.shangyingyoupin.top

Ruby: s.capitalize
来源：http://gdg.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://obd.sysykeji.top

[E18] 模板占位符替换
来源：http://gpq.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fyg.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jkm.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bug.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qpr.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dtg.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dfy.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fuf.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zbs.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://yog.pycfn.com

Py:   s.splitlines()
来源：http://tkg.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xlv.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://sfu.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://syh.chenlongwang.top

Java: s.lines().toList()
来源：http://tuk.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://xxj.ybcxt.top

Ruby: s.lines
来源：http://rmc.zhijiandao.cn

C#:   s.Split('\n')
来源：http://hlu.yvedp.cn

[E20] 判断字符串是否为空
来源：http://sxl.daria6918.cn

Py:   if not s:
来源：http://avh.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vfn.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wtd.ybcxt.top

TS:   if (s === "") {}
来源：http://lmx.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://vtb.jiagoushi.top

Go:   if s == "" {}
来源：http://uif.yonumen.top

Ruby: if s.empty?
来源：http://tsd.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gxq.fehbvm.com

[E21] 超长截断加省略号
来源：http://vly.hammf.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dpz.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ntf.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vqn.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mfz.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://osb.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://ygv.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hiu.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uoi.zycfv.cn

[E22] 字节长度与字符长度
来源：http://ezr.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wws.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fsj.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://swn.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yij.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cet.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ksk.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://raz.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qqq.hnxiangtu.top

================================================================================
来源：http://rkb.yuanzhike.top

F. 文件与目录
来源：http://wvh.sjlbkw.cn

================================================================================
来源：http://cys.cashguo.top

[F01] 读取整个文件
来源：http://mwr.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jff.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://kbv.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://euv.cqqwz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hvp.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://coa.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xdy.fktsv.cn

Ruby: File.read("a.txt")
来源：http://jgj.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://sma.yj202588.top

[F02] 逐行读取文件
来源：http://qyn.wangshuangyany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jzu.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mtu.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixb.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yer.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://igx.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wbp.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xpr.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jmu.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://xoh.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nbi.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://egh.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wbx.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rju.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zom.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bia.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://mtd.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ikj.zhongyouzk.top

[F04] 追加写入文件
来源：http://rou.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mow.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bmm.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxm.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tku.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ord.sjlbkw.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://upm.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mim.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ldv.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://vef.ctjpmb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dug.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://ymm.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://oyk.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://clf.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kru.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rnc.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://ipo.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://mgc.meibo888.top

[F06] 删除文件
来源：http://ozq.yj20258888.top

Py:   os.remove("a.txt")
来源：http://crp.ybcxt.top

PHP:  unlink("a.txt");
来源：http://eql.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://wjn.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://lft.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ggj.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://owg.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://xox.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://rki.redwolf501.top

[F07] 创建目录（含多级）
来源：http://zqt.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ezp.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oxm.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://twg.xuanzx.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zah.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ufe.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yvo.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wdm.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qqf.zhijiandao.cn

[F08] 遍历目录
来源：http://wbi.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://awk.havefunace.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://awo.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://fpc.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://nfp.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gor.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://wrs.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://jmp.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://cjl.pycfn.com

[F09] 获取文件大小
来源：http://hqk.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://uci.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://tvw.yanxiufei.cn

JS:   fs.statSync("a.txt").size
来源：http://ecu.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://vlt.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://xvn.jinqigfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cao.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://iiv.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://byv.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://dik.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://crl.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eog.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ipy.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://epf.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nwa.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ojy.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://woz.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ihv.9152youxi.cn

[F11] 复制与移动文件
来源：http://hzp.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://khb.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xoc.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sup.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mse.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kzk.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fln.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbg.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://esx.hfpthk.cn

[F12] CSV 读写
来源：http://aft.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hlt.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://spz.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wit.wangshuangyany.cn

TS:   // 同上
来源：http://kin.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://inb.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://peq.c1oappe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yeg.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mkt.guowangkeji.top

================================================================================
来源：http://tbp.xylfe.cn

G. 面向对象
来源：http://hlg.yongpay.top

================================================================================
来源：http://juf.dashuyun.cn

[G01] 定义类
来源：http://nro.zdqjudy.top

Py:   class User: pass
来源：http://rzq.chenzaomai.com

PHP:  class User {}
来源：http://rkp.316326.xyz

JS:   class User {}
来源：http://ohx.yongpay.top

TS:   class User { name: string = ""; }
来源：http://yas.birdmap.top

Java: class User {}
来源：http://cps.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://ima.fehbvm.com

Ruby: class User; end
来源：http://oaz.jqgfzy.top

C#:   class User {}
来源：http://kqt.yuanzhike.top

[G02] 构造函数
来源：http://nlp.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://pdj.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://vwb.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://osv.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://iwo.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://dwu.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ype.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://urj.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://ebk.hywenlv.cn

[G03] 实例属性
来源：http://bbk.daxiang520.top

Py:   self.name = "x"
来源：http://kjh.jyoumei.cn

PHP:  public string $name = "x";
来源：http://zjw.xziqi.cn

JS:   this.name = "x";
来源：http://yny.ctjpmb.com

TS:   name: string = "x";
来源：http://mlx.smart0.xyz

Java: private String name;
来源：http://ide.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://teb.daria6918.cn

Ruby: @name = "x"
来源：http://ckx.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://wzn.guannengcc.top

[G04] 定义方法
来源：http://cjr.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://szk.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zsv.ivvv.top

JS:   greet() { return this.name; }
来源：http://dkq.sweek.top

TS:   greet(): string { return this.name; }
来源：http://ukd.daxiang520.top

Java: String greet() { return name; }
来源：http://gug.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://zvv.cashguo.top

Ruby: def greet; @name; end
来源：http://bgk.hcnkem.com

C#:   public string Greet() => Name;
来源：http://cib.xziqi.cn

[G05] 继承
来源：http://bki.sxryk.cn

Py:   class Admin(User): pass
来源：http://rfn.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://tla.cheryme.top

JS:   class Admin extends User {}
来源：http://kxu.gotoacloud.top

TS:   class Admin extends User {}
来源：http://zsx.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://ykb.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdc.yvedp.cn

Ruby: class Admin < User; end
来源：http://zta.dashuyun.cn

C#:   class Admin : User {}
来源：http://eqe.zhiwuduotai.top

[G06] 重写方法
来源：http://lwo.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://tvm.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zzm.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://fll.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://ppb.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://jam.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nuc.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://wuv.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://rjh.yfazqb.com

[G07] 调用父类方法
来源：http://xgi.smart0.xyz

Py:   super().greet()
来源：http://xjt.sweek.top

PHP:  parent::greet();
来源：http://lvi.sxryk.cn

JS:   super.greet();
来源：http://kzl.svipenyu.cn

TS:   super.greet();
来源：http://jws.jinqigfzy.top

Java: super.greet();
来源：http://pcr.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mjw.yanxiufei.cn

Ruby: super
来源：http://ssg.fktsv.cn

C#:   base.Greet();
来源：http://wts.yj202588.top

[G08] 静态方法与属性
来源：http://jin.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://syc.epnwcf.com

PHP:  public static function f() {}
来源：http://oon.shangyingyoupin.top

JS:   static f() {}
来源：http://wxt.316326.xyz

TS:   static f(): void {}
来源：http://gyc.hcnkem.com

Java: static void f() {}
来源：http://ath.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ojo.nanxinkj.top

Ruby: def self.f; end
来源：http://jsi.svipenyu.cn

C#:   public static void F() {}
来源：http://asp.sweek.top

[G09] 接口 / 抽象类
来源：http://elz.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://jwk.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uaf.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mah.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://gjk.bbcook.cn

Java: interface Shape { double area(); }
来源：http://nkh.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://vyd.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gnz.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://mha.sjlbkw.cn

[G10] 访问控制
来源：http://mvi.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://mdn.yueranfly.top

PHP:  public / protected / private
来源：http://fks.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://faj.hesvh.cn


<!-- 参考信息 -->