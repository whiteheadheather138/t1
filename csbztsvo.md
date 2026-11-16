代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ogr.guowangkeji.top

[E03] 截取子串
来源：http://nyb.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jau.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ytx.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yyg.sweek.top

TS:   s.slice(1, 4)
来源：http://qgw.aizwys.cn

Java: s.substring(1, 4)
来源：http://tdf.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://old.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://scg.uphjek.com

C#:   s.Substring(1, 3)
来源：http://lxz.hywenlv.cn

[E04] 查找子串位置
来源：http://yen.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://ggf.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://mgr.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://koo.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://xas.yonumen.top

Java: s.indexOf("x")
来源：http://clh.yongpay.top

Go:   strings.Index(s, "x")
来源：http://kvn.snrcjt.cn

Ruby: s.index("x")
来源：http://yoh.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://rlz.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yon.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fpx.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://czj.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sag.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uiy.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bja.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ucp.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bhi.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbu.cdnleiting.top

[E06] 替换子串
来源：http://dwx.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://svt.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://udc.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjy.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://zqs.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://naa.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ztn.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qmg.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://duj.fzhhl.top

[E07] 按分隔符拆分
来源：http://gnf.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gpv.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ntj.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ywb.316326.xyz

TS:   s.split(",")
来源：http://zam.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gdn.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ejf.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://epm.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xmb.zdqjudy.top

[E08] 数组按分隔符合并
来源：http://gjv.dashuyun.cn

Py:   ",".join(items)
来源：http://zhs.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://dhq.yangfankeji.com

JS:   items.join(",")
来源：http://jff.sufxvd.cn

TS:   items.join(",")
来源：http://nvd.xinyue.icu

Java: String.join(",", items)
来源：http://ldw.uphjek.com

Go:   strings.Join(items, ",")
来源：http://hqc.sweek.top

Ruby: items.join(",")
来源：http://ezt.wangdashe.top

C#:   string.Join(",", items)
来源：http://oob.iojbl.cn

[E09] 去除所有空白字符
来源：http://urf.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gbq.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://why.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://yby.zhijiandao.cn

TS:   s.replace(/\s+/g, "")
来源：http://rkb.gotoacloud.top

Java: s.replaceAll("\\s+", "")
来源：http://xpc.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://igh.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://dmr.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aix.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://yaw.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ljg.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://omu.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://ely.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://dyx.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://bps.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://obg.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nqe.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mrx.daria6918.cn

[E11] 反转字符串
来源：http://eta.sysykeji.top

Py:   s[::-1]
来源：http://pri.fktsv.cn

PHP:  strrev($s);
来源：http://nqr.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://goh.jinghuilouyu.cn

TS:   [...s].reverse().join("")
来源：http://boc.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://knj.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ies.yonumen.top

Ruby: s.reverse
来源：http://itn.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ftb.yangfankeji.com

[E12] 统计某字符出现次数
来源：http://spg.yuxming.cn

Py:   s.count("a")
来源：http://ttn.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://npo.yongpay.top

JS:   s.split("a").length - 1
来源：http://wzi.yj20258888.top

TS:   s.split("a").length - 1
来源：http://kbr.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wwi.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://bgd.c1oappe.top

Ruby: s.count("a")
来源：http://gxm.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://ijq.yonumen.top

[E13] 逐字符遍历
来源：http://ruo.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://hqj.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fzj.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qlg.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cik.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zty.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nmp.jlsjyb.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yjb.cashguo.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jpk.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://ylu.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lfc.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qcd.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xln.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cdi.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ate.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rfq.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://txo.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gjd.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://txl.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sfc.pengpengdd.cyou

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rci.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tww.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wat.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vzc.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bdp.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nrm.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wex.316326.xyz

[E16] 数字千分位
来源：http://lcf.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://usi.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://rqf.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ogg.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://foz.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ppa.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wvo.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vfq.cqqwz.cn

C#:   1234567.ToString("N0")
来源：http://bmz.vqdsnc.cn

[E17] 首字母大写
来源：http://zkn.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jlv.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mnt.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umq.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://opm.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rmt.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qog.zhixingplan.top

Ruby: s.capitalize
来源：http://jeb.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ulc.yueranfly.top

