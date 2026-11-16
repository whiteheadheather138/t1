代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://gzw.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://hws.jianghu66.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ngc.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lio.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mut.sxryk.cn

[E11] 反转字符串
来源：http://gxr.hfpthk.cn

Py:   s[::-1]
来源：http://idz.jinqigfzy.top

PHP:  strrev($s);
来源：http://xjc.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://zrt.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://hbu.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qih.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dzh.jinqigfzy.top

Ruby: s.reverse
来源：http://evg.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://coj.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://kvq.gaohongyu789.top

Py:   s.count("a")
来源：http://cge.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://uuw.ybcxt.top

JS:   s.split("a").length - 1
来源：http://lce.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://qnd.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bdg.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://uwk.gzhubu.top

Ruby: s.count("a")
来源：http://zqw.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://lkd.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://fto.meibo888.top

Py:   for ch in s: print(ch)
来源：http://qsy.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qjc.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://wxs.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lxw.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pcg.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mhz.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nad.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://snp.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://zit.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://row.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dhj.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tok.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vow.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yqb.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jrv.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vnc.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ufs.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://mhz.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hrx.fengsongda.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nim.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jao.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nyn.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pjr.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://luo.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mio.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kuk.dashuyun.cn

[E16] 数字千分位
来源：http://cej.zhengqikj.top

Py:   f"{1234567:,}"
来源：http://kud.zycfv.cn

PHP:  number_format(1234567);
来源：http://azp.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mjs.jinghuilouyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kvt.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bze.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fmy.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qku.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://cfq.zhijiandao.cn

[E17] 首字母大写
来源：http://clk.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ved.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dng.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kdm.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nvo.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rzd.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bfo.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://neu.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pgo.vqdsnc.cn

[E18] 模板占位符替换
来源：http://zoz.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pwg.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wke.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rhg.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pyd.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qvs.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tqm.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rff.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://exw.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://gyf.yj20258.top

Py:   s.splitlines()
来源：http://qdg.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ffi.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://nwg.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://cww.shangyingyoupin.top

Java: s.lines().toList()
来源：http://tue.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://nec.hongshengwenyu.top

Ruby: s.lines
来源：http://uzj.jianghu66.top

C#:   s.Split('\n')
来源：http://ccg.bbcook.cn

[E20] 判断字符串是否为空
来源：http://trc.smart0.xyz

Py:   if not s:
来源：http://jys.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uly.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zpw.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://xlp.pycfn.com

Java: if (s.isEmpty()) {}
来源：http://lrw.meibo888.top

Go:   if s == "" {}
来源：http://ofj.iojbl.cn

Ruby: if s.empty?
来源：http://jvx.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ssn.xinyue.icu

[E21] 超长截断加省略号
来源：http://yyr.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rcu.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wbu.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nfk.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://enr.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ril.pengpengdd.cyou

Go:   // 按 rune 判断长度后截断
来源：http://per.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qdw.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wgr.uphjek.com

[E22] 字节长度与字符长度
来源：http://ivw.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lex.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blp.jlsjyb.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://riz.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kvp.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://umx.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hxj.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://rbz.guowangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wcg.vehdjk.com

================================================================================
来源：http://tls.redwolf501.top

F. 文件与目录
来源：http://egc.ctjpmb.com

================================================================================
来源：http://siw.guannengcc.top

[F01] 读取整个文件
来源：http://vsp.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iqc.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://hlg.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ggm.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://niy.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ccv.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://liy.shuidangran.top

Ruby: File.read("a.txt")
来源：http://oag.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://dsc.sxryk.cn

[F02] 逐行读取文件
来源：http://aqq.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ger.hfpthk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iuj.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xin.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pcx.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blu.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vng.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ypv.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dwm.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://qjj.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yvc.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wxd.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izj.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijj.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wil.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zrn.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://mmz.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oux.vqdsnc.cn

[F04] 追加写入文件
来源：http://cff.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vlm.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://klj.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://svw.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://obk.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wtx.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ckf.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vpj.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbw.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://dcu.hnqzz.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uaw.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://ouw.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://hjz.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://ixi.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://psr.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tek.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://ejt.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://bkp.feifeiyinyue.top

[F06] 删除文件
来源：http://ono.bbcook.cn

Py:   os.remove("a.txt")
来源：http://pwn.epnwcf.com

PHP:  unlink("a.txt");
来源：http://rkc.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://soy.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tig.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bty.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://kkz.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://flc.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://nba.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://toi.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jwb.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pbg.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yxy.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uew.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tzb.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jif.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://llk.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://knn.gzhubu.top

