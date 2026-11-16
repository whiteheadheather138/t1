代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dbj.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nbs.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://eiq.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eqo.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bga.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cax.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kpl.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gzv.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://obi.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://duu.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://myu.havefunace.top

[D26] 数组转字符串
来源：http://qpe.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://xpj.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://tth.iojbl.cn

JS:   arr.join(", ")
来源：http://viv.quarkkingdee.top

TS:   arr.join(", ")
来源：http://ncv.bbcook.cn

Java: String.join(", ", list)
来源：http://wrv.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://min.andypj.xyz

Ruby: arr.join(", ")
来源：http://wuo.ybcxt.top

C#:   string.Join(", ", list)
来源：http://voy.hcnkem.com

================================================================================
来源：http://kcz.nanxinkj.top

E. 字符串处理
来源：http://fvn.uphjek.com

================================================================================
来源：http://gox.zdqjudy.top

[E01] 拼接字符串
来源：http://djb.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pct.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tac.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yng.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hcy.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qyi.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rzo.jyoumei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nom.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgx.cucudq.cn

[E02] 重复字符串
来源：http://wdp.jqgufenzy.top

Py:   "ab" * 3
来源：http://dls.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://fxb.birdmap.top

JS:   "ab".repeat(3)
来源：http://pmm.yongpay.top

TS:   "ab".repeat(3)
来源：http://nxu.cqqwz.cn

Java: "ab".repeat(3)
来源：http://vuv.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://ghy.zhijiandao.cn

Ruby: "ab" * 3
来源：http://rwz.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qnj.guannengcc.top

[E03] 截取子串
来源：http://myv.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ddh.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wps.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rqi.shuidangran.top

TS:   s.slice(1, 4)
来源：http://tsw.316326.xyz

Java: s.substring(1, 4)
来源：http://iqq.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ytg.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://kzj.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://fql.dashuyun.cn

[E04] 查找子串位置
来源：http://tvh.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://idv.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://pif.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wao.ehwqpu.com

TS:   s.indexOf("x")
来源：http://cua.snrcjt.cn

Java: s.indexOf("x")
来源：http://vsw.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://pyb.pengpengdd.cyou

Ruby: s.index("x")
来源：http://maj.yonumen.top

C#:   s.IndexOf("x")
来源：http://aip.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yiv.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dyv.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jpp.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fly.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ecm.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://clc.andypj.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hgj.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vss.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vnd.feifeiyinyue.top

[E06] 替换子串
来源：http://jci.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wku.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://gqr.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lja.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://azu.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://orz.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jcj.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aid.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://ora.ehwqpu.com

[E07] 按分隔符拆分
来源：http://sim.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cnk.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pez.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kxj.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://qny.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://off.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ldu.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://had.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cze.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://uli.jinqigfzy.top

Py:   ",".join(items)
来源：http://mba.zhixingplan.top

PHP:  implode(",", $items);
来源：http://yfa.jqgufenzy.top

JS:   items.join(",")
来源：http://wfl.birdmap.top

TS:   items.join(",")
来源：http://gdg.yangfankeji.com

Java: String.join(",", items)
来源：http://rki.sweek.top

Go:   strings.Join(items, ",")
来源：http://dvf.ppjwa.cn

Ruby: items.join(",")
来源：http://wgd.yangfankeji.com

C#:   string.Join(",", items)
来源：http://xxf.yueranfly.top

[E09] 去除所有空白字符
来源：http://uqm.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kjq.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zkm.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://oof.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://skt.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://hhe.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hkq.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://sqb.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://piz.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://pjc.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qmp.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jiy.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://mwt.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://eko.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://xam.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://dqi.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yqe.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oma.shangyingyoupin.top

[E11] 反转字符串
来源：http://dlq.zhiwuduotai.top

Py:   s[::-1]
来源：http://wza.jqgufenzy.top

PHP:  strrev($s);
来源：http://kyj.hysaishi.cn

JS:   [...s].reverse().join("")
来源：http://gas.yj20258888.top

TS:   [...s].reverse().join("")
来源：http://xgg.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://yap.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ohh.gaohongyu789.top

Ruby: s.reverse
来源：http://jml.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://yqz.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://uxd.wangshuangyany.cn

Py:   s.count("a")
来源：http://meo.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://ife.iojbl.cn

JS:   s.split("a").length - 1
来源：http://hve.fengsongda.top

