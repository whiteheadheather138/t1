代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://bgl.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://qwz.nanxuanxn.top

JS:   arr.join(", ")
来源：http://idn.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://qdy.fktsv.cn

Java: String.join(", ", list)
来源：http://wur.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://pgc.bbcook.cn

Ruby: arr.join(", ")
来源：http://itn.cashguo.top

C#:   string.Join(", ", list)
来源：http://kym.hammf.cn

================================================================================
来源：http://qkp.jinqigfzy.top

E. 字符串处理
来源：http://xcy.sufxvd.cn

================================================================================
来源：http://msb.sufxvd.cn

[E01] 拼接字符串
来源：http://kue.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://avz.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lza.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mlt.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://epy.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xge.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ehf.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vko.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hxm.yonumen.top

[E02] 重复字符串
来源：http://giz.hnqzz.top

Py:   "ab" * 3
来源：http://jfa.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://ctg.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://ykw.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://rza.zdqjudy.top

Java: "ab".repeat(3)
来源：http://ykx.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://jgx.tianlin.xyz

Ruby: "ab" * 3
来源：http://lqf.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tci.xziqi.cn

[E03] 截取子串
来源：http://gmj.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yhw.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dwn.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mmm.fzhhl.top

TS:   s.slice(1, 4)
来源：http://jdk.tanke756.top

Java: s.substring(1, 4)
来源：http://bii.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ecs.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://tff.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://woj.gotoacloud.top

[E04] 查找子串位置
来源：http://owq.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://ckl.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://ycb.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dcy.316326.xyz

TS:   s.indexOf("x")
来源：http://zxv.hnxiangtu.top

Java: s.indexOf("x")
来源：http://xtt.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://myv.hesvh.cn

Ruby: s.index("x")
来源：http://fbk.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://oqa.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://shg.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lik.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sid.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pew.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tri.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qja.zdbjq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mmp.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rwd.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qah.ctjpmb.com

[E06] 替换子串
来源：http://iha.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wmk.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://ylv.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxu.jqgfzy.top

TS:   s.replaceAll("a", "b")
来源：http://czc.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cxn.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fqg.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uhk.316326.xyz

C#:   s.Replace("a", "b")
来源：http://xqg.cucudq.cn

[E07] 按分隔符拆分
来源：http://kkb.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nrt.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xhr.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cpn.aizwys.cn

TS:   s.split(",")
来源：http://jnj.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://gbs.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qma.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://brc.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qqg.meibo888.top

[E08] 数组按分隔符合并
来源：http://ysl.sjlbkw.cn

Py:   ",".join(items)
来源：http://qzu.ydzc1.top

PHP:  implode(",", $items);
来源：http://fbh.ydjk.org.cn

JS:   items.join(",")
来源：http://pqr.aizwys.cn

TS:   items.join(",")
来源：http://tpp.316326.xyz

Java: String.join(",", items)
来源：http://yyy.aibaodan.cn

Go:   strings.Join(items, ",")
来源：http://vlc.vehdjk.com

Ruby: items.join(",")
来源：http://fcc.jinqigufen.top

C#:   string.Join(",", items)
来源：http://tte.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://pmc.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bbz.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://noo.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://zjz.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://bip.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://cgx.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yyg.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://eqh.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dhp.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://hyz.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hbp.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nwg.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://blf.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://ees.shangyingyoupin.top

Java: String.format("%03d", 7)
来源：http://lht.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ged.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ipf.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dul.shanyushiyangtech.top

[E11] 反转字符串
来源：http://aae.yongpay.top

Py:   s[::-1]
来源：http://xtn.chenzaomai.com

PHP:  strrev($s);
来源：http://jvj.fengsongda.top

JS:   [...s].reverse().join("")
来源：http://ikm.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://rso.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nab.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://dxi.xziqi.cn

Ruby: s.reverse
来源：http://chh.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://eox.fzhhl.top

[E12] 统计某字符出现次数
来源：http://wfw.jqgufenzy.top

Py:   s.count("a")
来源：http://zpd.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://juo.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://vtl.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://ajj.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hvk.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://qzz.zhengqikj.top

Ruby: s.count("a")
来源：http://ymo.redwolf501.top

C#:   s.Count(c => c == 'a')
来源：http://ubz.fengsongda.top

[E13] 逐字符遍历
来源：http://oqe.sweek.top

