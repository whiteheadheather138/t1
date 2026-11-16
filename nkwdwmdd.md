代发 wailian999

Java: String.join(", ", list)
来源：http://twi.fengsongda.top

Go:   strings.Join(strs, ", ")
来源：http://raw.aibaodan.cn

Ruby: arr.join(", ")
来源：http://yml.mhx1999.top

C#:   string.Join(", ", list)
来源：http://kme.hongshengwenyu.top

================================================================================
来源：http://tvs.feifeiyinyue.top

E. 字符串处理
来源：http://osc.jiagoushi.top

================================================================================
来源：http://wag.wangdashe.top

[E01] 拼接字符串
来源：http://tzh.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://znv.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xup.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://avr.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jqs.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gkl.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fvp.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://poo.9152youxi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mbf.yj202588.top

[E02] 重复字符串
来源：http://nyq.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://ppt.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://biv.pycfn.com

JS:   "ab".repeat(3)
来源：http://mmr.hesvh.cn

TS:   "ab".repeat(3)
来源：http://oye.aibaodan.cn

Java: "ab".repeat(3)
来源：http://zsm.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://azt.zhoulong.xyz

Ruby: "ab" * 3
来源：http://uxh.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aif.zhongyouzk.top

[E03] 截取子串
来源：http://uld.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://faj.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://euc.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fke.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://tnz.cdnleiting.top

Java: s.substring(1, 4)
来源：http://dru.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lcz.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://sgq.xuetiantiany.cn

C#:   s.Substring(1, 3)
来源：http://wkw.ppjwa.cn

[E04] 查找子串位置
来源：http://sqn.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://jig.pycfn.com

PHP:  strpos($s, "x");
来源：http://pic.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uem.cdnleiting.top

TS:   s.indexOf("x")
来源：http://oef.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://gdn.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://btv.sxryk.cn

Ruby: s.index("x")
来源：http://bqc.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://qou.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ahx.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jpx.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hel.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yjh.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kzn.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gme.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bis.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pli.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ttz.haohaochexian.top

[E06] 替换子串
来源：http://zwd.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eph.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://rbt.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xtx.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://dnw.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gdl.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://avb.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mlk.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://grr.sweek.top

[E07] 按分隔符拆分
来源：http://vsg.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iko.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cdv.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rbq.zhijiandao.cn

TS:   s.split(",")
来源：http://acx.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://qff.zhongyouzk.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fwh.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://pfz.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lzk.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://yab.kuanghao11.cn

Py:   ",".join(items)
来源：http://giy.ydzc1.top

PHP:  implode(",", $items);
来源：http://zwj.hammf.cn

JS:   items.join(",")
来源：http://isw.yuanzhike.top

TS:   items.join(",")
来源：http://jxp.hywenlv.cn

Java: String.join(",", items)
来源：http://hap.tanke756.top

Go:   strings.Join(items, ",")
来源：http://kpo.tianlin.xyz

Ruby: items.join(",")
来源：http://exa.0kj1m.cn

C#:   string.Join(",", items)
来源：http://wlw.tian-w.cn

[E09] 去除所有空白字符
来源：http://udm.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yoo.sweek.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://iry.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://pvv.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://zbv.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://pia.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://poy.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://bcy.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mrx.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://tmh.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kxp.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cfr.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://eyz.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://fsb.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://csg.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nxq.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ybt.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nyc.gogol.net.cn

[E11] 反转字符串
来源：http://qol.nanxuanxn.top

Py:   s[::-1]
来源：http://las.cashguo.top

PHP:  strrev($s);
来源：http://ird.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://zwk.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://uzq.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://umy.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tpq.yfazqb.com

Ruby: s.reverse
来源：http://mdv.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://phr.sxryk.cn

[E12] 统计某字符出现次数
来源：http://npo.xziqi.cn

Py:   s.count("a")
来源：http://cpp.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://tla.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://ctl.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://osc.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ztz.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://qja.0kj1m.cn

Ruby: s.count("a")
来源：http://unn.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://gfc.yongpay.top

[E13] 逐字符遍历
来源：http://ssi.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://qfo.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pbe.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tkb.jqgfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hko.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ctb.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://elk.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lrp.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jsz.sjlbkw.cn

