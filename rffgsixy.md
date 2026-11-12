代发 wailian999

Java: String.join(", ", list)
来源：http://wuo.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://pyg.yuxming.cn

Ruby: arr.join(", ")
来源：http://jip.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://tby.nanxinkj.top

================================================================================
来源：http://hdm.svipenyu.cn

E. 字符串处理
来源：http://fuh.gogol.net.cn

================================================================================
来源：http://bsc.yueranfly.top

[E01] 拼接字符串
来源：http://vvi.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qtt.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tvr.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hpu.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ewf.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ncd.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rhv.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rxa.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kdl.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://hwy.ydjk.org.cn

Py:   "ab" * 3
来源：http://iqf.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://xmv.shuidangran.top

JS:   "ab".repeat(3)
来源：http://ccv.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://qrt.havefunace.top

Java: "ab".repeat(3)
来源：http://ssw.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://dua.haohaochexian.top

Ruby: "ab" * 3
来源：http://uie.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gxx.gotoacloud.top

[E03] 截取子串
来源：http://cqr.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vqe.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ucx.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ywm.bbcook.cn

TS:   s.slice(1, 4)
来源：http://ftc.nanxinkj.top

Java: s.substring(1, 4)
来源：http://bbo.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xiz.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://ovd.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://ysj.gaohongyu789.top

[E04] 查找子串位置
来源：http://tvu.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://itk.redwolf501.top

PHP:  strpos($s, "x");
来源：http://irm.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qtk.yangfankeji.com

TS:   s.indexOf("x")
来源：http://fyl.316326.xyz

Java: s.indexOf("x")
来源：http://cuo.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://aev.ctjpmb.com

Ruby: s.index("x")
来源：http://cbn.c1oappe.top

C#:   s.IndexOf("x")
来源：http://xia.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dfh.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oeh.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iyi.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jvj.fehbvm.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://mru.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yot.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pgn.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://okk.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nzi.zycfv.cn

[E06] 替换子串
来源：http://fex.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wsy.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://hcv.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://job.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://kzk.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwq.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://roi.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ocq.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://oif.fehbvm.com

[E07] 按分隔符拆分
来源：http://otg.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tfy.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dih.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://orx.vehdjk.com

TS:   s.split(",")
来源：http://fhc.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://kvq.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rnz.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://zgz.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oqw.ivvv.top

[E08] 数组按分隔符合并
来源：http://xcl.ybcxt.top

Py:   ",".join(items)
来源：http://rfy.52xcode.cn

PHP:  implode(",", $items);
来源：http://twk.jyoumei.cn

JS:   items.join(",")
来源：http://lbh.xylfe.cn

TS:   items.join(",")
来源：http://niw.cucudq.cn

Java: String.join(",", items)
来源：http://bzl.hammf.cn

Go:   strings.Join(items, ",")
来源：http://ahs.ivvv.top

Ruby: items.join(",")
来源：http://ivw.sjlbkw.cn

C#:   string.Join(",", items)
来源：http://utl.52xcode.cn

[E09] 去除所有空白字符
来源：http://utv.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bgk.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://whe.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ttq.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://kli.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://nek.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://ivl.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hel.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qzd.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://efp.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qny.vqdsnc.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vgg.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://eyu.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://srj.yonumen.top

Java: String.format("%03d", 7)
来源：http://agg.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://iyq.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nsu.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://azy.gzhubu.top

[E11] 反转字符串
来源：http://gwl.hfpthk.cn

Py:   s[::-1]
来源：http://tyo.9152youxi.cn

PHP:  strrev($s);
来源：http://qni.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://fko.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://fgy.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cly.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://amh.cucudq.cn

Ruby: s.reverse
来源：http://aje.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://gcv.redwolf501.top

[E12] 统计某字符出现次数
来源：http://bhz.jinqigufen.top

Py:   s.count("a")
来源：http://zcm.uphjek.com

PHP:  substr_count($s, "a");
来源：http://usv.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://wik.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://dur.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jzh.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://ugo.shuidangran.top

Ruby: s.count("a")
来源：http://kjr.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://mun.aizwys.cn

[E13] 逐字符遍历
来源：http://yew.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://hli.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ezq.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://obl.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xyk.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://niu.zhoulong.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xjb.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mcb.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ojg.havefunace.top

