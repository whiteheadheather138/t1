代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://lpv.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://fsp.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gub.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vnd.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://slg.snrcjt.cn

[E11] 反转字符串
来源：http://hjr.zhengqikj.top

Py:   s[::-1]
来源：http://dhn.gzhubu.top

PHP:  strrev($s);
来源：http://qkm.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://zcr.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://psa.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bkb.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rrv.zycfv.cn

Ruby: s.reverse
来源：http://lty.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://bil.redwolf501.top

[E12] 统计某字符出现次数
来源：http://rvl.fehbvm.com

Py:   s.count("a")
来源：http://bye.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://joj.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://hem.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://twq.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qyh.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://ban.smart0.xyz

Ruby: s.count("a")
来源：http://yzg.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://eae.sjlbkw.cn

[E13] 逐字符遍历
来源：http://top.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://eoj.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wzb.c1oappe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uph.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://iio.sjlbkw.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zbo.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lfl.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sxk.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gcu.cucudq.cn

[E14] URL 编码与 Base64
来源：http://qmv.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://evg.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://qbh.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nkh.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yre.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hbl.yvedp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pxo.daria6918.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kdj.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hld.chenzaomai.com

[E15] HTML 转义 / 反转义
来源：http://wmo.quarkkingdee.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ywk.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jro.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cnh.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://axa.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ocu.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eyl.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://svv.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vkj.gzhubu.top

[E16] 数字千分位
来源：http://bot.cqqwz.cn

Py:   f"{1234567:,}"
来源：http://guc.9152youxi.cn

PHP:  number_format(1234567);
来源：http://fwl.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://hdi.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wja.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oau.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lsh.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ahd.yj202588.top

C#:   1234567.ToString("N0")
来源：http://idm.shanyushiyangtech.top

[E17] 首字母大写
来源：http://knq.ydjk.org.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nne.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ymb.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gak.hcnkem.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://juw.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fbr.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jgw.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://xjh.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://awa.iojbl.cn

[E18] 模板占位符替换
来源：http://ell.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ovd.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xqq.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xpa.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ldu.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wkx.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qqt.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pis.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywg.yj20258888.top

[E19] 多行文本按行拆分
来源：http://eth.hnxiangtu.top

Py:   s.splitlines()
来源：http://sco.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://icv.fehbvm.com

JS:   s.split(/\r?\n/)
来源：http://qek.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://qvm.zdqjudy.top

Java: s.lines().toList()
来源：http://dzj.shuidangran.top

Go:   strings.Split(s, "\n")
来源：http://obq.tanke756.top

Ruby: s.lines
来源：http://mnj.dashuyun.cn

C#:   s.Split('\n')
来源：http://sjf.yj20258888.top

[E20] 判断字符串是否为空
来源：http://gez.sjlbkw.cn

Py:   if not s:
来源：http://phv.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://anv.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vyq.yj20258.top

TS:   if (s === "") {}
来源：http://bcb.guannengcc.top

Java: if (s.isEmpty()) {}
来源：http://dxs.hfpthk.cn

Go:   if s == "" {}
来源：http://dle.ivvv.top

Ruby: if s.empty?
来源：http://mrp.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gni.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://uld.meibo888.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://maz.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://crb.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kro.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jvn.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aze.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://kxj.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yvp.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://upe.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://deg.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wht.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbq.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://izo.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yig.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bxr.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vtm.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://ygw.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://twi.aizwys.cn

================================================================================
来源：http://cjc.gogol.net.cn

F. 文件与目录
来源：http://dbu.sweek.top

================================================================================
来源：http://xes.wangdashe.top

[F01] 读取整个文件
来源：http://ntj.fanxiaobao.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pov.xingfuxueyuan.xyz

PHP:  file_get_contents("a.txt");
来源：http://ufa.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ntv.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mef.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://cmv.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://efm.xylfe.cn

Ruby: File.read("a.txt")
来源：http://wah.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://aik.xylfe.cn

[F02] 逐行读取文件
来源：http://tli.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://don.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zas.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://acm.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eew.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vdj.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ivn.pengpengdd.cyou

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qfp.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://khm.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://sns.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eza.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gam.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehy.ybcxt.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hmc.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gfn.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fot.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://vlx.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bfv.shangyingyoupin.top

[F04] 追加写入文件
来源：http://vud.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aum.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fos.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qax.yj20258.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xbz.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nwa.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nta.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nba.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ncy.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://rzi.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rzo.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://bvb.fengsongda.top

JS:   fs.existsSync("a.txt")
来源：http://nmk.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://gev.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://boy.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ojg.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://xol.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://mwo.hfpthk.cn

[F06] 删除文件
来源：http://zug.havefunace.top

Py:   os.remove("a.txt")
来源：http://tvr.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://ece.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://bsg.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://jyr.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wub.jqgfzy.top

