代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://xaa.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zwj.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qem.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://vix.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://nvd.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://mhf.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rkx.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kjn.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://prd.yuxming.cn

[E11] 反转字符串
来源：http://mss.yfazqb.com

Py:   s[::-1]
来源：http://gvh.bbcook.cn

PHP:  strrev($s);
来源：http://amo.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://tth.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://hsb.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hll.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://egg.guowangkeji.top

Ruby: s.reverse
来源：http://pqu.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://exd.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://asi.gzhubu.top

Py:   s.count("a")
来源：http://ynn.yanxiufei.cn

PHP:  substr_count($s, "a");
来源：http://ysh.yvedp.cn

JS:   s.split("a").length - 1
来源：http://sdw.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://yny.fanxiaobao.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wau.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://dek.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://jpz.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://lht.ydjk.org.cn

[E13] 逐字符遍历
来源：http://jai.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://ptc.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dgm.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gby.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://psp.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rtt.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cvp.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rji.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://suf.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://zdq.meibo888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://whi.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bms.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zxg.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pkb.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wrd.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xjn.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://isi.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eaj.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://rji.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jmc.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jqr.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hsg.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://kwh.cdnleiting.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vpm.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nvr.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tsd.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lmw.hongshengwenyu.top

[E16] 数字千分位
来源：http://pzb.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://hhc.andypj.xyz

PHP:  number_format(1234567);
来源：http://cch.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vyd.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gxc.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nzk.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uja.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qlx.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://uol.hysaishi.cn

[E17] 首字母大写
来源：http://zhk.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wnm.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ghz.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hzv.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ril.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kpz.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://akd.gzhubu.top

Ruby: s.capitalize
来源：http://znc.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rbk.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://zpa.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lcr.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aab.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://qop.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://chz.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://doj.fehbvm.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kxx.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mej.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sxn.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://mzy.shuidangran.top

Py:   s.splitlines()
来源：http://bxp.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tha.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://prj.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://vkd.sjlbkw.cn

Java: s.lines().toList()
来源：http://fcq.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://bim.vehdjk.com

Ruby: s.lines
来源：http://sqn.svipenyu.cn

C#:   s.Split('\n')
来源：http://jvg.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://qxd.sweek.top

Py:   if not s:
来源：http://wss.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rxm.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hpu.chenzaomai.com

TS:   if (s === "") {}
来源：http://whf.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://jzo.yongpay.top

Go:   if s == "" {}
来源：http://swu.gaohongyu789.top

Ruby: if s.empty?
来源：http://gzy.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yql.snrcjt.cn

[E21] 超长截断加省略号
来源：http://mxk.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cfo.sxryk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xiw.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jpc.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dtg.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ybp.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://mpg.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://izp.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tvz.sweek.top

[E22] 字节长度与字符长度
来源：http://vzz.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://whe.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://irs.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fim.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wdl.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ryx.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rvy.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://qxe.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czj.shanyushiyangkeji.top

================================================================================
来源：http://mta.kuanghao11.cn

F. 文件与目录
来源：http://vvp.hnqzz.top

================================================================================
来源：http://yof.c1oappe.top

[F01] 读取整个文件
来源：http://lnv.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kvs.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://ucs.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uwb.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vlr.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xox.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hff.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://tck.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://sgn.iojbl.cn

[F02] 逐行读取文件
来源：http://ehz.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://anz.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fgz.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hzy.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syd.zhongyouzk.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://euk.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://noj.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gya.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lnq.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://lyp.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qzv.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://udp.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mui.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cvr.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://myg.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ntz.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://tte.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aod.xuanzx.com

[F04] 追加写入文件
来源：http://izl.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gzo.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ftp.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://utg.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qda.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ieh.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://itb.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dho.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://skg.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://frv.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nid.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://der.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://ksl.xingfuxueyuan.xyz

TS:   fs.existsSync("a.txt")
来源：http://rjp.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://azf.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gay.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://joa.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://fzx.ivvv.top

[F06] 删除文件
来源：http://hhp.hammf.cn

Py:   os.remove("a.txt")
来源：http://wmq.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://qjk.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://gsj.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://jav.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mkh.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://dnx.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://wxj.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://gbi.hcnkem.com

[F07] 创建目录（含多级）
来源：http://lcq.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zum.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ctl.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://adn.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aap.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nkm.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aun.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqg.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nbr.sysykeji.top

[F08] 遍历目录
来源：http://zhb.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fbb.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bht.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://kgm.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://ytq.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wii.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ifo.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://hiq.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://qly.hnxiangtu.top

