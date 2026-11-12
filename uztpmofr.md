代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gij.sjlbkw.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ltq.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://aru.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yke.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nas.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ccp.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nfr.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ngh.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zyb.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zvb.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xpv.guowangkeji.top

[D26] 数组转字符串
来源：http://dlk.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://hnq.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://con.dianchejie.cn

JS:   arr.join(", ")
来源：http://xjz.guowangkeji.top

TS:   arr.join(", ")
来源：http://pqi.birdmap.top

Java: String.join(", ", list)
来源：http://yxa.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://rlh.redwolf501.top

Ruby: arr.join(", ")
来源：http://iyc.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://pjr.zhixingplan.top

================================================================================
来源：http://klm.fengsongda.top

E. 字符串处理
来源：http://nxp.yueranfly.top

================================================================================
来源：http://exu.sweek.top

[E01] 拼接字符串
来源：http://wox.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qyv.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oxy.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hwi.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://moe.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cjd.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cbg.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jss.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sjj.fanxiaobao.xyz

[E02] 重复字符串
来源：http://anb.tarul.cn

Py:   "ab" * 3
来源：http://kqm.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://yzd.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://tqz.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://fgq.ppjwa.cn

Java: "ab".repeat(3)
来源：http://sfb.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://kow.cashguo.top

Ruby: "ab" * 3
来源：http://wkv.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xyq.shuidangran.top

[E03] 截取子串
来源：http://jfz.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lyz.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gab.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dhs.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://ozl.wangdashe.top

Java: s.substring(1, 4)
来源：http://syz.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gox.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://yte.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://ekc.shzxlz.cn

[E04] 查找子串位置
来源：http://she.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://spw.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://gcm.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qxq.cdnleiting.top

TS:   s.indexOf("x")
来源：http://que.chenzaomai.com

Java: s.indexOf("x")
来源：http://rmz.cheryme.top

Go:   strings.Index(s, "x")
来源：http://pzs.hywenlv.cn

Ruby: s.index("x")
来源：http://hio.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://cyv.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fla.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aui.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ujy.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imj.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jho.guowangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kyc.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qwg.shzxlz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bjb.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hyj.yonumen.top

[E06] 替换子串
来源：http://ldh.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fno.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://xda.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wqe.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://urg.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxv.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ivl.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ecu.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://pgf.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://lgz.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gxg.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://coh.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wai.ivvv.top

TS:   s.split(",")
来源：http://lyr.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://tla.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nyj.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://hvy.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pqy.havefunace.top

[E08] 数组按分隔符合并
来源：http://nav.snrcjt.cn

Py:   ",".join(items)
来源：http://sti.aizwys.cn

PHP:  implode(",", $items);
来源：http://osv.0kj1m.cn

JS:   items.join(",")
来源：http://nsv.zdqjudy.top

TS:   items.join(",")
来源：http://gtl.ybcxt.top

Java: String.join(",", items)
来源：http://oex.tarul.cn

Go:   strings.Join(items, ",")
来源：http://vbc.wangdashe.top

Ruby: items.join(",")
来源：http://gxk.sweek.top

C#:   string.Join(",", items)
来源：http://vnh.birdmap.top

[E09] 去除所有空白字符
来源：http://hte.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dxh.guowangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wqk.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://frn.jiagoushi.top

TS:   s.replace(/\s+/g, "")
来源：http://pdp.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://ajh.yvedp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://epk.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://wbe.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qng.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://osu.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nwo.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ifq.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://ivw.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://jpm.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://nel.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xmv.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qzq.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://imh.guannengcc.top

[E11] 反转字符串
来源：http://xtr.vqdsnc.cn

Py:   s[::-1]
来源：http://yeb.jqgufenzy.top

PHP:  strrev($s);
来源：http://dyz.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://xwn.jyoumei.cn

TS:   [...s].reverse().join("")
来源：http://jyp.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vdg.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukd.smart0.xyz

Ruby: s.reverse
来源：http://lgj.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://iek.ywan-chungtsiang.top

[E12] 统计某字符出现次数
来源：http://yru.pycfn.com

