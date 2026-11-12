代发 wailian999

================================================================================
来源：http://ybu.cucudq.cn

E. 字符串处理
来源：http://bvn.svipenyu.cn

================================================================================
来源：http://mrp.zhengqikj.top

[E01] 拼接字符串
来源：http://ynp.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fcu.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vdc.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://agu.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jye.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ggk.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ufo.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wmd.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vzj.iojbl.cn

[E02] 重复字符串
来源：http://fge.birdmap.top

Py:   "ab" * 3
来源：http://exm.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://egi.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://tjk.vqdsnc.cn

TS:   "ab".repeat(3)
来源：http://ilf.sufxvd.cn

Java: "ab".repeat(3)
来源：http://dgl.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://umo.epnwcf.com

Ruby: "ab" * 3
来源：http://gfz.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://djx.zdqjudy.top

[E03] 截取子串
来源：http://yrr.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://epf.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://edb.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hzt.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://vql.cashguo.top

Java: s.substring(1, 4)
来源：http://vjd.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ofu.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jdx.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://qht.yanxiufei.cn

[E04] 查找子串位置
来源：http://xsd.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://mjk.hnqzz.top

PHP:  strpos($s, "x");
来源：http://gqc.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xox.fzhhl.top

TS:   s.indexOf("x")
来源：http://ley.guannengcc.top

Java: s.indexOf("x")
来源：http://dwh.yj20258.top

Go:   strings.Index(s, "x")
来源：http://eba.yfazqb.com

Ruby: s.index("x")
来源：http://myx.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://vio.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qkc.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ttz.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://thp.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hrk.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tbg.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rel.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qsm.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vkg.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iwq.zhiwuduotai.top

[E06] 替换子串
来源：http://vhl.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vjc.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://pzz.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhc.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://vas.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uql.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dty.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lkv.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://twf.zdqjudy.top

[E07] 按分隔符拆分
来源：http://fdk.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hnb.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rpf.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://upz.bbcook.cn

TS:   s.split(",")
来源：http://qho.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://itx.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xpt.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://yky.aizwys.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ciu.havefunace.top

[E08] 数组按分隔符合并
来源：http://cmi.dianchejie.cn

Py:   ",".join(items)
来源：http://tlw.smart0.xyz

PHP:  implode(",", $items);
来源：http://hpz.gogol.net.cn

JS:   items.join(",")
来源：http://evv.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://ahe.hnxiangtu.top

Java: String.join(",", items)
来源：http://xdt.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://qyq.kuanghao11.cn

Ruby: items.join(",")
来源：http://dbm.guannengcc.top

C#:   string.Join(",", items)
来源：http://ksv.birdmap.top

[E09] 去除所有空白字符
来源：http://hww.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ynp.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ycn.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://hlw.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://yqj.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://nne.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zzl.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gxy.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lpr.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://gze.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ebm.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gxx.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://ubj.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://son.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://vbn.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ngp.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vwn.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yqg.zycfv.cn

[E11] 反转字符串
来源：http://rwf.zhoulong.xyz

Py:   s[::-1]
来源：http://yfc.kuanghao11.cn

PHP:  strrev($s);
来源：http://cok.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://kvf.nanxinkj.top

TS:   [...s].reverse().join("")
来源：http://vfc.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://kdz.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zxe.cucudq.cn

Ruby: s.reverse
来源：http://wog.kuanghao11.cn

C#:   new string(s.Reverse().ToArray())
来源：http://drm.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://hva.cdnleiting.top

Py:   s.count("a")
来源：http://hqr.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://yip.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://han.mhx1999.top

TS:   s.split("a").length - 1
来源：http://imf.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vsz.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://tei.aizwys.cn

Ruby: s.count("a")
来源：http://rqs.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://wtm.smart0.xyz

[E13] 逐字符遍历
来源：http://tdw.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://dcn.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lpn.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lmv.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://jwi.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggt.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aye.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://foi.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hyh.smart0.xyz

[E14] URL 编码与 Base64
来源：http://fgg.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yhu.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gxn.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tho.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uog.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mpk.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jkn.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xqh.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://owa.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://mir.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://emy.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dyh.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://saf.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tbd.ctjpmb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sdk.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mjv.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jvh.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://idh.ydzc1.top

[E16] 数字千分位
来源：http://okd.vehdjk.com

Py:   f"{1234567:,}"
来源：http://kba.nanxinkj.top

PHP:  number_format(1234567);
来源：http://zbr.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wyd.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ksw.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lzk.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rxo.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wuu.pengpengdd.cyou