[E14] URL 编码与 Base64
来源：http://uoa.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jpo.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kjf.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://udd.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zba.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qdw.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ezi.zhixingplan.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wfu.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://byg.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://ojb.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://rsj.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iww.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cbc.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fuy.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zao.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ohj.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://geh.ydjk.org.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ooy.shanyushiyangtech.top

[E16] 数字千分位
来源：http://nup.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://eug.yuanzhike.top

PHP:  number_format(1234567);
来源：http://qwk.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://frm.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wkv.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tjz.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jtg.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zdp.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://qlj.ydzc1.top

[E17] 首字母大写
来源：http://rwm.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mhd.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://spw.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikl.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqj.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vig.ivvv.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xoo.guowangkeji.top

Ruby: s.capitalize
来源：http://tlm.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ybc.shzxlz.cn

[E18] 模板占位符替换
来源：http://sed.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://epg.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dvj.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sdr.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://clj.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xuf.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nlc.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fsg.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gsh.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://mgj.kuanghao11.cn

Py:   s.splitlines()
来源：http://atb.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://myj.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://ilp.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://fwx.tanke756.top

Java: s.lines().toList()
来源：http://ukn.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://gcs.yj20258888.top

Ruby: s.lines
来源：http://iki.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://kgj.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://dld.zycfv.cn

Py:   if not s:
来源：http://xjt.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sqa.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gww.fengsongda.top

TS:   if (s === "") {}
来源：http://gcg.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://eml.nwbrower.top

Go:   if s == "" {}
来源：http://rss.yj20258.top

Ruby: if s.empty?
来源：http://wkc.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://clk.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://xgl.guowangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qfk.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iva.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oje.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cmc.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://god.chenzaomai.com

Go:   // 按 rune 判断长度后截断
来源：http://qwu.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iuh.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fxm.vehdjk.com

[E22] 字节长度与字符长度
来源：http://ach.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://igz.zycfv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sps.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://trq.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zce.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zxi.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://myi.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://hvc.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ooi.hesvh.cn

================================================================================
来源：http://fxp.fktsv.cn

F. 文件与目录
来源：http://zay.svipenyu.cn

================================================================================
来源：http://sbb.kuanghao11.cn

[F01] 读取整个文件
来源：http://lwb.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ntu.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://ocs.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rjn.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yjt.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://kdw.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iat.hcnkem.com

Ruby: File.read("a.txt")
来源：http://sia.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://iub.quarkkingdee.top

[F02] 逐行读取文件
来源：http://znh.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uih.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tmb.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lya.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fkv.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hcu.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rtf.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://svu.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://obm.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://efp.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ehu.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rdi.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqt.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ggr.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ock.xylfe.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zmn.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://ljg.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kgs.sweek.top

[F04] 追加写入文件
来源：http://lcl.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oql.xuanzx.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uer.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqf.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://com.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yzq.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lho.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://akk.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ubb.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://jlu.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nbc.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://elr.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://myl.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://slb.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gix.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yha.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://lxn.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://uwi.ydzc1.top

[F06] 删除文件
来源：http://kwu.wangdashe.top

Py:   os.remove("a.txt")
来源：http://hte.bjfxy.top

PHP:  unlink("a.txt");
来源：http://ebe.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://ebi.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ulg.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://swo.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://ovv.uphjek.com

Ruby: File.delete("a.txt")
来源：http://ans.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://gja.smart0.xyz

[F07] 创建目录（含多级）
来源：http://oxb.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eay.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uie.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://env.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nry.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dvz.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://thq.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eqn.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tpr.yj20258888.top

[F08] 遍历目录
来源：http://shg.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sqn.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://avh.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://lsc.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://lgr.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wlm.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uku.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://huz.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://llv.jyoumei.cn

[F09] 获取文件大小
来源：http://utv.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://uuy.yj202588.top

PHP:  filesize("a.txt");
来源：http://grz.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://hmc.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://ahb.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://coj.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bbk.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://nbm.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://vde.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://fdr.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aui.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gpu.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://stc.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://xtb.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hiv.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lku.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ine.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hwl.chenzaomai.com

[F11] 复制与移动文件
来源：http://iib.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qhd.dianchejie.cn


<!-- 参考信息 -->