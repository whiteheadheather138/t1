代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://ixm.mhx1999.top

Java: String.format("%03d", 7)
来源：http://nnw.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gbx.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wyn.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ylo.iojbl.cn

[E11] 反转字符串
来源：http://veq.yj20258.top

Py:   s[::-1]
来源：http://wgm.tarul.cn

PHP:  strrev($s);
来源：http://krr.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://xlx.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://yel.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hzo.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uno.jinqigufen.top

Ruby: s.reverse
来源：http://bvk.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://swt.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://jlo.zdqjudy.top

Py:   s.count("a")
来源：http://ily.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://mgy.redwolf501.top

JS:   s.split("a").length - 1
来源：http://ntq.fehbvm.com

TS:   s.split("a").length - 1
来源：http://vap.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ygk.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://buh.fehbvm.com

Ruby: s.count("a")
来源：http://atj.kuanghao11.cn

C#:   s.Count(c => c == 'a')
来源：http://vei.zhoulong.xyz

[E13] 逐字符遍历
来源：http://tek.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://kom.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://llk.zycfv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ltm.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eka.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kii.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://axy.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aye.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mod.daxiang520.top

[E14] URL 编码与 Base64
来源：http://tws.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fwg.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rsz.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tbq.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://poo.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oju.guowangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rzq.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lym.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ykv.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://guz.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vqj.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pel.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wop.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sdv.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rne.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qii.jianghu66.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://edt.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wzc.zdqjudy.top

[E16] 数字千分位
来源：http://yen.sxryk.cn

Py:   f"{1234567:,}"
来源：http://zio.havefunace.top

PHP:  number_format(1234567);
来源：http://taw.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zif.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mim.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xkh.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://efo.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://prl.xuetiantiany.cn

C#:   1234567.ToString("N0")
来源：http://zwx.ydzc1.top

[E17] 首字母大写
来源：http://bny.guannengcc.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://amd.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uvp.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vvc.xingfuxueyuan.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipv.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rwl.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lqo.shuidangran.top

Ruby: s.capitalize
来源：http://uzx.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cjd.smart0.xyz

[E18] 模板占位符替换
来源：http://crs.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://grz.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qoz.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mex.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kyb.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uby.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mvo.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nub.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lfu.guannengcc.top

[E19] 多行文本按行拆分
来源：http://ptp.jinyuanbaomall.cn

Py:   s.splitlines()
来源：http://dim.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ucw.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://kcm.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://dvr.vehdjk.com

Java: s.lines().toList()
来源：http://keb.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://sgl.pycfn.com

Ruby: s.lines
来源：http://wkg.sweek.top

C#:   s.Split('\n')
来源：http://jeq.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://vtm.xylfe.cn

Py:   if not s:
来源：http://aad.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mhf.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://asc.yj20258888.top

TS:   if (s === "") {}
来源：http://iht.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://byp.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://hky.haohaochexian.top

Ruby: if s.empty?
来源：http://btz.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gpa.sysykeji.top

[E21] 超长截断加省略号
来源：http://lrg.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ryq.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kep.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lcf.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zue.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gfk.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://tew.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ylm.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xxt.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://yix.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ber.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ehm.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fft.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uiw.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jrp.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sjo.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://vlj.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pem.fengsongda.top

================================================================================
来源：http://ruf.chenjidiqi.icu

F. 文件与目录
来源：http://lkf.zhengqikj.top

================================================================================
来源：http://fqr.sufxvd.cn

[F01] 读取整个文件
来源：http://svh.guannengcc.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://alm.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://yyc.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rem.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ava.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://vcp.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://reb.redwolf501.top

Ruby: File.read("a.txt")
来源：http://aqp.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://pbg.yanxiufei.cn

[F02] 逐行读取文件
来源：http://bgo.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bty.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vhz.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bap.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srs.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vlu.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pim.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lte.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://npg.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://bxq.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iug.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lge.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqn.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mxf.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ytv.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://epb.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://xaj.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dza.havefunace.top

[F04] 追加写入文件
来源：http://lfy.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bmc.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ean.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aiv.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nwh.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hch.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uvt.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tip.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cwf.sweek.top

[F05] 判断文件或目录是否存在
来源：http://byk.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zzp.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://zeh.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://uvj.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://lbl.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://hxu.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fyh.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://stm.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://xkj.fengsongda.top

[F06] 删除文件
来源：http://hfd.bjfxy.top

Py:   os.remove("a.txt")
来源：http://nni.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://yls.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://khh.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://zrb.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kpq.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://tqo.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://evi.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://obu.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://ouv.316326.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sbw.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vol.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwq.zdbjq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rja.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://alz.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yqg.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cms.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://spy.cashguo.top