C#:   1234567.ToString("N0")
来源：http://gow.yvedp.cn

[E17] 首字母大写
来源：http://jsf.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://asn.jyoumei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ero.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cnn.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yvk.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jib.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cph.daria6918.cn

Ruby: s.capitalize
来源：http://jvg.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://acf.xuanzx.com

[E18] 模板占位符替换
来源：http://pqf.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vsq.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rmk.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zfq.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pgv.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kwy.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://viq.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mwd.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gqj.cashguo.top

[E19] 多行文本按行拆分
来源：http://ruv.gzhubu.top

Py:   s.splitlines()
来源：http://jjt.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ren.hywenlv.cn

JS:   s.split(/\r?\n/)
来源：http://zui.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://aqh.ehwqpu.com

Java: s.lines().toList()
来源：http://onl.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://ejw.yonumen.top

Ruby: s.lines
来源：http://qzb.yanxiufei.cn

C#:   s.Split('\n')
来源：http://sjl.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://rat.redwolf501.top

Py:   if not s:
来源：http://tiq.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://koo.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hse.jlsjyb.cn

TS:   if (s === "") {}
来源：http://dsl.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://gur.shzxlz.cn

Go:   if s == "" {}
来源：http://txw.epnwcf.com

Ruby: if s.empty?
来源：http://xae.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aem.tianlin.xyz

[E21] 超长截断加省略号
来源：http://zbo.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jgg.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://laq.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqy.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fka.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xxr.vqdsnc.cn

Go:   // 按 rune 判断长度后截断
来源：http://cpl.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hwu.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivc.shuidangran.top

[E22] 字节长度与字符长度
来源：http://zzy.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sjn.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wxa.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://opd.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yyg.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mag.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qnq.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://fat.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wdf.ywan-chungtsiang.top

================================================================================
来源：http://kwr.xuetiantiany.cn

F. 文件与目录
来源：http://qwq.sysykeji.top

================================================================================
来源：http://kaz.pengpengdd.cyou

[F01] 读取整个文件
来源：http://tlq.yfazqb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nnh.zhengqikj.top

PHP:  file_get_contents("a.txt");
来源：http://urx.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cgg.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zdi.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://brn.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hze.nwbrower.top

Ruby: File.read("a.txt")
来源：http://mmt.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://rny.yj20258.top

[F02] 逐行读取文件
来源：http://mwr.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wyl.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hyq.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gua.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eef.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lvj.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rsh.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hkw.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://clh.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://hte.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ajk.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://nge.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fkv.wangdashe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tbe.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ijp.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cfv.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://ziq.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyb.shuidangran.top

[F04] 追加写入文件
来源：http://kcx.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ysd.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qzk.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fhf.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fmj.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ceg.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wyn.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gls.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zwb.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://gwo.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ifh.ivvv.top

PHP:  file_exists("a.txt");
来源：http://gxv.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://fyy.jinghuilouyu.cn

TS:   fs.existsSync("a.txt")
来源：http://yvs.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://adi.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sbp.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://mrr.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://fop.aibaodan.cn

[F06] 删除文件
来源：http://eeh.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://mar.52xcode.cn

PHP:  unlink("a.txt");
来源：http://nmi.tian-w.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ybc.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kvs.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hop.shanyushiyangkeji.top

Go:   os.Remove("a.txt")
来源：http://vsc.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://qhc.yj202588.top

C#:   File.Delete("a.txt");
来源：http://fkj.xziqi.cn

[F07] 创建目录（含多级）
来源：http://yka.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rsv.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zmq.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pnp.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gys.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yqv.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rxt.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uoz.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xqf.hesvh.cn

[F08] 遍历目录
来源：http://yye.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wux.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kxz.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://vub.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://rhn.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://esa.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uop.hesvh.cn

Ruby: Dir.children("dir")
来源：http://gko.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://qpq.nanxuanxn.top

[F09] 获取文件大小
来源：http://xsl.xylfe.cn

Py:   os.path.getsize("a.txt")
来源：http://img.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://emu.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://chm.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://mnk.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://jcz.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rcr.bbcook.cn

Ruby: File.size("a.txt")
来源：http://rop.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://mho.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://zdn.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zzc.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://usu.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nem.epnwcf.com

TS:   path.extname("a.txt")
来源：http://cut.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rlx.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ood.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kiu.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jwf.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://rva.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rij.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fuf.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xcj.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yrq.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gfy.sysykeji.top


<!-- 参考信息 -->