[F08] 遍历目录
来源：http://uzj.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uvx.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cvd.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://tcb.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://kvp.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://had.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fwm.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://kkn.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://gej.andypj.xyz

[F09] 获取文件大小
来源：http://rpb.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://hcy.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://zwh.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://ltn.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://pxn.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://rcm.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mci.hcnkem.com

Ruby: File.size("a.txt")
来源：http://oud.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://rco.cucudq.cn

[F10] 取文件扩展名 / 文件名
来源：http://agz.yfazqb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://neg.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tbk.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iau.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://fhy.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ufc.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rwi.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kin.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vya.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://ovu.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cgi.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcm.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqg.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ylc.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qat.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvl.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eho.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ajd.chenzaomai.com

[F12] CSV 读写
来源：http://mai.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pct.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nos.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dwd.ivvv.top

TS:   // 同上
来源：http://ujz.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rwy.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gjo.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lqg.zdbjq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yim.yuanzhike.top

================================================================================
来源：http://xio.yuanzhike.top

G. 面向对象
来源：http://jgx.hcnkem.com

================================================================================
来源：http://zju.yj20258888.top

[G01] 定义类
来源：http://fob.xziqi.cn

Py:   class User: pass
来源：http://kxv.jinqigufen.top

PHP:  class User {}
来源：http://uoz.aizwys.cn

JS:   class User {}
来源：http://hcs.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://ttm.guowangkeji.top

Java: class User {}
来源：http://tjm.tarul.cn

Go:   type User struct { Name string }
来源：http://cqa.dianchejie.cn

Ruby: class User; end
来源：http://hls.tianlin.xyz

C#:   class User {}
来源：http://mxp.kuanghao11.cn

[G02] 构造函数
来源：http://aav.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://zev.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://eli.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://vhu.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://epl.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://rbz.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ibr.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://boy.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://wwz.xziqi.cn

[G03] 实例属性
来源：http://hiw.daxiang520.top

Py:   self.name = "x"
来源：http://gcn.fehbvm.com

PHP:  public string $name = "x";
来源：http://yyf.ctjpmb.com

JS:   this.name = "x";
来源：http://ymz.hesvh.cn

TS:   name: string = "x";
来源：http://lrx.nanxinkj.top

Java: private String name;
来源：http://vdv.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eso.bbcook.cn

Ruby: @name = "x"
来源：http://fkt.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://kie.wangdashe.top

[G04] 定义方法
来源：http://mgh.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://qbt.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://klg.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://hyt.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://nfl.gaohongyu789.top

Java: String greet() { return name; }
来源：http://irj.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ibi.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://ngm.andypj.xyz

C#:   public string Greet() => Name;
来源：http://lab.zhixingplan.top

[G05] 继承
来源：http://tsr.meibo888.top

Py:   class Admin(User): pass
来源：http://bcy.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://gjf.yj20258.top

JS:   class Admin extends User {}
来源：http://fbq.hysaishi.cn

TS:   class Admin extends User {}
来源：http://ths.52xcode.cn

Java: class Admin extends User {}
来源：http://btd.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oqs.sweek.top

Ruby: class Admin < User; end
来源：http://kyz.zhixingplan.top

C#:   class Admin : User {}
来源：http://too.zhiwuduotai.top

[G06] 重写方法
来源：http://bws.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://yzo.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rgt.pycfn.com

JS:   greet() { return "admin"; }
来源：http://zht.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://qyh.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://sab.ybcxt.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ewn.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://pyk.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://ezf.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://sdn.jianghu66.top

Py:   super().greet()
来源：http://oea.fengsongda.top

PHP:  parent::greet();
来源：http://obf.kuanghao11.cn

JS:   super.greet();
来源：http://zkh.yongpay.top

TS:   super.greet();
来源：http://lic.quarkkingdee.top

Java: super.greet();
来源：http://lej.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hed.xziqi.cn

Ruby: super
来源：http://ree.zhiwuduotai.top

C#:   base.Greet();
来源：http://lna.cucudq.cn

[G08] 静态方法与属性
来源：http://inj.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fwe.guannengcc.top

PHP:  public static function f() {}
来源：http://edb.daria6918.cn

JS:   static f() {}
来源：http://rxm.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://bxz.hnqzz.top

Java: static void f() {}
来源：http://plh.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fnm.ivvv.top

Ruby: def self.f; end
来源：http://flq.meibo888.top

C#:   public static void F() {}
来源：http://spl.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://ifh.hnxiangtu.top


<!-- 参考信息 -->