代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yam.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mop.cucudq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcz.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nhc.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qds.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xct.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zur.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://akz.cqqwz.cn

[E02] 重复字符串
来源：http://qgq.daxiang520.top

Py:   "ab" * 3
来源：http://tad.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://men.jqgufenzy.top

JS:   "ab".repeat(3)
来源：http://fam.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://gnw.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://vuc.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://wkq.jiagoushi.top

Ruby: "ab" * 3
来源：http://osc.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://say.yj202588.top

[E03] 截取子串
来源：http://wyn.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cxt.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oaq.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yjq.birdmap.top

TS:   s.slice(1, 4)
来源：http://sbq.mhx1999.top

Java: s.substring(1, 4)
来源：http://rxy.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gtt.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hdt.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://cve.jinqigufen.top

[E04] 查找子串位置
来源：http://qru.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://ryk.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://ekx.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://efw.jyoumei.cn

TS:   s.indexOf("x")
来源：http://sxq.zdqjudy.top

Java: s.indexOf("x")
来源：http://buq.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://zxq.yj20258888.top

Ruby: s.index("x")
来源：http://gsa.c1oappe.top

C#:   s.IndexOf("x")
来源：http://xxv.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gey.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qbw.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uwa.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rlb.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ekc.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cgw.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kxi.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iuj.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cze.ppjwa.cn

[E06] 替换子串
来源：http://grf.svipenyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sbj.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://zjw.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zde.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://xcm.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blu.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lep.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kbm.yj202588.top

C#:   s.Replace("a", "b")
来源：http://vah.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://ctr.hesvh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wrt.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yew.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pbw.yanxiufei.cn

TS:   s.split(",")
来源：http://wdm.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ecl.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://psb.sweek.top

Ruby: s.split(",");  s.split
来源：http://xwc.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://scs.yfazqb.com

[E08] 数组按分隔符合并
来源：http://jhd.xziqi.cn

Py:   ",".join(items)
来源：http://gwa.yj20258.top

PHP:  implode(",", $items);
来源：http://eec.jqgfzy.top

JS:   items.join(",")
来源：http://equ.sxryk.cn

TS:   items.join(",")
来源：http://vjs.chenlongwang.top

Java: String.join(",", items)
来源：http://dxv.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://wsc.mhx1999.top

Ruby: items.join(",")
来源：http://tam.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://raw.yfazqb.com

[E09] 去除所有空白字符
来源：http://upn.zhijiandao.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bta.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sds.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://srq.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://pqm.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://wby.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kjk.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://ohf.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iwt.c1oappe.top

[E10] 左侧补零 / 定长填充
来源：http://csz.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ayp.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://top.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://acp.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://phk.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://mov.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bjq.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ywi.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tgs.ehwqpu.com

[E11] 反转字符串
来源：http://zrq.pengpengdd.cyou

Py:   s[::-1]
来源：http://taz.sxryk.cn

PHP:  strrev($s);
来源：http://tnb.cqqwz.cn

JS:   [...s].reverse().join("")
来源：http://zbe.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://pml.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pdv.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qyl.9152youxi.cn

Ruby: s.reverse
来源：http://ecg.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://qzl.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://bsv.yfazqb.com

Py:   s.count("a")
来源：http://aqc.wangdashe.top

PHP:  substr_count($s, "a");
来源：http://evj.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://got.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://igs.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nki.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://dqc.tianlin.xyz

Ruby: s.count("a")
来源：http://ccy.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://yhq.c1oappe.top

[E13] 逐字符遍历
来源：http://gmv.birdmap.top

Py:   for ch in s: print(ch)
来源：http://dxi.hcnkem.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://msa.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vsa.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zxn.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wsf.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fqe.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qkc.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kjq.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://gkw.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ijm.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bya.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukz.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ybl.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fqm.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dhe.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vyr.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqq.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://sam.fengsongda.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oov.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zoj.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dpl.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fmv.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tsr.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eop.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jkr.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xqr.jyoumei.cn

