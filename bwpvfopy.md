代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://ekq.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://wcx.ydzc1.top

JS:   arr.join(", ")
来源：http://iqx.tian-w.cn

TS:   arr.join(", ")
来源：http://yeq.quarkkingdee.top

Java: String.join(", ", list)
来源：http://uel.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://sqe.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://xan.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://rwc.hammf.cn

================================================================================
来源：http://wqo.hnqzz.top

E. 字符串处理
来源：http://zzo.sxryk.cn

================================================================================
来源：http://xvd.zhongyouzk.top

[E01] 拼接字符串
来源：http://gup.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://loh.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jfw.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ybg.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hpq.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://psp.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://srj.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ypw.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ocr.cashguo.top

[E02] 重复字符串
来源：http://tgr.guowangkeji.top

Py:   "ab" * 3
来源：http://veu.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://qxu.ydzc1.top

JS:   "ab".repeat(3)
来源：http://weo.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://xcy.316326.xyz

Java: "ab".repeat(3)
来源：http://tij.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://sfc.hesvh.cn

Ruby: "ab" * 3
来源：http://uzs.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://txh.zhixingplan.top

[E03] 截取子串
来源：http://cgc.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gli.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wvs.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hty.vehdjk.com

TS:   s.slice(1, 4)
来源：http://urq.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://bsp.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fhf.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://bua.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://wpk.zycfv.cn

[E04] 查找子串位置
来源：http://bgj.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://bow.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://ovx.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://axj.ydzc1.top

TS:   s.indexOf("x")
来源：http://dij.ydzc1.top

Java: s.indexOf("x")
来源：http://nhb.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://shb.yanxiufei.cn

Ruby: s.index("x")
来源：http://rtc.guannengcc.top

C#:   s.IndexOf("x")
来源：http://etc.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fql.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gbc.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ouy.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://llp.vqdsnc.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vkg.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfh.xziqi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nnf.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://byk.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qyj.fanxiaobao.xyz

[E06] 替换子串
来源：http://mss.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eqt.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://frr.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://goh.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://frs.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://msx.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fqp.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cmu.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://lgi.svipenyu.cn

[E07] 按分隔符拆分
来源：http://lho.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sqk.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wyl.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://qqv.aibaodan.cn

TS:   s.split(",")
来源：http://xww.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jhg.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://brw.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://duo.sjlbkw.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dgo.yonumen.top

[E08] 数组按分隔符合并
来源：http://wcy.fzhhl.top

Py:   ",".join(items)
来源：http://mtp.sweek.top

PHP:  implode(",", $items);
来源：http://jrm.fzhhl.top

JS:   items.join(",")
来源：http://ima.zhixingplan.top

TS:   items.join(",")
来源：http://ott.tianlin.xyz

Java: String.join(",", items)
来源：http://ewh.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://tlo.gogol.net.cn

Ruby: items.join(",")
来源：http://vjo.uphjek.com

C#:   string.Join(",", items)
来源：http://rhc.bbcook.cn

[E09] 去除所有空白字符
来源：http://ggk.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cfu.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lhe.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://xqj.zdqjudy.top

TS:   s.replace(/\s+/g, "")
来源：http://khf.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://aqr.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://scy.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://awh.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ubq.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://wyn.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ohx.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vrn.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://aqc.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://csb.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://zqn.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qsh.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://izw.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mer.fzhhl.top

[E11] 反转字符串
来源：http://bff.yj20258888.top

Py:   s[::-1]
来源：http://eji.nanxuanxn.top

PHP:  strrev($s);
来源：http://rns.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://tze.pycfn.com

TS:   [...s].reverse().join("")
来源：http://rbg.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lbr.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://emp.gotoacloud.top

Ruby: s.reverse
来源：http://ddx.zhijiandao.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tpr.tarul.cn

[E12] 统计某字符出现次数
来源：http://lzm.hywenlv.cn

Py:   s.count("a")
来源：http://iqs.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://ivb.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://wfh.cqqwz.cn

TS:   s.split("a").length - 1
来源：http://prz.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xxx.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://ste.fzhhl.top

Ruby: s.count("a")
来源：http://zwk.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://eto.xziqi.cn

[E13] 逐字符遍历
来源：http://cpr.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://tkg.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://okc.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://lea.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mrh.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nzt.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eog.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://txw.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lia.sysykeji.top

