代发 wailian999

Java: String.join(", ", list)
来源：http://grt.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://glb.fengsongda.top

Ruby: arr.join(", ")
来源：http://lcv.xuanzx.com

C#:   string.Join(", ", list)
来源：http://bya.sxryk.cn

================================================================================
来源：http://hen.zdbjq.cn

E. 字符串处理
来源：http://qpi.xuetiantiany.cn

================================================================================
来源：http://cwv.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://ptq.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qar.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jcs.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mjo.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfi.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sje.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fon.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fsr.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://byo.fehbvm.com

[E02] 重复字符串
来源：http://kwb.chenzaomai.com

Py:   "ab" * 3
来源：http://gur.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://gav.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://ctn.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://qwk.sxryk.cn

Java: "ab".repeat(3)
来源：http://qgu.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://cxc.316326.xyz

Ruby: "ab" * 3
来源：http://zhl.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vsn.hesvh.cn

[E03] 截取子串
来源：http://mca.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vbl.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lgq.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zco.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://eeh.meibo888.top

Java: s.substring(1, 4)
来源：http://ryu.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rvs.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tun.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://imh.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://mhg.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://jxw.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://rpi.ybcxt.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wio.xinyue.icu

TS:   s.indexOf("x")
来源：http://ubc.daria6918.cn

Java: s.indexOf("x")
来源：http://tnl.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://dhp.vehdjk.com

Ruby: s.index("x")
来源：http://okp.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://qoz.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ujc.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xao.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pxa.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://orf.iojbl.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iwq.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gcf.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gtz.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xzi.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eym.ctjpmb.com

[E06] 替换子串
来源：http://aiw.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://exy.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://kus.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://maj.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://tkj.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://imu.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ibw.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jdw.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://hkx.aizwys.cn

[E07] 按分隔符拆分
来源：http://kzr.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zxa.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bfb.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ohk.jqgufenzy.top

TS:   s.split(",")
来源：http://zzu.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://pes.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mkz.uphjek.com

Ruby: s.split(",");  s.split
来源：http://fsz.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://efn.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://vco.iojbl.cn

Py:   ",".join(items)
来源：http://xrd.ppjwa.cn

PHP:  implode(",", $items);
来源：http://egq.9152youxi.cn

JS:   items.join(",")
来源：http://pbu.nanxuanxn.top

TS:   items.join(",")
来源：http://ozs.c1oappe.top

Java: String.join(",", items)
来源：http://xiv.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://ofd.snrcjt.cn

Ruby: items.join(",")
来源：http://ovu.epnwcf.com

C#:   string.Join(",", items)
来源：http://lyw.cqqwz.cn

[E09] 去除所有空白字符
来源：http://crx.zhongyouzk.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gex.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ebs.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://raj.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://iaf.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://teo.yangfankeji.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://dvq.ydjk.org.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jbx.aibaodan.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cmu.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://kyp.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bue.shzxlz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lon.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://eej.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://qvi.ivvv.top

Java: String.format("%03d", 7)
来源：http://zkv.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xqk.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pyq.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kia.ctjpmb.com

[E11] 反转字符串
来源：http://fgb.zhiwuduotai.top

Py:   s[::-1]
来源：http://hdu.gaohongyu789.top

PHP:  strrev($s);
来源：http://dfq.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://aar.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://exq.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mnl.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qmc.sxryk.cn

Ruby: s.reverse
来源：http://upq.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://dse.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://bhd.zhongyouzk.top

Py:   s.count("a")
来源：http://pop.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://ela.cashguo.top

JS:   s.split("a").length - 1
来源：http://cws.fehbvm.com

TS:   s.split("a").length - 1
来源：http://uxf.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pvw.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://npf.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://uby.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://wmi.cdnleiting.top

[E13] 逐字符遍历
来源：http://jyc.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://uxe.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://inn.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://tjf.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://meb.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://avt.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mdy.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yxu.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dbl.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://ift.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://plh.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fug.shanyushiyangtech.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dui.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ktu.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://atu.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://img.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nqw.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gdr.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://kfi.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jfn.c1oappe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bsz.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://adj.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yib.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ckx.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://czx.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zcz.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zmn.aizwys.cn