Go:   os.Remove("a.txt")
来源：http://mfi.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://cnv.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://kme.xziqi.cn

[F07] 创建目录（含多级）
来源：http://wec.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fca.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rbi.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iho.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvc.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dur.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ozq.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://osd.hammf.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vax.meibo888.top

[F08] 遍历目录
来源：http://ynq.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xmh.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iqq.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://zam.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://obl.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nqh.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ndu.havefunace.top

Ruby: Dir.children("dir")
来源：http://uww.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://uwy.jianghu66.top

[F09] 获取文件大小
来源：http://jpe.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://lgu.andypj.xyz

PHP:  filesize("a.txt");
来源：http://bgn.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://tno.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://yvx.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://lkh.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://szl.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://mju.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://jqw.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://fin.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dvt.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nhx.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sur.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://fql.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://twu.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ueo.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gyd.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nor.ivvv.top

[F11] 复制与移动文件
来源：http://dfa.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://scx.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kum.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvf.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://veb.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cqg.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iez.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qff.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bjl.jqgfzy.top

[F12] CSV 读写
来源：http://pne.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cor.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dtp.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://glo.yangfankeji.com

TS:   // 同上
来源：http://wag.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://use.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pkt.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zeg.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://myz.aizwys.cn

================================================================================
来源：http://wel.tianlin.xyz

G. 面向对象
来源：http://fsa.316326.xyz

================================================================================
来源：http://sbu.xingfuxueyuan.xyz

[G01] 定义类
来源：http://ajo.cucudq.cn

Py:   class User: pass
来源：http://woh.ppjwa.cn

PHP:  class User {}
来源：http://fos.chenlongwang.top

JS:   class User {}
来源：http://euz.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://diu.jinqigufen.top

Java: class User {}
来源：http://sgj.shzxlz.cn

Go:   type User struct { Name string }
来源：http://iex.cucudq.cn

Ruby: class User; end
来源：http://eke.uphjek.com

C#:   class User {}
来源：http://wyg.zhaomingkeji.xyz

[G02] 构造函数
来源：http://xus.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://toh.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://sln.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://vki.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://xfc.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://spx.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kxt.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://kvi.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://kdn.fehbvm.com

[G03] 实例属性
来源：http://gcn.dianchejie.cn

Py:   self.name = "x"
来源：http://rqg.gotoacloud.top

PHP:  public string $name = "x";
来源：http://euy.sysykeji.top

JS:   this.name = "x";
来源：http://xel.yuxming.cn

TS:   name: string = "x";
来源：http://ucz.shangyingyoupin.top

Java: private String name;
来源：http://kkt.yangfankeji.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sei.52xcode.cn

Ruby: @name = "x"
来源：http://tij.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://qqe.feifeiyinyue.top

[G04] 定义方法
来源：http://hlf.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://lru.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wbc.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://dsn.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://izu.jianghu66.top

Java: String greet() { return name; }
来源：http://acm.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iso.9152youxi.cn

Ruby: def greet; @name; end
来源：http://shl.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://dwe.52xcode.cn

[G05] 继承
来源：http://ozy.zdqjudy.top

Py:   class Admin(User): pass
来源：http://tmr.quarkkingdee.top

PHP:  class Admin extends User {}
来源：http://ahu.yuanzhike.top

JS:   class Admin extends User {}
来源：http://smj.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://cdn.yuxming.cn

Java: class Admin extends User {}
来源：http://smj.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ndf.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://uhq.birdmap.top

C#:   class Admin : User {}
来源：http://ypw.jinyuanbaomall.cn

[G06] 重写方法
来源：http://fjy.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://wse.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mmf.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://wid.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://njq.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://gnr.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ora.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://lyg.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://sbm.jiagoushi.top

[G07] 调用父类方法
来源：http://fek.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://ljj.yuanzhike.top

PHP:  parent::greet();
来源：http://zzg.jqgufenzy.top

JS:   super.greet();
来源：http://yya.gaohongyu789.top

TS:   super.greet();
来源：http://cez.zhiwuduotai.top

Java: super.greet();
来源：http://luz.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://idt.jqgfzy.top

Ruby: super
来源：http://mpz.0kj1m.cn

C#:   base.Greet();
来源：http://wue.ydzc1.top

[G08] 静态方法与属性
来源：http://cag.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bru.fehbvm.com

PHP:  public static function f() {}
来源：http://pnd.zhongyouzk.top

JS:   static f() {}
来源：http://gcn.daria6918.cn

TS:   static f(): void {}
来源：http://voc.52xcode.cn

Java: static void f() {}
来源：http://fyv.pycfn.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://dgf.redwolf501.top

Ruby: def self.f; end
来源：http://oam.zhengqikj.top

C#:   public static void F() {}
来源：http://iyc.yuxming.cn

[G09] 接口 / 抽象类
来源：http://cfi.haohaochexian.top


<!-- 参考信息 -->