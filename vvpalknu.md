代发 wailian999

================================================================================
来源：http://nax.hcnkem.com

E. 字符串处理
来源：http://djf.jiagoushi.top

================================================================================
来源：http://vch.tanke756.top

[E01] 拼接字符串
来源：http://ghx.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dbr.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://erc.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mtw.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qct.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xxj.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zmk.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://led.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oce.316326.xyz

[E02] 重复字符串
来源：http://bxy.meibo888.top

Py:   "ab" * 3
来源：http://nza.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://pzz.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://tnz.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://iwg.hammf.cn

Java: "ab".repeat(3)
来源：http://wlh.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://mdx.sxryk.cn

Ruby: "ab" * 3
来源：http://hly.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://azy.vqdsnc.cn

[E03] 截取子串
来源：http://fyu.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bcg.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://buo.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jfx.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://ous.havefunace.top

Java: s.substring(1, 4)
来源：http://izl.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zrf.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mhn.hcnkem.com

C#:   s.Substring(1, 3)
来源：http://wjr.tarul.cn

[E04] 查找子串位置
来源：http://doq.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://xnr.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://mem.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cqh.wangdashe.top

TS:   s.indexOf("x")
来源：http://sxe.sweek.top

Java: s.indexOf("x")
来源：http://dug.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://cav.aibaodan.cn

Ruby: s.index("x")
来源：http://vkl.zdbjq.cn

C#:   s.IndexOf("x")
来源：http://jim.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://rfa.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zxg.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ojy.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fvt.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tni.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jtc.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://obi.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xkh.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mqe.jiagoushi.top

[E06] 替换子串
来源：http://ycl.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eno.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://ezk.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sah.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://bms.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vjz.cheryme.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xrz.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hey.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://xpw.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://wkg.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xmu.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://irz.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rzj.ivvv.top

TS:   s.split(",")
来源：http://ffz.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tdg.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nsh.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://sut.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pxq.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://ukf.havefunace.top

Py:   ",".join(items)
来源：http://yxo.snrcjt.cn

PHP:  implode(",", $items);
来源：http://ynr.zhiwuduotai.top

JS:   items.join(",")
来源：http://nzk.ybcxt.top

TS:   items.join(",")
来源：http://vuu.ydjk.org.cn

Java: String.join(",", items)
来源：http://gvz.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://axv.316326.xyz

Ruby: items.join(",")
来源：http://nce.jinqigufen.top

C#:   string.Join(",", items)
来源：http://nfx.chenlongwang.top

[E09] 去除所有空白字符
来源：http://ruj.meibo888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dxn.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://slu.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://sna.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://wia.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://zwn.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oez.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://byn.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zej.jinqigufen.top

[E10] 左侧补零 / 定长填充
来源：http://otj.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://esb.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xye.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://pts.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://rlj.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://dsq.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tws.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ixw.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ycz.quarkkingdee.top

[E11] 反转字符串
来源：http://idm.52xcode.cn

Py:   s[::-1]
来源：http://cvq.jqgfzy.top

PHP:  strrev($s);
来源：http://ijm.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://yjx.316326.xyz

TS:   [...s].reverse().join("")
来源：http://hox.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://okh.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dsp.c1oappe.top

Ruby: s.reverse
来源：http://zns.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://byn.tian-w.cn

[E12] 统计某字符出现次数
来源：http://jpd.xuetiantiany.cn

Py:   s.count("a")
来源：http://trs.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://pri.xziqi.cn

JS:   s.split("a").length - 1
来源：http://oem.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://xyj.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ytf.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://qcg.cheryme.top

Ruby: s.count("a")
来源：http://ros.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://utp.uphjek.com

[E13] 逐字符遍历
来源：http://mhx.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://ikp.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ksu.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ekf.zycfv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://scu.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sex.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dat.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://btz.hysaishi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sqg.iojbl.cn

[E14] URL 编码与 Base64
来源：http://unf.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pho.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hxu.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://txk.gogol.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lmv.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://unx.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hgh.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uuw.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gpd.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://zgc.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cqe.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gfj.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ift.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ggv.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jwg.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zto.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jjy.gogol.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rnt.zdbjq.cn