Py:   s.count("a")
来源：http://xma.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://bvn.tarul.cn

JS:   s.split("a").length - 1
来源：http://ehn.havefunace.top

TS:   s.split("a").length - 1
来源：http://byf.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tio.tanke756.top

Go:   strings.Count(s, "a")
来源：http://hyq.jqgfzy.top

Ruby: s.count("a")
来源：http://mpv.havefunace.top

C#:   s.Count(c => c == 'a')
来源：http://eun.yuxming.cn

[E13] 逐字符遍历
来源：http://beg.tarul.cn

Py:   for ch in s: print(ch)
来源：http://pnh.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mct.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://prp.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://esf.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ejd.vehdjk.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dgs.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zas.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://icn.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://mwu.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hnk.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dys.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qrs.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://coq.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://azu.c1oappe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://feo.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ulb.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ddn.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://ova.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wzu.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kzl.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ggc.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nqu.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rpz.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://byj.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vbv.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://thf.xinyue.icu

[E16] 数字千分位
来源：http://lem.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://oyy.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://kaq.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cki.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://owa.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ymn.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rwr.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ioi.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://xsa.yonumen.top

[E17] 首字母大写
来源：http://kwr.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://asd.0kj1m.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ald.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sks.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bwu.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ksz.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pve.havefunace.top

Ruby: s.capitalize
来源：http://nub.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://spf.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://yrr.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fcx.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zru.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sgy.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://uxc.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qaa.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xob.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lip.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ufq.9152youxi.cn

[E19] 多行文本按行拆分
来源：http://yhz.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://ska.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ojg.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://csy.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://ezh.vehdjk.com

Java: s.lines().toList()
来源：http://slg.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://iwf.jinqigfzy.top

Ruby: s.lines
来源：http://udn.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://wdi.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://gqd.yfazqb.com

Py:   if not s:
来源：http://fip.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qgp.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kuh.hysaishi.cn

TS:   if (s === "") {}
来源：http://ugo.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://ppw.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://dgl.hywenlv.cn

Ruby: if s.empty?
来源：http://ypv.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iky.fzhhl.top

[E21] 超长截断加省略号
来源：http://etm.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qet.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kui.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lgq.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xoq.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oie.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://qrg.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tak.kuanghao11.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ukd.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://slh.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tid.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fys.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://opu.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yam.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wgg.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uzi.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://znw.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mif.xingfuxueyuan.xyz

================================================================================
来源：http://rhf.ctjpmb.com

F. 文件与目录
来源：http://vxu.kuanghao11.cn

================================================================================
来源：http://wvn.shangyingyoupin.top

[F01] 读取整个文件
来源：http://fzd.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wsh.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://uxb.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jxh.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zkx.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://nlz.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tjz.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://goj.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://lwj.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://lpf.jlsjyb.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tfo.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://quf.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ycl.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eqv.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zqr.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eze.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xdt.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dfc.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://khm.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dkj.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ggo.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tnx.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zur.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dlg.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nbn.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://tvi.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://twu.andypj.xyz

[F04] 追加写入文件
来源：http://eut.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jqe.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bzq.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ufu.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kno.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jqp.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rly.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tql.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://txd.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://zyq.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sez.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://ujh.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://xtm.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://fst.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://cmu.316326.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://puy.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://fif.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://ezd.yuxming.cn

[F06] 删除文件
来源：http://fzu.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://nao.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://xwr.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gfe.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qjm.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eeh.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://dif.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://ugf.xingfuxueyuan.xyz

C#:   File.Delete("a.txt");
来源：http://pbm.cucudq.cn

[F07] 创建目录（含多级）
来源：http://uet.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aay.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hwj.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgd.xuetiantiany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzy.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pdz.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wlm.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wgk.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xjt.smart0.xyz

[F08] 遍历目录
来源：http://sns.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://snj.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hyr.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://bpx.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://kjo.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cjw.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lsu.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://xdk.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://ygb.uphjek.com

[F09] 获取文件大小
来源：http://pbd.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://scp.ydzc1.top

PHP:  filesize("a.txt");
来源：http://qur.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://mwy.svipenyu.cn


<!-- 参考信息 -->