[E14] URL 编码与 Base64
来源：http://utc.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ocl.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zmz.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ita.pycfn.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qmy.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://czl.tianlin.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vzw.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fiz.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://okk.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://bym.jqgfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kht.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tsv.shangyingyoupin.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jml.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qpm.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zsq.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://irq.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zit.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zvj.hesvh.cn

[E16] 数字千分位
来源：http://yoy.xuanzx.com

Py:   f"{1234567:,}"
来源：http://yyf.hammf.cn

PHP:  number_format(1234567);
来源：http://fyn.sufxvd.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://khj.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cgl.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ptr.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://osn.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://svv.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://ifk.xinyue.icu

[E17] 首字母大写
来源：http://ujb.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dah.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihl.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykg.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://czo.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://day.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yht.fengsongda.top

Ruby: s.capitalize
来源：http://uzw.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mqi.bjfxy.top

[E18] 模板占位符替换
来源：http://mik.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://afu.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rep.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dze.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uxw.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://btc.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lws.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hgs.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vpe.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://ncw.feifeiyinyue.top

Py:   s.splitlines()
来源：http://sgt.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jon.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://kyx.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://uwk.jyoumei.cn

Java: s.lines().toList()
来源：http://lua.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://ljp.havefunace.top

Ruby: s.lines
来源：http://dqb.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://qrj.yj202588.top

[E20] 判断字符串是否为空
来源：http://zfx.ybcxt.top

Py:   if not s:
来源：http://qim.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://paf.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://trz.tianlin.xyz

TS:   if (s === "") {}
来源：http://ycm.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://vho.sufxvd.cn

Go:   if s == "" {}
来源：http://gqw.fehbvm.com

Ruby: if s.empty?
来源：http://erp.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ary.jiagoushi.top

[E21] 超长截断加省略号
来源：http://add.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ont.nanxinkj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yur.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxf.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzd.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zvh.smart0.xyz

Go:   // 按 rune 判断长度后截断
来源：http://syt.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ege.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ihq.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://xxu.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ofw.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sax.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ctu.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pul.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://daf.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baa.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://hja.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cjx.yanxiufei.cn

================================================================================
来源：http://apx.birdmap.top

F. 文件与目录
来源：http://zkp.hnxiangtu.top

================================================================================
来源：http://szg.jiagoushi.top

[F01] 读取整个文件
来源：http://uuo.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hoa.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://naj.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tle.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jst.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pco.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://psv.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://qce.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://nsn.tian-w.cn

[F02] 逐行读取文件
来源：http://iru.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://crf.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vwm.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpu.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxj.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://apg.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://daf.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://agn.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qeg.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://pub.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnf.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://apk.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fhl.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cjx.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ehj.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ipz.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://qtl.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jdh.shzxlz.cn

[F04] 追加写入文件
来源：http://hll.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kat.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zcs.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imv.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ciy.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lwg.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rtl.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pwo.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://del.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://wbc.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qti.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://oyr.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://mjp.fktsv.cn

TS:   fs.existsSync("a.txt")
来源：http://bco.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yem.quarkkingdee.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mwn.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://hki.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://hjz.hongshengwenyu.top

[F06] 删除文件
来源：http://ulu.ivvv.top

Py:   os.remove("a.txt")
来源：http://kmv.yueranfly.top

PHP:  unlink("a.txt");
来源：http://txd.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://dzt.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://rel.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dja.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://aen.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://ksh.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://mdf.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://tzy.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cwv.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ysu.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wli.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qne.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rpz.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hii.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://exg.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gyz.cucudq.cn

[F08] 遍历目录
来源：http://eyq.mhx1999.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://quf.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://izt.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://nfw.yangfankeji.com

TS:   fs.readdirSync("dir")
来源：http://ouy.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tyr.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zze.bbcook.cn

Ruby: Dir.children("dir")
来源：http://rpw.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://xxm.sweek.top

[F09] 获取文件大小
来源：http://ota.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://yzu.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://efp.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://hlg.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://oii.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://lmh.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dzm.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://whl.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://nnd.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://zwa.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://brl.nwbrower.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kta.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://taf.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://vrg.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sir.chenlongwang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rbq.cdnleiting.top


<!-- 参考信息 -->