Py:   for ch in s: print(ch)
来源：http://bvx.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://toy.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fag.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://keb.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wxh.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://svs.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dik.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sdq.birdmap.top

[E14] URL 编码与 Base64
来源：http://suq.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://box.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://hay.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cyi.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vfl.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bje.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hpp.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pcc.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://byo.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://ljb.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xgi.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dqw.yuanzhike.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gee.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://gyi.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fbf.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://srp.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ntv.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jjq.sweek.top

[E16] 数字千分位
来源：http://cfw.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://hpo.52xcode.cn

PHP:  number_format(1234567);
来源：http://ici.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tsy.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pwy.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hyy.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://umy.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qaf.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://cgy.dianchejie.cn

[E17] 首字母大写
来源：http://bfy.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pdi.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://eed.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://esd.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mze.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fmz.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://doj.hongshengwenyu.top

Ruby: s.capitalize
来源：http://wal.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nnm.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://ihl.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qfg.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gun.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jvl.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cjb.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cgr.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nhc.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mzw.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ago.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://ghv.hammf.cn

Py:   s.splitlines()
来源：http://smj.cashguo.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ocb.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://qyy.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://gyx.ybcxt.top

Java: s.lines().toList()
来源：http://sdp.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://xnl.yangfankeji.com

Ruby: s.lines
来源：http://evh.nanxuanxn.top

C#:   s.Split('\n')
来源：http://dmz.shanyushiyangkeji.top

[E20] 判断字符串是否为空
来源：http://uxm.zhengqikj.top

Py:   if not s:
来源：http://pqa.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gwa.fktsv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kdm.iojbl.cn

TS:   if (s === "") {}
来源：http://rcd.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://bqu.c1oappe.top

Go:   if s == "" {}
来源：http://jdc.redwolf501.top

Ruby: if s.empty?
来源：http://lfa.zdbjq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://djb.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://gnq.dianchejie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nlf.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://itx.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://btg.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nwi.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qvt.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://fre.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nqt.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cff.fktsv.cn

[E22] 字节长度与字符长度
来源：http://orl.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://atb.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mwz.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uad.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxe.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vmh.yj20258888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jwv.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://avq.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qgs.vehdjk.com

================================================================================
来源：http://tdp.ybcxt.top

F. 文件与目录
来源：http://fui.yanxiufei.cn

================================================================================
来源：http://pdq.yj20258888.top

[F01] 读取整个文件
来源：http://tmh.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vdl.tianlin.xyz

PHP:  file_get_contents("a.txt");
来源：http://mik.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nzr.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tud.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://akr.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jeb.sweek.top

Ruby: File.read("a.txt")
来源：http://nmk.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://eqk.meibo888.top

[F02] 逐行读取文件
来源：http://sqt.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ink.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vuw.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ptc.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fpf.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ofr.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bax.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oxl.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zsh.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://rhp.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zut.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://guy.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ihj.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vmz.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rjd.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ome.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://zba.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fec.gzhubu.top

[F04] 追加写入文件
来源：http://kka.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bub.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vry.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mnm.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://slp.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mns.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gfx.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yva.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vzb.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://bwh.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://frz.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://dty.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://ryk.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://jmq.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lhc.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ctf.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://how.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://fiv.chenlongwang.top

[F06] 删除文件
来源：http://ffl.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://hbb.316326.xyz

PHP:  unlink("a.txt");
来源：http://fjw.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://bhw.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ghq.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://llz.hammf.cn

Go:   os.Remove("a.txt")
来源：http://kvb.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://nxy.yj202588.top

C#:   File.Delete("a.txt");
来源：http://pzh.andypj.xyz

[F07] 创建目录（含多级）
来源：http://kso.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://clv.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bnh.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rcu.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dfh.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tuc.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gvs.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rdv.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://amb.shanyushiyangtech.top

[F08] 遍历目录
来源：http://ojl.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hed.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ygq.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://hck.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://kff.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oyu.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://xfv.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://chy.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://knb.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://ygu.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://ixk.bjfxy.top

PHP:  filesize("a.txt");
来源：http://acx.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://pes.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://hbb.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eix.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pmq.andypj.xyz

Ruby: File.size("a.txt")
来源：http://bsr.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://ghf.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://xds.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ovp.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ntj.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://flj.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://say.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cnc.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iou.wangdashe.top


<!-- 参考信息 -->