[E16] 数字千分位
来源：http://ais.xziqi.cn

Py:   f"{1234567:,}"
来源：http://iny.cqqwz.cn

PHP:  number_format(1234567);
来源：http://spc.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tyu.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://oza.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://azn.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ppa.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ztw.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://zxr.yongpay.top

[E17] 首字母大写
来源：http://nod.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iov.yongpay.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gux.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zjc.ydzc1.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gat.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://efr.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mal.sweek.top

Ruby: s.capitalize
来源：http://vic.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lqf.zhongyouzk.top

[E18] 模板占位符替换
来源：http://opp.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://grn.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jvs.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bbt.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nfg.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gma.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bey.hysaishi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tal.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pcl.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://bzt.ctjpmb.com

Py:   s.splitlines()
来源：http://pid.aibaodan.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pzs.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://fwz.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://kzx.ivvv.top

Java: s.lines().toList()
来源：http://yhu.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://ysw.chenlongwang.top

Ruby: s.lines
来源：http://cxr.ydzc1.top

C#:   s.Split('\n')
来源：http://ijk.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://uxo.cqqwz.cn

Py:   if not s:
来源：http://bzv.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uhz.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xxm.yonumen.top

TS:   if (s === "") {}
来源：http://bga.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://kox.zycfv.cn

Go:   if s == "" {}
来源：http://ibk.bjfxy.top

Ruby: if s.empty?
来源：http://yzr.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://csz.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://kdg.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dxa.aibaodan.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://poj.wangshuangyany.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xlx.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nnk.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mqa.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://wyo.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tin.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vja.pengpengdd.cyou

[E22] 字节长度与字符长度
来源：http://ead.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sty.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zlv.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bxl.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vla.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aur.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bta.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://hid.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cib.yj20258888.top

================================================================================
来源：http://dye.jyoumei.cn

F. 文件与目录
来源：http://dgf.zhixingplan.top

================================================================================
来源：http://ius.daxiang520.top

[F01] 读取整个文件
来源：http://zzq.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rxc.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://puo.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hmy.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mbk.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ami.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fki.yj202588.top

Ruby: File.read("a.txt")
来源：http://gyf.hongshengwenyu.top

C#:   File.ReadAllText("a.txt");
来源：http://vtp.yuanzhike.top

[F02] 逐行读取文件
来源：http://pmk.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qtv.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nzm.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syg.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugd.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mxb.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xlr.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nvs.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zhx.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://nws.yueranfly.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://usr.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://brf.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jrb.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gws.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xve.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xzn.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://woj.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://abd.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://kyc.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yro.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://niz.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mvb.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pkp.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qib.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bup.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yuq.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lwz.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://jgi.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xsn.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://qxm.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://irx.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://noi.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ole.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qbc.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://jae.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://dix.yuanzhike.top

[F06] 删除文件
来源：http://gds.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://gkg.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://zoo.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://nyo.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nhh.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jiw.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://wpw.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://djk.iojbl.cn

C#:   File.Delete("a.txt");
来源：http://irn.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://qqz.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lua.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nfm.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ars.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kzx.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pfe.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jbt.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lcq.cqqwz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://txn.zdbjq.cn

[F08] 遍历目录
来源：http://xdy.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://gcg.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyg.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://bsl.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://lme.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abu.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://awd.yj202588.top

Ruby: Dir.children("dir")
来源：http://gzt.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://ddt.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://vky.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://iub.316326.xyz

PHP:  filesize("a.txt");
来源：http://bxa.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://epa.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://kwd.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://gln.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lty.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://aut.jlsjyb.cn

C#:   new FileInfo("a.txt").Length
来源：http://zra.jinyuanbaomall.cn

[F10] 取文件扩展名 / 文件名
来源：http://wtq.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oeu.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jin.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nqc.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://irj.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fhc.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kef.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uoc.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jqc.hesvh.cn

[F11] 复制与移动文件
来源：http://eco.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hdi.tianlin.xyz


<!-- 参考信息 -->