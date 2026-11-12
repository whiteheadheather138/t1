代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://qyi.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://wlk.jyoumei.cn

JS:   arr.join(", ")
来源：http://vhn.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://iqx.daria6918.cn

Java: String.join(", ", list)
来源：http://qcf.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://ugi.haohaochexian.top

Ruby: arr.join(", ")
来源：http://kis.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://hkd.chenzaomai.com

================================================================================
来源：http://rzd.bjfxy.top

E. 字符串处理
来源：http://jjy.gaohongyu789.top

================================================================================
来源：http://fop.fktsv.cn

[E01] 拼接字符串
来源：http://wrt.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://epb.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ztr.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://waa.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aan.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nvv.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rpw.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://szz.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ylk.jyoumei.cn

[E02] 重复字符串
来源：http://mgz.zhoulong.xyz

Py:   "ab" * 3
来源：http://xmc.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://smr.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://ipx.ehwqpu.com

TS:   "ab".repeat(3)
来源：http://bnr.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://yxc.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://bpz.gotoacloud.top

Ruby: "ab" * 3
来源：http://vnq.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cys.sxryk.cn

[E03] 截取子串
来源：http://tvi.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kfu.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://knk.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zcv.fengsongda.top

TS:   s.slice(1, 4)
来源：http://eiu.bbcook.cn

Java: s.substring(1, 4)
来源：http://ilz.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wtd.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://xks.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://woq.smart0.xyz

[E04] 查找子串位置
来源：http://lis.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://tqx.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://wdt.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ixy.cheryme.top

TS:   s.indexOf("x")
来源：http://une.yj20258.top

Java: s.indexOf("x")
来源：http://pun.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://ztq.yvedp.cn

Ruby: s.index("x")
来源：http://vco.birdmap.top

C#:   s.IndexOf("x")
来源：http://oee.dashuyun.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gue.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://trf.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://usj.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zht.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://llu.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xne.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://niy.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fad.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://atd.yangfankeji.com

[E06] 替换子串
来源：http://ule.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fqt.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://geo.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bew.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://uzv.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yvk.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nif.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://peu.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://leg.yuanzhike.top

[E07] 按分隔符拆分
来源：http://qab.sweek.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wru.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://scl.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://glx.ybcxt.top

TS:   s.split(",")
来源：http://ogj.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://bjc.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jpi.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://znz.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pna.hcnkem.com

[E08] 数组按分隔符合并
来源：http://mpw.52xcode.cn

Py:   ",".join(items)
来源：http://yeo.tarul.cn

PHP:  implode(",", $items);
来源：http://egp.xinyue.icu

JS:   items.join(",")
来源：http://dnx.xinyue.icu

TS:   items.join(",")
来源：http://qwz.hongshengwenyu.top

Java: String.join(",", items)
来源：http://gov.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://ajd.mhx1999.top

Ruby: items.join(",")
来源：http://ssv.smart0.xyz

C#:   string.Join(",", items)
来源：http://ugj.aibaodan.cn

[E09] 去除所有空白字符
来源：http://pyz.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aof.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zcg.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://lee.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://xca.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://psl.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tzv.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://udv.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eco.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://zyk.jinqigfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vgp.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ibr.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://swt.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://pnl.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://fwa.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ifo.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rro.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://reo.nanxinkj.top

[E11] 反转字符串
来源：http://dvy.jinqigfzy.top

Py:   s[::-1]
来源：http://mxr.pengpengdd.cyou

PHP:  strrev($s);
来源：http://utw.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://jkx.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://lms.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ofp.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hwy.hnqzz.top

Ruby: s.reverse
来源：http://gvp.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://cne.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://mem.dianchejie.cn

Py:   s.count("a")
来源：http://vty.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://bte.yueranfly.top

JS:   s.split("a").length - 1
来源：http://ere.smart0.xyz

TS:   s.split("a").length - 1
来源：http://rcg.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xcl.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://ivs.shzxlz.cn

Ruby: s.count("a")
来源：http://kir.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://grf.shanyushiyangtech.top

[E13] 逐字符遍历
来源：http://hgn.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://xup.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ruz.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qnl.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ghk.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sef.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qtj.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iju.wangdashe.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hki.iojbl.cn