TS:   s.split("a").length - 1
来源：http://fsv.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kyf.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://osf.gotoacloud.top

Ruby: s.count("a")
来源：http://tms.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://qrc.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://gqs.sysykeji.top

Py:   for ch in s: print(ch)
来源：http://szb.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vbm.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qwr.sysykeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mbr.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wgd.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qxq.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iqc.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qwb.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://ynf.c1oappe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mze.hcnkem.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://axa.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kzj.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bou.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hzb.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rvh.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fuq.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fcd.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://aaf.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ddf.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cgq.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hbe.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ddu.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mdq.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hhe.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wsl.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vsq.jqgfzy.top

[E16] 数字千分位
来源：http://bkn.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://hko.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://qoj.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://jzl.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mhg.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xuj.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fzu.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vys.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://ehb.zycfv.cn

[E17] 首字母大写
来源：http://jsd.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jlt.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nhq.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbq.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ywk.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tmv.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kyk.jinqigufen.top

Ruby: s.capitalize
来源：http://ipj.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zyg.aibaodan.cn

[E18] 模板占位符替换
来源：http://gwo.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ote.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://abd.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zbr.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://eys.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://osz.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ypy.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rnz.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wxn.yuxming.cn

[E19] 多行文本按行拆分
来源：http://wrc.chenlongwang.top

Py:   s.splitlines()
来源：http://asr.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ods.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://myy.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://yor.pycfn.com

Java: s.lines().toList()
来源：http://cui.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://qcw.hysaishi.cn

Ruby: s.lines
来源：http://fkq.havefunace.top

C#:   s.Split('\n')
来源：http://oly.tanke756.top

[E20] 判断字符串是否为空
来源：http://luo.jqgufenzy.top

Py:   if not s:
来源：http://yen.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gxx.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rtx.xinyue.icu

TS:   if (s === "") {}
来源：http://bvv.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://ali.nanxuanxn.top

Go:   if s == "" {}
来源：http://gbe.52xcode.cn

Ruby: if s.empty?
来源：http://yea.yj202588.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pfy.sufxvd.cn

[E21] 超长截断加省略号
来源：http://tos.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zfv.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jim.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cem.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wiq.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://peg.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://rzh.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jjf.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gmw.andypj.xyz

[E22] 字节长度与字符长度
来源：http://wwl.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jen.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zua.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dcu.guannengcc.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rtn.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ysn.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qjn.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://wov.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://srv.epnwcf.com

================================================================================
来源：http://mrb.gzhubu.top

F. 文件与目录
来源：http://ugr.shzxlz.cn

================================================================================
来源：http://ptc.nanxinkj.top

[F01] 读取整个文件
来源：http://cug.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ykd.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://dks.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dis.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hea.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gjk.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fpc.smart0.xyz

Ruby: File.read("a.txt")
来源：http://qiq.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://xpn.0kj1m.cn

[F02] 逐行读取文件
来源：http://ckf.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dik.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qtz.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://arb.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fzh.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xwn.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pzo.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mfk.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://whi.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://vcf.yj20258.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vpk.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://xty.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gif.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cex.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://slr.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ral.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://oth.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ojc.sweek.top

[F04] 追加写入文件
来源：http://qly.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tvx.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ums.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uml.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mlm.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dps.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jic.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fot.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dzr.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://zpy.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xdp.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://qqn.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://yqe.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://kvw.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kdq.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hzw.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://zzk.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://oev.zhixingplan.top

[F06] 删除文件
来源：http://buo.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://bks.cucudq.cn

PHP:  unlink("a.txt");
来源：http://hzi.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://fiy.fengsongda.top

TS:   fs.unlinkSync("a.txt")
来源：http://ogp.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lvf.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://nlv.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://osi.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://fwe.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://iib.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://axk.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jzx.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtj.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hqv.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lob.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ixz.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ifo.nanxinkj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lne.nanxuanxn.top

[F08] 遍历目录
来源：http://lkv.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://amp.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ujn.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://mga.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://hcj.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://osd.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://utt.hnqzz.top

Ruby: Dir.children("dir")
来源：http://fpk.zhiwuduotai.top

C#:   Directory.GetFiles("dir")
来源：http://tgm.jianghu66.top

[F09] 获取文件大小
来源：http://vqw.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://xsy.birdmap.top

PHP:  filesize("a.txt");
来源：http://ifv.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://rcb.smart0.xyz


<!-- 参考信息 -->