[F09] 获取文件大小
来源：http://nkf.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://xxk.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://arh.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://plv.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://qmy.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zrx.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qcc.c1oappe.top

Ruby: File.size("a.txt")
来源：http://ezv.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://uvd.ybcxt.top

[F10] 取文件扩展名 / 文件名
来源：http://bpb.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gjx.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sag.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gka.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://rem.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kuj.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iah.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dfs.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjq.epnwcf.com

[F11] 复制与移动文件
来源：http://pka.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vcu.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iga.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqt.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hib.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bpr.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vbe.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ffz.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zrr.gogol.net.cn

[F12] CSV 读写
来源：http://bfh.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://crk.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivt.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://itp.yuxming.cn

TS:   // 同上
来源：http://awi.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://elx.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wga.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xhf.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xht.zhongyouzk.top

================================================================================
来源：http://zbs.c1oappe.top

G. 面向对象
来源：http://ifi.zhaomingkeji.xyz

================================================================================
来源：http://usa.wangshuangyany.cn

[G01] 定义类
来源：http://upa.cucudq.cn

Py:   class User: pass
来源：http://veg.yonumen.top

PHP:  class User {}
来源：http://mfo.hfpthk.cn

JS:   class User {}
来源：http://tpd.bjfxy.top

TS:   class User { name: string = ""; }
来源：http://tde.fehbvm.com

Java: class User {}
来源：http://tlm.316326.xyz

Go:   type User struct { Name string }
来源：http://iaf.shangyingyoupin.top

Ruby: class User; end
来源：http://myb.cdnleiting.top

C#:   class User {}
来源：http://ncy.chenzaomai.com

[G02] 构造函数
来源：http://mas.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://gne.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://emq.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://ggv.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://ixo.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://ycf.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://unn.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://tyu.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://dth.andypj.xyz

[G03] 实例属性
来源：http://pql.zycfv.cn

Py:   self.name = "x"
来源：http://emz.mhx1999.top

PHP:  public string $name = "x";
来源：http://ikh.pengpengdd.cyou

JS:   this.name = "x";
来源：http://chq.sxryk.cn

TS:   name: string = "x";
来源：http://qti.316326.xyz

Java: private String name;
来源：http://oon.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jmg.chenlongwang.top

Ruby: @name = "x"
来源：http://pqn.fengsongda.top

C#:   public string Name { get; set; } = "x";
来源：http://tvi.uphjek.com

[G04] 定义方法
来源：http://bpa.ivvv.top

Py:   def greet(self): return self.name
来源：http://nmg.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yhe.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://ick.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://wge.mhx1999.top

Java: String greet() { return name; }
来源：http://iyz.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://jdl.tian-w.cn

Ruby: def greet; @name; end
来源：http://usd.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://ogk.vehdjk.com

[G05] 继承
来源：http://uwv.cdnleiting.top

Py:   class Admin(User): pass
来源：http://yvr.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://mym.hesvh.cn

JS:   class Admin extends User {}
来源：http://ggp.ppjwa.cn

TS:   class Admin extends User {}
来源：http://pdu.9152youxi.cn

Java: class Admin extends User {}
来源：http://ilu.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vyu.fengsongda.top

Ruby: class Admin < User; end
来源：http://iyp.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://rnv.cheryme.top

[G06] 重写方法
来源：http://gwd.cashguo.top

Py:   def greet(self): return "admin"
来源：http://zlq.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://acv.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://zrl.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://nli.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://jgn.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://neb.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://srx.sysykeji.top

C#:   public override string Greet() => "admin";
来源：http://omf.wangdashe.top

[G07] 调用父类方法
来源：http://vhq.yvedp.cn

Py:   super().greet()
来源：http://xvn.zdbjq.cn

PHP:  parent::greet();
来源：http://wsm.sweek.top

JS:   super.greet();
来源：http://xvm.jqgfzy.top

TS:   super.greet();
来源：http://ced.jlsjyb.cn

Java: super.greet();
来源：http://zrl.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jkb.feifeiyinyue.top

Ruby: super
来源：http://chz.fanxiaobao.xyz

C#:   base.Greet();
来源：http://vbk.zhoulong.xyz

[G08] 静态方法与属性
来源：http://xlr.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pyn.jinqigufen.top

PHP:  public static function f() {}
来源：http://kwa.hfpthk.cn

JS:   static f() {}
来源：http://pnx.pengpengdd.cyou

TS:   static f(): void {}
来源：http://rfj.c1oappe.top

Java: static void f() {}
来源：http://lub.hesvh.cn


<!-- 参考信息 -->