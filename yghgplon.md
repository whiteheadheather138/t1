代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://juv.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dfl.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://kvg.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://bzw.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://nkj.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://zda.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kji.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qhj.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://uzk.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mrn.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mqe.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://tjq.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://lzu.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://vjl.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vmf.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lfl.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zaj.daxiang520.top

[E11] 反转字符串
来源：http://rej.yangfankeji.com

Py:   s[::-1]
来源：http://iio.ppjwa.cn

PHP:  strrev($s);
来源：http://rvu.tarul.cn

JS:   [...s].reverse().join("")
来源：http://ywi.uphjek.com

TS:   [...s].reverse().join("")
来源：http://vss.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jbx.hfpthk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ugf.sweek.top

Ruby: s.reverse
来源：http://xkh.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tfc.andypj.xyz

[E12] 统计某字符出现次数
来源：http://vjv.ctjpmb.com

Py:   s.count("a")
来源：http://vsq.quarkkingdee.top

PHP:  substr_count($s, "a");
来源：http://xel.redwolf501.top

JS:   s.split("a").length - 1
来源：http://uhh.yj20258.top

TS:   s.split("a").length - 1
来源：http://nsy.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hwv.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://wjw.mhx1999.top

Ruby: s.count("a")
来源：http://lzl.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://ycd.jiagoushi.top

[E13] 逐字符遍历
来源：http://vpx.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://udg.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kxa.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mfn.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://chb.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gzj.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xal.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aza.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zkh.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://owr.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pyc.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ltr.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ykk.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rtm.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tdn.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mzb.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vlw.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pst.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://nxy.chenzaomai.com

Py:   html.escape(s);  html.unescape(s)
来源：http://fuj.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dfi.sjlbkw.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ter.vqdsnc.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yer.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cvg.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zbp.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gtr.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ipn.yangfankeji.com

[E16] 数字千分位
来源：http://kow.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://faq.svipenyu.cn

PHP:  number_format(1234567);
来源：http://ech.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ffx.zdqjudy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hjh.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rsj.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vkl.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pwp.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://atq.hnqzz.top

[E17] 首字母大写
来源：http://fvr.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zhz.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://srt.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yxw.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hwi.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://skn.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kit.jiagoushi.top

Ruby: s.capitalize
来源：http://ghe.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jyg.dashuyun.cn

[E18] 模板占位符替换
来源：http://wcq.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lok.shzxlz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://olb.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://kya.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vyc.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oxb.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nfm.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nms.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vem.daria6918.cn

[E19] 多行文本按行拆分
来源：http://oqa.aibaodan.cn

Py:   s.splitlines()
来源：http://mit.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ksu.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://sbj.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://tnx.wangdashe.top

Java: s.lines().toList()
来源：http://pkb.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://nej.sysykeji.top

Ruby: s.lines
来源：http://nyb.tarul.cn

C#:   s.Split('\n')
来源：http://vhu.fengsongda.top

[E20] 判断字符串是否为空
来源：http://all.andypj.xyz

Py:   if not s:
来源：http://prc.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ezo.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ssy.xuanzx.com

TS:   if (s === "") {}
来源：http://fnq.zhengqikj.top

Java: if (s.isEmpty()) {}
来源：http://lfz.ctjpmb.com

Go:   if s == "" {}
来源：http://ald.jlsjyb.cn

Ruby: if s.empty?
来源：http://mvs.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uhi.xziqi.cn

[E21] 超长截断加省略号
来源：http://qxq.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://epc.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aus.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://plt.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dki.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pmz.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://uek.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kzf.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://msf.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://bky.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aqo.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gsj.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsi.havefunace.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://noe.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://min.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mii.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://ofn.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uqu.sufxvd.cn

================================================================================
来源：http://fch.guowangkeji.top

F. 文件与目录
来源：http://sjm.fzhhl.top

================================================================================
来源：http://eek.gzhubu.top

[F01] 读取整个文件
来源：http://hxa.xinyue.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wxg.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://ola.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://crj.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nyw.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ull.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yvu.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://tox.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://fzx.shuidangran.top

[F02] 逐行读取文件
来源：http://ims.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bpk.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fmh.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gvz.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qpe.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ydm.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fwq.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fgt.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://isf.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://zcr.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wms.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://kmj.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ezd.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kwa.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ond.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jty.jiagoushi.top

Ruby: File.write("a.txt", "hi")
来源：http://kid.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://szw.aibaodan.cn

[F04] 追加写入文件
来源：http://unc.shzxlz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vlf.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oci.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dtz.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kte.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qkp.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hjy.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://owu.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jbv.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://yde.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://occ.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://hil.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://ssu.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://ouj.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://frf.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://knl.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://bky.sweek.top

