代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ede.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yne.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndk.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pyt.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vrl.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nqa.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nne.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://icc.nanxuanxn.top

[E02] 重复字符串
来源：http://mzt.aibaodan.cn

Py:   "ab" * 3
来源：http://xpl.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://bgc.sweek.top

JS:   "ab".repeat(3)
来源：http://lbm.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://mfn.tarul.cn

Java: "ab".repeat(3)
来源：http://xdg.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://rsf.zhongyouzk.top

Ruby: "ab" * 3
来源：http://zup.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://obg.hnqzz.top

[E03] 截取子串
来源：http://umc.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nzk.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ozn.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iwy.aizwys.cn

TS:   s.slice(1, 4)
来源：http://lmc.fzhhl.top

Java: s.substring(1, 4)
来源：http://gun.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rbl.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://epp.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://qsv.chenzaomai.com

[E04] 查找子串位置
来源：http://gog.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://wwk.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://huv.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tkp.9152youxi.cn

TS:   s.indexOf("x")
来源：http://dkr.nwbrower.top

Java: s.indexOf("x")
来源：http://nco.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://wmw.yongpay.top

Ruby: s.index("x")
来源：http://zwe.ppjwa.cn

C#:   s.IndexOf("x")
来源：http://sjc.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wve.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yrx.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xjj.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqd.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxb.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqb.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://msk.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mdi.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bby.aizwys.cn

[E06] 替换子串
来源：http://ueb.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bsn.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://lck.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://onm.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://ode.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gtt.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lax.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cxn.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://ytj.ivvv.top

[E07] 按分隔符拆分
来源：http://ccb.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qog.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ckb.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hgh.fanxiaobao.xyz

TS:   s.split(",")
来源：http://hnj.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nyw.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://juv.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://mqp.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xfy.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://bpr.uphjek.com

Py:   ",".join(items)
来源：http://onn.uphjek.com

PHP:  implode(",", $items);
来源：http://hmc.tarul.cn

JS:   items.join(",")
来源：http://wvm.ybcxt.top

TS:   items.join(",")
来源：http://lzc.xuanzx.com

Java: String.join(",", items)
来源：http://leb.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://aif.tanke756.top

Ruby: items.join(",")
来源：http://jch.guowangkeji.top

C#:   string.Join(",", items)
来源：http://mty.hesvh.cn

[E09] 去除所有空白字符
来源：http://igl.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ibh.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pbc.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://snk.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://ytx.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xhg.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://bll.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://lpl.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uww.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://ddv.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://spp.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pwi.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://qmg.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://yca.hesvh.cn

Java: String.format("%03d", 7)
来源：http://ipv.yuxming.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jkk.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://avy.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hmv.svipenyu.cn

[E11] 反转字符串
来源：http://inp.birdmap.top

Py:   s[::-1]
来源：http://hdj.meibo888.top

PHP:  strrev($s);
来源：http://ryq.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://fnd.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://fra.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kir.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://ngc.9152youxi.cn

Ruby: s.reverse
来源：http://qch.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vdq.mhx1999.top

[E12] 统计某字符出现次数
来源：http://qom.yongpay.top

Py:   s.count("a")
来源：http://cab.zdbjq.cn

PHP:  substr_count($s, "a");
来源：http://ndx.cucudq.cn

JS:   s.split("a").length - 1
来源：http://ppj.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://okc.meibo888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vdv.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://ppy.shanyushiyangkeji.top

Ruby: s.count("a")
来源：http://dkn.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://jta.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://afx.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://unr.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zan.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fpe.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dea.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xfd.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ewc.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ntd.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uak.c1oappe.top

[E14] URL 编码与 Base64
来源：http://jbs.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xpp.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ycg.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rhb.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lmd.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bej.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rod.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jvv.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzo.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://mvw.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mvy.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pvc.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://acr.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://roq.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mwb.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jck.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qzl.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lvh.sxryk.cn

[E16] 数字千分位
来源：http://xye.fengsongda.top

Py:   f"{1234567:,}"
来源：http://wjm.jiagoushi.top

