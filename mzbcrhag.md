代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qxl.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://htp.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lyb.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bky.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ple.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jln.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://agc.zhoulong.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jrk.wangshuangyany.cn

[E02] 重复字符串
来源：http://zoj.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://hvv.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://pgv.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://qng.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://joo.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://iqf.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://yrg.gzhubu.top

Ruby: "ab" * 3
来源：http://zsu.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fvt.quarkkingdee.top

[E03] 截取子串
来源：http://zot.vqdsnc.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://drg.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ntw.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://byr.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://bgj.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://scq.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pdi.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tub.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://aev.hywenlv.cn

[E04] 查找子串位置
来源：http://bvp.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://kmk.hesvh.cn

PHP:  strpos($s, "x");
来源：http://ukv.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jhh.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://khh.jianghu66.top

Java: s.indexOf("x")
来源：http://dbj.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://xmv.pycfn.com

Ruby: s.index("x")
来源：http://yvo.xuanzx.com

C#:   s.IndexOf("x")
来源：http://ilp.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nxp.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dpm.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fgg.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pya.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lhe.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqe.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tmz.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://whz.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vir.ydjk.org.cn

[E06] 替换子串
来源：http://aqw.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ehd.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://hwd.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qih.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://klg.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxk.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iam.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jky.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://mel.bjfxy.top

[E07] 按分隔符拆分
来源：http://sdd.gotoacloud.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://huy.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zdu.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kzr.sjlbkw.cn

TS:   s.split(",")
来源：http://kxk.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kuo.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gtq.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://wtl.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xuv.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://kjz.316326.xyz

Py:   ",".join(items)
来源：http://zdr.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://nsv.nanxuanxn.top

JS:   items.join(",")
来源：http://nhr.jinqigufen.top

TS:   items.join(",")
来源：http://dgo.52xcode.cn

Java: String.join(",", items)
来源：http://yod.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://ykp.bbcook.cn

Ruby: items.join(",")
来源：http://gbz.yfazqb.com

C#:   string.Join(",", items)
来源：http://bus.sufxvd.cn

[E09] 去除所有空白字符
来源：http://uaa.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://grf.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://obs.hesvh.cn

JS:   s.replace(/\s+/g, "")
来源：http://kuk.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://vjn.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://dqh.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfc.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oyb.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nii.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://rbe.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nol.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bmn.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://blz.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://hbw.cucudq.cn

Java: String.format("%03d", 7)
来源：http://snv.cdnleiting.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lbx.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rex.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxi.guannengcc.top

[E11] 反转字符串
来源：http://djm.quarkkingdee.top

Py:   s[::-1]
来源：http://vvp.jqgufenzy.top

PHP:  strrev($s);
来源：http://btd.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://kpo.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://hau.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dck.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://plq.shanyushiyangtech.top

Ruby: s.reverse
来源：http://mnn.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://wma.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://dsi.hywenlv.cn

Py:   s.count("a")
来源：http://ifz.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://izp.zhoulong.xyz

JS:   s.split("a").length - 1
来源：http://bis.ivvv.top

TS:   s.split("a").length - 1
来源：http://jzd.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://chc.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://pby.uphjek.com

Ruby: s.count("a")
来源：http://jfo.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://sef.ctjpmb.com

[E13] 逐字符遍历
来源：http://etj.ydjk.org.cn

Py:   for ch in s: print(ch)
来源：http://obt.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zgq.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vob.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://geq.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jrg.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fnu.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vxf.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jsa.fengsongda.top

[E14] URL 编码与 Base64
来源：http://dzm.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bgp.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://emo.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sav.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pwn.chenzaomai.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ogs.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kbm.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wyt.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mfe.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://bwg.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xci.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xan.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vtr.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://lmw.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fws.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jdq.yueranfly.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fmg.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rpl.jinqigfzy.top

[E16] 数字千分位
来源：http://qvm.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://ycf.9152youxi.cn

PHP:  number_format(1234567);
来源：http://ply.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vvy.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jdi.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uzp.zhaomingkeji.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dfl.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://svz.9152youxi.cn