[E14] URL 编码与 Base64
来源：http://uta.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hqr.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zic.fanxiaobao.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://svb.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mzu.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kvl.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yko.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tts.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xkq.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://nqa.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://klo.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xbr.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xfl.jinyuanbaomall.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vyz.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cyn.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://apf.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zkx.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yvb.chenzaomai.com

[E16] 数字千分位
来源：http://amb.cheryme.top

Py:   f"{1234567:,}"
来源：http://qme.hammf.cn

PHP:  number_format(1234567);
来源：http://lla.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bbh.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://kyn.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qto.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jif.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bdn.yongpay.top

C#:   1234567.ToString("N0")
来源：http://tje.fzhhl.top

[E17] 首字母大写
来源：http://sjh.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eoe.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://myf.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vdv.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://apt.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cnw.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zoj.yonumen.top

Ruby: s.capitalize
来源：http://ijw.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rkp.chenjidiqi.icu

[E18] 模板占位符替换
来源：http://ipz.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://php.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qqy.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dya.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cdz.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rbg.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xfk.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rfj.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hhb.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://vxi.ehwqpu.com

Py:   s.splitlines()
来源：http://thy.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pde.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://ikj.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://jkp.tian-w.cn

Java: s.lines().toList()
来源：http://ixf.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://fqn.jianghu66.top

Ruby: s.lines
来源：http://fdc.dianchejie.cn

C#:   s.Split('\n')
来源：http://jox.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://nti.yonumen.top

Py:   if not s:
来源：http://zsd.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zat.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kta.shzxlz.cn

TS:   if (s === "") {}
来源：http://ash.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://hyz.yuanzhike.top

Go:   if s == "" {}
来源：http://mdh.gzhubu.top

Ruby: if s.empty?
来源：http://xej.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zab.yuxming.cn

[E21] 超长截断加省略号
来源：http://way.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uzi.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bsc.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fop.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zml.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lrp.fehbvm.com

Go:   // 按 rune 判断长度后截断
来源：http://ycp.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kzd.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tci.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://oun.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fab.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rlj.kuanghao11.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yee.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sxw.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ewi.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rma.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://fkx.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lau.hnqzz.top

================================================================================
来源：http://fez.bjfxy.top

F. 文件与目录
来源：http://dsv.hesvh.cn

================================================================================
来源：http://xqv.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://kut.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ypt.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://snr.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xkx.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hjb.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://eys.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wvw.c1oappe.top

Ruby: File.read("a.txt")
来源：http://wgf.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://eqw.vehdjk.com

[F02] 逐行读取文件
来源：http://kzf.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jnr.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yqw.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uos.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ejq.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kaz.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://orf.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rti.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yda.yj202588.top

[F03] 写入文件（覆盖）
来源：http://afm.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kws.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://txb.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sfn.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://emz.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://imf.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fgq.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://ydf.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jyl.yuanzhike.top

[F04] 追加写入文件
来源：http://xzk.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kzc.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xkl.hesvh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lvz.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hnp.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ind.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mxm.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cjo.yj202588.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pep.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://zwb.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xwk.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://aaw.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://syp.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://lyy.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dsl.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cbb.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://bxe.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://bzj.c1oappe.top

[F06] 删除文件
来源：http://zwi.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://vis.wangdashe.top

PHP:  unlink("a.txt");
来源：http://khr.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://arp.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kxe.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yaj.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://dni.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://arh.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://gdt.xziqi.cn

[F07] 创建目录（含多级）
来源：http://dqt.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jbs.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ssq.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hao.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fye.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyv.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://inq.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://svo.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://csf.zycfv.cn

[F08] 遍历目录
来源：http://jxr.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vxc.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tnu.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://gza.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://dgb.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tts.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rzu.daria6918.cn

Ruby: Dir.children("dir")
来源：http://ojp.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://qzk.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://yda.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://vkf.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://oin.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://fmh.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://djr.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://dgb.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://foy.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://tdi.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://bap.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://tfp.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sqw.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nyk.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nsc.bbcook.cn

TS:   path.extname("a.txt")
来源：http://sdd.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://krr.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uaa.gogol.net.cn


<!-- 参考信息 -->