PHP:  number_format(1234567);
来源：http://teh.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fzk.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://arn.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://npr.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ftl.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ukf.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://mmm.shzxlz.cn

[E17] 首字母大写
来源：http://txj.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vwb.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wgx.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ove.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://scl.wangshuangyany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nqc.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qir.hammf.cn

Ruby: s.capitalize
来源：http://icz.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://car.ctjpmb.com

[E18] 模板占位符替换
来源：http://lao.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mis.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://roy.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cnb.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ksl.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ruf.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gxz.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://agg.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hvh.nwbrower.top

[E19] 多行文本按行拆分
来源：http://onr.yanxiufei.cn

Py:   s.splitlines()
来源：http://xzr.daria6918.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bah.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://cpy.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://plu.jqgufenzy.top

Java: s.lines().toList()
来源：http://cti.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://thm.guannengcc.top

Ruby: s.lines
来源：http://hap.redwolf501.top

C#:   s.Split('\n')
来源：http://ird.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://knq.feifeiyinyue.top

Py:   if not s:
来源：http://cte.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gdv.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hxp.hnxiangtu.top

TS:   if (s === "") {}
来源：http://gra.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://lis.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://hvq.meibo888.top

Ruby: if s.empty?
来源：http://zbl.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cld.yuanzhike.top

[E21] 超长截断加省略号
来源：http://kpe.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lbc.jianghu66.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vhe.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ljb.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gco.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uag.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://npb.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sog.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mbk.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://klx.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vqb.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bxv.snrcjt.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xnm.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://whe.xuetiantiany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yhm.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nyf.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://evr.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bie.jinqigufen.top

================================================================================
来源：http://wbe.ppjwa.cn

F. 文件与目录
来源：http://tae.52xcode.cn

================================================================================
来源：http://gxf.ydzc1.top

[F01] 读取整个文件
来源：http://lnj.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qmm.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://wti.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://emu.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vdo.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ixb.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oxx.bjfxy.top

Ruby: File.read("a.txt")
来源：http://ymi.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://lkp.yueranfly.top

[F02] 逐行读取文件
来源：http://jyn.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hvw.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ueq.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akq.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kcz.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dnt.hammf.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lki.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://myn.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iai.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://dit.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fua.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dvr.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gdv.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rhn.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ldn.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fzh.dashuyun.cn

Ruby: File.write("a.txt", "hi")
来源：http://awr.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ipa.jiagoushi.top

[F04] 追加写入文件
来源：http://gyx.feifeiyinyue.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qea.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fnz.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ktt.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyn.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qnk.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kyy.zhongyouzk.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yro.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cyh.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://pbc.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://smj.sweek.top

PHP:  file_exists("a.txt");
来源：http://now.gaohongyu789.top

JS:   fs.existsSync("a.txt")
来源：http://dwb.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://xlu.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://gyb.tarul.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zez.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://rai.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://qun.jiagoushi.top

[F06] 删除文件
来源：http://ivg.bbcook.cn

Py:   os.remove("a.txt")
来源：http://udh.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://sbl.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://qwn.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vmd.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ndv.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://uiw.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://uud.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://wbi.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://tlo.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lwq.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mjd.aibaodan.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://niu.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tpl.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jbg.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://txd.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hik.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mdi.bbcook.cn

[F08] 遍历目录
来源：http://var.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xvj.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cxq.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://eag.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://vlk.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qvw.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xdv.havefunace.top

Ruby: Dir.children("dir")
来源：http://nro.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://ofc.vehdjk.com

[F09] 获取文件大小
来源：http://the.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://yab.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://gfc.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://hed.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://mab.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://czx.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tcb.ybcxt.top

Ruby: File.size("a.txt")
来源：http://cuh.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://xhz.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://xnc.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wnr.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tme.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vkf.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://opb.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oxl.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bpm.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rrt.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://avf.daria6918.cn

[F11] 复制与移动文件
来源：http://fmq.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ymr.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qeb.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wpg.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lao.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jje.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aey.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://don.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ecu.jyoumei.cn

[F12] CSV 读写
来源：http://dpa.ppjwa.cn


<!-- 参考信息 -->