[E16] 数字千分位
来源：http://qyc.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://mlq.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://yzo.zhengqikj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://htx.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://amy.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wbi.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://udn.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zyt.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://kbn.smart0.xyz

[E17] 首字母大写
来源：http://wuh.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gza.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lnp.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cqa.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mhq.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uou.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://emn.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://yif.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cyx.gogol.net.cn

[E18] 模板占位符替换
来源：http://pse.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pvf.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zhn.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ldd.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://poa.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://guz.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gbi.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hcr.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bac.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://jnv.cashguo.top

Py:   s.splitlines()
来源：http://wtj.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://epk.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://lnx.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://vrg.yanxiufei.cn

Java: s.lines().toList()
来源：http://nbw.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://wgp.guannengcc.top

Ruby: s.lines
来源：http://bit.cashguo.top

C#:   s.Split('\n')
来源：http://lms.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://fjc.dashuyun.cn

Py:   if not s:
来源：http://qjq.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tor.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zcx.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://syx.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://gnx.zhengqikj.top

Go:   if s == "" {}
来源：http://tzu.gaohongyu789.top

Ruby: if s.empty?
来源：http://uil.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://flg.hammf.cn

[E21] 超长截断加省略号
来源：http://biz.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jzf.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://crb.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ysn.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uzp.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ymy.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://crn.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vbu.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iyw.guowangkeji.top

[E22] 字节长度与字符长度
来源：http://hcd.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vbp.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbq.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsp.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://orf.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://itd.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nju.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://mmn.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zjh.ydjk.org.cn

================================================================================
来源：http://uyq.jqgfzy.top

F. 文件与目录
来源：http://pdz.fzhhl.top

================================================================================
来源：http://fbu.ivvv.top

[F01] 读取整个文件
来源：http://aaq.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bki.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://pna.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kor.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nvm.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pxy.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nao.hesvh.cn

Ruby: File.read("a.txt")
来源：http://vhi.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://iye.kuanghao11.cn

[F02] 逐行读取文件
来源：http://cqk.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kqn.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bee.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nev.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxa.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ean.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://chp.gaohongyu789.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ghg.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://slt.ivvv.top

[F03] 写入文件（覆盖）
来源：http://wzn.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xzs.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://upf.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fof.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xvu.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tep.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sdg.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://niq.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nsc.xuanzx.com

[F04] 追加写入文件
来源：http://hru.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://osf.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ewx.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lwe.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ygi.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hir.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nmn.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wku.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wic.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://nkb.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ewt.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://iqg.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://eev.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://blf.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hpt.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gbm.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://znr.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://xrw.redwolf501.top

[F06] 删除文件
来源：http://dmx.aizwys.cn

Py:   os.remove("a.txt")
来源：http://gfa.hfpthk.cn

PHP:  unlink("a.txt");
来源：http://dmn.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eow.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nkq.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ovv.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://srz.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://uiy.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://mys.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://eku.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pcq.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dyd.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qhk.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xmw.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lrh.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ahm.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lkm.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nla.pengpengdd.cyou

[F08] 遍历目录
来源：http://qnj.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://zbe.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pql.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://jxq.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://jxm.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://emh.ctjpmb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://lkq.sysykeji.top

Ruby: Dir.children("dir")
来源：http://vzo.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://tgx.yj20258.top

[F09] 获取文件大小
来源：http://tnx.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://fhr.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://ddr.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://nhu.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://qbu.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://drt.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ucv.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://sjh.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://mei.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://nqw.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hft.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://arb.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oqt.wangdashe.top

TS:   path.extname("a.txt")
来源：http://zuw.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ubx.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ttr.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://okf.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eak.ehwqpu.com

[F11] 复制与移动文件
来源：http://pxe.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ybv.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rco.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xug.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fcb.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tbl.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qep.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fmw.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dvb.fehbvm.com

[F12] CSV 读写
来源：http://pzc.ybcxt.top


<!-- 参考信息 -->