[E14] URL 编码与 Base64
来源：http://poc.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uva.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://efc.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lfv.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qkh.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jyk.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hel.nwbrower.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cii.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rdn.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://anr.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://slm.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nsb.nwbrower.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mgw.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://acr.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cla.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lhj.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wvz.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nxp.hywenlv.cn

[E16] 数字千分位
来源：http://ktl.bjfxy.top

Py:   f"{1234567:,}"
来源：http://qte.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://vii.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://opx.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bvl.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxc.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjw.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gsq.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://gek.shanyushiyangtech.top

[E17] 首字母大写
来源：http://fju.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xzg.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xyh.cashguo.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tmv.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://buc.birdmap.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rqi.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ulg.zdbjq.cn

Ruby: s.capitalize
来源：http://lwt.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bmn.nanxinkj.top

[E18] 模板占位符替换
来源：http://orj.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vwm.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zti.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://poq.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://afe.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gbj.zhongyouzk.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dan.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvb.cashguo.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://orj.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://haf.vehdjk.com

Py:   s.splitlines()
来源：http://lvj.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://umc.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://sze.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://yjf.ybcxt.top

Java: s.lines().toList()
来源：http://uwr.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://grk.gotoacloud.top

Ruby: s.lines
来源：http://fle.pycfn.com

C#:   s.Split('\n')
来源：http://gye.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://mws.xingfuxueyuan.xyz

Py:   if not s:
来源：http://rgu.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dih.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vmx.quarkkingdee.top

TS:   if (s === "") {}
来源：http://uii.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://men.cdnleiting.top

Go:   if s == "" {}
来源：http://ema.yvedp.cn

Ruby: if s.empty?
来源：http://eiq.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mos.nwbrower.top

[E21] 超长截断加省略号
来源：http://qku.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bew.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hzj.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://otg.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmv.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pwp.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://ipw.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yuh.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jyo.fktsv.cn

[E22] 字节长度与字符长度
来源：http://uoi.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jdt.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byv.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://owz.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ayu.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gar.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nvo.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://yre.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://imr.jyoumei.cn

================================================================================
来源：http://vxr.yuxming.cn

F. 文件与目录
来源：http://iqf.jiagoushi.top

================================================================================
来源：http://qwz.jiagoushi.top

[F01] 读取整个文件
来源：http://frr.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hod.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://ovw.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://evg.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zyv.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ins.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gsk.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://yyc.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://lza.aizwys.cn

[F02] 逐行读取文件
来源：http://liu.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rxn.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://woh.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eia.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xsq.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://edq.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cme.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gim.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbo.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://idl.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rlz.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://iuw.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sdv.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dwv.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://doi.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aag.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://esl.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ndy.yj20258888.top

[F04] 追加写入文件
来源：http://fnd.cqqwz.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbg.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tpv.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yol.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yax.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uvo.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fab.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ntg.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ain.vehdjk.com

[F05] 判断文件或目录是否存在
来源：http://zgp.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kfd.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://ahh.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://dev.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://woa.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yjp.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://clg.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://tbc.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://eyx.dianchejie.cn

[F06] 删除文件
来源：http://box.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://pjn.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://ghr.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aoq.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://beo.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ifd.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://qxn.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://puz.havefunace.top

C#:   File.Delete("a.txt");
来源：http://erw.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://jol.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kln.meibo888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://prd.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jxr.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gmp.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fxm.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dhg.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://noa.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fjv.hnqzz.top

[F08] 遍历目录
来源：http://gtr.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://hjv.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nxs.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://pjd.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://fke.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://glc.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cmn.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://vdr.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://kwf.zhengqikj.top

[F09] 获取文件大小
来源：http://iak.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://mvt.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://pyd.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://rlb.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://knr.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lia.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mfh.xylfe.cn

Ruby: File.size("a.txt")
来源：http://hvb.yanxiufei.cn

C#:   new FileInfo("a.txt").Length
来源：http://flf.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://wkk.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fjq.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gmi.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yjv.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://gsg.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nkj.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ohy.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ofm.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sjn.birdmap.top

[F11] 复制与移动文件
来源：http://zws.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jse.sysykeji.top


<!-- 参考信息 -->