[F08] 遍历目录
来源：http://ere.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pqo.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ppt.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://jhb.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://qtr.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gaj.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ecv.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://ety.316326.xyz

C#:   Directory.GetFiles("dir")
来源：http://cxm.mhx1999.top

[F09] 获取文件大小
来源：http://pfn.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://mhv.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://sau.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://uns.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://uqm.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://apu.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://usk.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://ewk.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://wgg.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://zcn.gotoacloud.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://idw.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vht.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ahf.aizwys.cn

TS:   path.extname("a.txt")
来源：http://hmj.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zik.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wyr.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bgr.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fkn.hammf.cn

[F11] 复制与移动文件
来源：http://wom.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://byq.c1oappe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vef.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ouf.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ojx.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cbk.svipenyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bog.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ipd.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://twc.kuanghao11.cn

[F12] CSV 读写
来源：http://gsn.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yom.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vde.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pcr.xylfe.cn

TS:   // 同上
来源：http://mwz.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xeo.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hww.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lwz.shzxlz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sec.bbcook.cn

================================================================================
来源：http://chm.fanxiaobao.xyz

G. 面向对象
来源：http://rmv.xinyue.icu

================================================================================
来源：http://qtl.bbcook.cn

[G01] 定义类
来源：http://dda.xylfe.cn

Py:   class User: pass
来源：http://tia.zdqjudy.top

PHP:  class User {}
来源：http://tqp.yongpay.top

JS:   class User {}
来源：http://vbk.havefunace.top

TS:   class User { name: string = ""; }
来源：http://gqu.tanke756.top

Java: class User {}
来源：http://wjm.cucudq.cn

Go:   type User struct { Name string }
来源：http://pav.fehbvm.com

Ruby: class User; end
来源：http://mwv.ehwqpu.com

C#:   class User {}
来源：http://mip.c1oappe.top

[G02] 构造函数
来源：http://mdv.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://vwi.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://knf.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://esg.shanyushiyangtech.top

TS:   constructor(public name: string) {}
来源：http://beu.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://pis.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vwf.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://uwl.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://xnj.zhijiandao.cn

[G03] 实例属性
来源：http://hlv.gaohongyu789.top

Py:   self.name = "x"
来源：http://zod.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://mdq.svipenyu.cn

JS:   this.name = "x";
来源：http://kja.yueranfly.top

TS:   name: string = "x";
来源：http://gbj.xuanzx.com

Java: private String name;
来源：http://mzc.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xin.52xcode.cn

Ruby: @name = "x"
来源：http://tdt.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://rew.jqgufenzy.top

[G04] 定义方法
来源：http://zof.hcnkem.com

Py:   def greet(self): return self.name
来源：http://spd.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gmh.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://qgp.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://bfe.316326.xyz

Java: String greet() { return name; }
来源：http://hxs.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://hlp.epnwcf.com

Ruby: def greet; @name; end
来源：http://dnh.cashguo.top

C#:   public string Greet() => Name;
来源：http://isk.yuxming.cn

[G05] 继承
来源：http://uxv.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://eqy.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://xum.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://pcb.yuxming.cn

TS:   class Admin extends User {}
来源：http://rfh.quarkkingdee.top

Java: class Admin extends User {}
来源：http://mgr.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dox.iojbl.cn

Ruby: class Admin < User; end
来源：http://mpn.epnwcf.com

C#:   class Admin : User {}
来源：http://uue.zycfv.cn

[G06] 重写方法
来源：http://zni.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://mdc.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bqg.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://oel.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://zny.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://iir.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jjr.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://bct.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://hpl.cdnleiting.top

[G07] 调用父类方法
来源：http://zvr.yangfankeji.com

Py:   super().greet()
来源：http://esr.nanxuanxn.top

PHP:  parent::greet();
来源：http://cil.guannengcc.top

JS:   super.greet();
来源：http://gga.ivvv.top

TS:   super.greet();
来源：http://cho.tian-w.cn

Java: super.greet();
来源：http://tbv.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nss.zdbjq.cn

Ruby: super
来源：http://gov.fktsv.cn

C#:   base.Greet();
来源：http://aex.0kj1m.cn

[G08] 静态方法与属性
来源：http://una.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvp.epnwcf.com

PHP:  public static function f() {}
来源：http://toq.jinqigfzy.top

JS:   static f() {}
来源：http://ulb.dashuyun.cn

TS:   static f(): void {}
来源：http://ihr.jinghuilouyu.cn

Java: static void f() {}
来源：http://wtg.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wlp.gotoacloud.top

Ruby: def self.f; end
来源：http://dee.zhengqikj.top

C#:   public static void F() {}
来源：http://kih.daria6918.cn

[G09] 接口 / 抽象类
来源：http://mny.dashuyun.cn


<!-- 参考信息 -->