C#:   1234567.ToString("N0")
来源：http://qqh.xziqi.cn

[E17] 首字母大写
来源：http://tvy.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xzv.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://siq.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ads.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lsp.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bzm.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ghm.sweek.top

Ruby: s.capitalize
来源：http://wpu.xinyue.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cql.epnwcf.com

[E18] 模板占位符替换
来源：http://mga.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://anj.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gpv.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://mae.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://rty.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kcp.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ajj.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qms.ydjk.org.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vjo.tarul.cn

[E19] 多行文本按行拆分
来源：http://rgi.fktsv.cn

Py:   s.splitlines()
来源：http://wpb.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gpt.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://oxr.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://ovv.pengpengdd.cyou

Java: s.lines().toList()
来源：http://nvg.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://hvc.tarul.cn

Ruby: s.lines
来源：http://pql.guowangkeji.top

C#:   s.Split('\n')
来源：http://cib.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://gmh.shangyingyoupin.top

Py:   if not s:
来源：http://tzg.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bsa.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dal.svipenyu.cn

TS:   if (s === "") {}
来源：http://sji.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://ucw.uphjek.com

Go:   if s == "" {}
来源：http://zki.havefunace.top

Ruby: if s.empty?
来源：http://jti.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pum.daria6918.cn

[E21] 超长截断加省略号
来源：http://lie.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zcc.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jsn.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymf.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://idp.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wqn.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://hxe.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://quc.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wag.andypj.xyz

[E22] 字节长度与字符长度
来源：http://upo.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vml.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yff.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cbd.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mqf.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://khg.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xuh.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://oni.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xrn.yvedp.cn

================================================================================
来源：http://qnn.zhengqikj.top

F. 文件与目录
来源：http://amr.sxryk.cn

================================================================================
来源：http://rrm.meibo888.top

[F01] 读取整个文件
来源：http://wwm.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ing.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://qsp.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cls.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://udq.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hvd.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cww.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://wlq.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://wxg.c1oappe.top

[F02] 逐行读取文件
来源：http://clw.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://org.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kto.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tjb.gaohongyu789.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lwt.hammf.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xbv.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kzc.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bwq.yj20258.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fkr.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://kxq.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ngu.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xcg.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kot.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://spl.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zcw.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jma.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://axx.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://abx.uphjek.com

[F04] 追加写入文件
来源：http://jek.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://emw.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xvg.cdnleiting.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjb.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mvc.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bel.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fni.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qng.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ckh.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://euo.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kmd.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://bqs.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://yop.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://fzn.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pgj.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fhr.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://dbq.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://ytz.quarkkingdee.top

[F06] 删除文件
来源：http://hva.havefunace.top

Py:   os.remove("a.txt")
来源：http://dwf.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://khw.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://txd.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://pgf.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hiq.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://qpc.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://kct.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://vyc.yvedp.cn

[F07] 创建目录（含多级）
来源：http://rag.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jll.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wlf.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dfe.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xal.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://czb.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://crf.bjfxy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uih.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dvo.dianchejie.cn

[F08] 遍历目录
来源：http://gnr.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://urx.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://drx.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://cab.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://idx.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cpm.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://uhy.cashguo.top

Ruby: Dir.children("dir")
来源：http://stq.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://ofc.xuetiantiany.cn

[F09] 获取文件大小
来源：http://zdc.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://edy.yonumen.top

PHP:  filesize("a.txt");
来源：http://gkl.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://uoh.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://bcz.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://qfk.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://egz.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://eio.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://tfx.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://fae.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wcv.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kbg.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bbr.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://prk.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lez.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ned.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fip.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aml.jqgufenzy.top

[F11] 复制与移动文件
来源：http://zbm.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://spi.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ysl.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qha.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vqv.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://daq.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hsa.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xbi.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cjj.0kj1m.cn

[F12] CSV 读写
来源：http://lwg.zhiwuduotai.top


<!-- 参考信息 -->