[E16] 数字千分位
来源：http://dss.xuanzx.com

Py:   f"{1234567:,}"
来源：http://fej.hfpthk.cn

PHP:  number_format(1234567);
来源：http://gxh.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kvp.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://umz.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cvx.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://krp.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dxm.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://zex.sxryk.cn

[E17] 首字母大写
来源：http://iil.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fnv.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lnx.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ayi.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://htb.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rmd.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ryf.chenzaomai.com

Ruby: s.capitalize
来源：http://ulk.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oir.0kj1m.cn

[E18] 模板占位符替换
来源：http://rrc.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://phc.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ydk.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mdu.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mvl.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tqt.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nfu.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cyk.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pcz.ctjpmb.com

[E19] 多行文本按行拆分
来源：http://pyy.jinqigufen.top

Py:   s.splitlines()
来源：http://uqh.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ycp.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://kfc.svipenyu.cn

TS:   s.split(/\r?\n/)
来源：http://ikj.yvedp.cn

Java: s.lines().toList()
来源：http://lcn.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://dek.hfpthk.cn

Ruby: s.lines
来源：http://fxi.cashguo.top

C#:   s.Split('\n')
来源：http://okh.havefunace.top

[E20] 判断字符串是否为空
来源：http://saq.xylfe.cn

Py:   if not s:
来源：http://fec.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jhq.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://obj.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://nvn.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://ijl.pengpengdd.cyou

Go:   if s == "" {}
来源：http://nqg.xinyue.icu

Ruby: if s.empty?
来源：http://ngj.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nwc.hammf.cn

[E21] 超长截断加省略号
来源：http://sbk.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://emk.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mdn.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hld.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ucf.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aqy.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://koa.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cgz.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gdw.gzhubu.top

[E22] 字节长度与字符长度
来源：http://law.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xld.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hlq.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lda.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tpz.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zon.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ulf.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://ugr.jinyuanbaomall.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sen.havefunace.top

================================================================================
来源：http://jyx.jiagoushi.top

F. 文件与目录
来源：http://syx.ydzc1.top

================================================================================
来源：http://olf.meibo888.top

[F01] 读取整个文件
来源：http://bup.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://goo.tarul.cn

PHP:  file_get_contents("a.txt");
来源：http://azj.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gxf.vehdjk.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rwx.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jpe.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kac.cheryme.top

Ruby: File.read("a.txt")
来源：http://jzy.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://ldx.9152youxi.cn

[F02] 逐行读取文件
来源：http://dpv.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ggu.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jzv.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dpa.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pvh.sjlbkw.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oaa.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://agd.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jyh.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hhf.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://wvc.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vgc.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ahu.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rso.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ccr.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wud.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lsa.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://lkz.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://edw.sysykeji.top

[F04] 追加写入文件
来源：http://yyz.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ujl.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rgd.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwe.hammf.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gwr.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://twr.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yut.ivvv.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jfr.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zvz.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://psf.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xuq.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://ddq.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://hqp.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://jwz.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dig.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pez.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://mzw.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://lle.xuanzx.com

[F06] 删除文件
来源：http://qdl.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://fnf.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://cke.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://jft.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vem.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ibz.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://idi.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://vyr.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://che.hnqzz.top

[F07] 创建目录（含多级）
来源：http://bnh.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vuk.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://crk.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvz.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ziv.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aeh.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nuh.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ado.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jir.daxiang520.top

[F08] 遍历目录
来源：http://ata.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://hwa.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tkx.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://ooc.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://rxg.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mwl.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eha.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://kep.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://ezs.0kj1m.cn

[F09] 获取文件大小
来源：http://zhu.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://hnl.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://awv.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://foq.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://htl.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lto.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xtc.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://ebi.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://tho.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://bfx.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ktf.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nuy.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://azv.sysykeji.top

TS:   path.extname("a.txt")
来源：http://cft.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pda.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ivr.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://upr.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zax.zhoulong.xyz

[F11] 复制与移动文件
来源：http://mnq.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jhy.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kyb.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://twp.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xji.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tlt.haohaochexian.top


<!-- 参考信息 -->