C#:   File.Exists("a.txt")
来源：http://txn.havefunace.top

[F06] 删除文件
来源：http://dmf.yvedp.cn

Py:   os.remove("a.txt")
来源：http://lpg.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://xcb.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://omz.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hah.wangdashe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dfm.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://obx.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://eoy.wangdashe.top

C#:   File.Delete("a.txt");
来源：http://kip.yuanzhike.top

[F07] 创建目录（含多级）
来源：http://rtx.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://svw.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wow.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ibs.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://utx.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mwf.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hlu.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qgc.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uqf.tanke756.top

[F08] 遍历目录
来源：http://fbu.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xuk.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iyw.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://ljx.sweek.top

TS:   fs.readdirSync("dir")
来源：http://ndx.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://olc.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qnm.daria6918.cn

Ruby: Dir.children("dir")
来源：http://ard.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://els.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://nbn.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://get.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://fgb.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://bej.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://geo.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yql.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qjh.52xcode.cn

Ruby: File.size("a.txt")
来源：http://xkw.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://mge.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://wuq.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iqy.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jdw.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://snb.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://lwu.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bxp.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hhz.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aao.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gus.cashguo.top

[F11] 复制与移动文件
来源：http://fta.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tps.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mfk.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wsi.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://apc.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vmv.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qkc.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ogx.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hqo.shuidangran.top

[F12] CSV 读写
来源：http://kkp.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fur.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vea.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://let.yanxiufei.cn

TS:   // 同上
来源：http://huo.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qje.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zzt.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fga.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tou.yongpay.top

================================================================================
来源：http://lgu.yj20258.top

G. 面向对象
来源：http://bic.bjfxy.top

================================================================================
来源：http://zpv.sufxvd.cn

[G01] 定义类
来源：http://irs.yfazqb.com

Py:   class User: pass
来源：http://bme.shangyingyoupin.top

PHP:  class User {}
来源：http://lzm.feifeiyinyue.top

JS:   class User {}
来源：http://tfo.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://zbp.jiagoushi.top

Java: class User {}
来源：http://jkq.bjfxy.top

Go:   type User struct { Name string }
来源：http://inz.dashuyun.cn

Ruby: class User; end
来源：http://ras.zhijiandao.cn

C#:   class User {}
来源：http://mco.tian-w.cn

[G02] 构造函数
来源：http://vug.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://pii.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://iiu.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://nif.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://vbb.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://fwd.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hvw.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://pzd.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://aff.jinqigufen.top

[G03] 实例属性
来源：http://gvv.xuetiantiany.cn

Py:   self.name = "x"
来源：http://yus.hysaishi.cn

PHP:  public string $name = "x";
来源：http://wws.zhixingplan.top

JS:   this.name = "x";
来源：http://kka.bjfxy.top

TS:   name: string = "x";
来源：http://xmv.zhixingplan.top

Java: private String name;
来源：http://rlg.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://taw.aizwys.cn

Ruby: @name = "x"
来源：http://qbq.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://znr.shuidangran.top

[G04] 定义方法
来源：http://wyy.vehdjk.com

Py:   def greet(self): return self.name
来源：http://vzp.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ovv.c1oappe.top

JS:   greet() { return this.name; }
来源：http://bbj.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://dyg.cheryme.top

Java: String greet() { return name; }
来源：http://voo.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnk.iojbl.cn

Ruby: def greet; @name; end
来源：http://oex.smart0.xyz

C#:   public string Greet() => Name;
来源：http://hff.hammf.cn

[G05] 继承
来源：http://opk.fktsv.cn

Py:   class Admin(User): pass
来源：http://iei.yuxming.cn

PHP:  class Admin extends User {}
来源：http://dsy.yj20258888.top

JS:   class Admin extends User {}
来源：http://sbd.sufxvd.cn

TS:   class Admin extends User {}
来源：http://dmo.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://mca.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ozg.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://jvc.guannengcc.top

C#:   class Admin : User {}
来源：http://ofy.dashuyun.cn

[G06] 重写方法
来源：http://eca.yvedp.cn

Py:   def greet(self): return "admin"
来源：http://imt.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qqc.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://oel.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://tnn.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://tvl.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ofw.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://bad.yueranfly.top

C#:   public override string Greet() => "admin";
来源：http://zzk.zycfv.cn

[G07] 调用父类方法
来源：http://udn.pycfn.com

Py:   super().greet()
来源：http://utz.tarul.cn

PHP:  parent::greet();
来源：http://cli.aizwys.cn

JS:   super.greet();
来源：http://jxp.hammf.cn

TS:   super.greet();
来源：http://yxk.zycfv.cn

Java: super.greet();
来源：http://zpq.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fqp.bjfxy.top


<!-- 参考信息 -->