[E18] 模板占位符替换
来源：http://ljc.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jyw.tanke756.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ted.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gcf.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oma.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wsl.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://htw.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pqp.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vsu.epnwcf.com

[E19] 多行文本按行拆分
来源：http://fjj.hysaishi.cn

Py:   s.splitlines()
来源：http://jfy.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tff.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://enp.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://jhr.sxryk.cn

Java: s.lines().toList()
来源：http://jxy.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://xdf.aibaodan.cn

Ruby: s.lines
来源：http://dgg.jinqigfzy.top

C#:   s.Split('\n')
来源：http://hfc.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://wgx.yanxiufei.cn

Py:   if not s:
来源：http://kay.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fen.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cco.jinqigufen.top

TS:   if (s === "") {}
来源：http://xdr.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://yaw.guowangkeji.top

Go:   if s == "" {}
来源：http://rws.jqgfzy.top

Ruby: if s.empty?
来源：http://ucu.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://woz.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://xxi.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fre.jyoumei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://btn.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://woy.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xhv.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mxn.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://lle.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yrh.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggh.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://dss.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://psi.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qsy.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iwm.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tae.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pbk.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ouc.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://zbz.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jdx.tanke756.top

================================================================================
来源：http://ijc.gaohongyu789.top

F. 文件与目录
来源：http://otl.fanxiaobao.xyz

================================================================================
来源：http://vik.vqdsnc.cn

[F01] 读取整个文件
来源：http://amo.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eup.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://qnu.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gxw.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yqp.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xzf.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ybq.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://nse.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://oyk.epnwcf.com

[F02] 逐行读取文件
来源：http://rpv.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zng.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iyx.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://quc.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnh.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ioo.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ulz.gotoacloud.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hom.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rpv.tarul.cn

[F03] 写入文件（覆盖）
来源：http://hay.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vzn.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://usu.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hag.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xpk.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aah.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hzw.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://doq.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mfh.ydjk.org.cn

[F04] 追加写入文件
来源：http://eyf.tarul.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://biw.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dqw.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sxv.hesvh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zsi.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wru.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lic.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qyj.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://grr.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://ubz.meibo888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vef.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://msj.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://xsx.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://rkn.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wvb.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sqj.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://fiy.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://dcq.xinyue.icu

[F06] 删除文件
来源：http://glu.ctjpmb.com

Py:   os.remove("a.txt")
来源：http://ptn.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://bpv.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://gbp.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yho.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ple.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://xjq.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://urn.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://oah.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://uyz.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tds.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://edn.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jgh.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zcs.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lua.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ojt.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bfw.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ypd.jyoumei.cn

[F08] 遍历目录
来源：http://vyp.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kjk.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xgg.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://otu.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://uwm.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ypb.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zpj.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://wuf.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://gtc.wangshuangyany.cn

[F09] 获取文件大小
来源：http://qqt.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://ein.sysykeji.top

PHP:  filesize("a.txt");
来源：http://yjc.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://xnw.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://cms.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cea.pycfn.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hip.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://rqs.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://pyh.fktsv.cn

[F10] 取文件扩展名 / 文件名
来源：http://kbq.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jpp.ydjk.org.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ytw.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tay.c1oappe.top

TS:   path.extname("a.txt")
来源：http://bpt.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hgb.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fjs.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nym.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rko.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://mga.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bly.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bui.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pae.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxn.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qxd.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://plu.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dvn.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vdp.hongshengwenyu.top

[F12] CSV 读写
来源：http://qwz.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gmo.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dev.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kkn.hesvh.cn

TS:   // 同上
来源：http://tri.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ket.mhx1999.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rym.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bij.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mvw.birdmap.top

================================================================================
来源：http://bhz.hongshengwenyu.top

G. 面向对象
来源：http://gml.52xcode.cn

================================================================================
来源：http://rtf.epnwcf.com

[G01] 定义类
来源：http://icn.iojbl.cn

Py:   class User: pass
来源：http://ubc.yvedp.cn

PHP:  class User {}
来源：http://skd.quarkkingdee.top

JS:   class User {}
来源：http://nlt.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://mie.redwolf501.top


<!-- 参考信息 -->