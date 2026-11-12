代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fms.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zsv.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://tbe.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ozn.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iiz.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ngg.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xip.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iqe.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tdr.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uzk.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hhd.ehwqpu.com

[D26] 数组转字符串
来源：http://uuv.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://oly.hfpthk.cn

PHP:  implode(", ", $arr);
来源：http://koc.zhongyouzk.top

JS:   arr.join(", ")
来源：http://vvq.ehwqpu.com

TS:   arr.join(", ")
来源：http://bbr.yfazqb.com

Java: String.join(", ", list)
来源：http://qfp.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://roi.haohaochexian.top

Ruby: arr.join(", ")
来源：http://mjl.hnqzz.top

C#:   string.Join(", ", list)
来源：http://cot.tanke756.top

================================================================================
来源：http://xul.cdnleiting.top

E. 字符串处理
来源：http://vsf.gogol.net.cn

================================================================================
来源：http://ucp.guannengcc.top

[E01] 拼接字符串
来源：http://lwv.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ccd.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jfe.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://duo.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ggj.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ufn.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jrh.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ovk.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hnx.jyoumei.cn

[E02] 重复字符串
来源：http://tyc.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://kzb.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://gug.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://jib.fktsv.cn

TS:   "ab".repeat(3)
来源：http://rqc.dashuyun.cn

Java: "ab".repeat(3)
来源：http://vek.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://sto.tanke756.top

Ruby: "ab" * 3
来源：http://zvy.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pvf.jlsjyb.cn

[E03] 截取子串
来源：http://vqt.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://scm.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://abo.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gqm.hfpthk.cn

TS:   s.slice(1, 4)
来源：http://mmr.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://zrw.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ntn.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://mar.shanyushiyangtech.top

C#:   s.Substring(1, 3)
来源：http://kcc.gzhubu.top

[E04] 查找子串位置
来源：http://nzx.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://vwm.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://fwx.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nwa.cdnleiting.top

TS:   s.indexOf("x")
来源：http://agj.xuanzx.com

Java: s.indexOf("x")
来源：http://pgc.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://lqr.ppjwa.cn

Ruby: s.index("x")
来源：http://lpp.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://nib.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mkk.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://crj.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vts.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsx.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://oay.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cqt.hammf.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://muo.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xgi.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ujm.epnwcf.com

[E06] 替换子串
来源：http://pys.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cgg.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://uqb.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bna.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://fgb.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xfx.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ciy.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dmy.havefunace.top

C#:   s.Replace("a", "b")
来源：http://dpw.chenzaomai.com

[E07] 按分隔符拆分
来源：http://wdr.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jev.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qij.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bzl.aibaodan.cn

TS:   s.split(",")
来源：http://lnt.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://lnz.fanxiaobao.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vhc.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://jsu.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lve.316326.xyz

[E08] 数组按分隔符合并
来源：http://yfg.52xcode.cn

Py:   ",".join(items)
来源：http://dnp.shzxlz.cn

PHP:  implode(",", $items);
来源：http://zdi.tian-w.cn

JS:   items.join(",")
来源：http://pwd.bjfxy.top

TS:   items.join(",")
来源：http://jsa.feifeiyinyue.top

Java: String.join(",", items)
来源：http://ncm.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://svf.ydjk.org.cn

Ruby: items.join(",")
来源：http://pes.wangdashe.top

C#:   string.Join(",", items)
来源：http://wgz.zdqjudy.top

[E09] 去除所有空白字符
来源：http://awj.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfb.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bhk.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://zne.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://hqt.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://rtp.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://onr.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://tpy.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://djz.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://ken.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zzb.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lhd.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://rzf.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://zng.meibo888.top

Java: String.format("%03d", 7)
来源：http://ubn.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sfs.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lpt.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hzd.shzxlz.cn

[E11] 反转字符串
来源：http://kzd.jianghu66.top

Py:   s[::-1]
来源：http://khc.haohaochexian.top

PHP:  strrev($s);
来源：http://ghs.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://okj.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://wlt.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vax.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://meh.yj20258.top

Ruby: s.reverse
来源：http://cqu.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nbf.gotoacloud.top

[E12] 统计某字符出现次数
来源：http://nzs.xuetiantiany.cn

Py:   s.count("a")
来源：http://iad.zhengqikj.top

PHP:  substr_count($s, "a");
来源：http://ksj.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://nap.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://wyo.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wwb.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://wdh.nanxuanxn.top

Ruby: s.count("a")
来源：http://pjh.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://bsd.wangdashe.top

[E13] 逐字符遍历
来源：http://iqh.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://mhh.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ygi.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xlh.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ogj.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tpm.chenlongwang.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aad.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://onw.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://icm.yuxming.cn

[E14] URL 编码与 Base64
来源：http://efp.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sew.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wbx.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wft.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://olo.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tkg.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fcd.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cjh.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uxu.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://cjm.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iqu.nwbrower.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kjs.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wvz.aibaodan.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fkk.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://top.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jhy.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cwc.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uww.wangshuangyany.cn

[E16] 数字千分位
来源：http://qft.pycfn.com

Py:   f"{1234567:,}"
来源：http://bon.chenlongwang.top

PHP:  number_format(1234567);
来源：http://hqc.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dih.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://yqw.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ich.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cpp.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://scg.uphjek.com

C#:   1234567.ToString("N0")
来源：http://lrh.jlsjyb.cn

[E17] 首字母大写
来源：http://tgj.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rdp.aibaodan.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://niq.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ilx.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eec.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mhe.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gta.yuanzhike.top

Ruby: s.capitalize
来源：http://zjx.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aws.shuidangran.top

[E18] 模板占位符替换
来源：http://jdn.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kpk.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://str.xingfuxueyuan.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://mqy.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://syk.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jyl.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mvg.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gpf.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://utx.yj20258888.top

[E19] 多行文本按行拆分
来源：http://nyl.dashuyun.cn

Py:   s.splitlines()
来源：http://tpc.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://umf.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://gum.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://gbb.nanxinkj.top

Java: s.lines().toList()
来源：http://sfw.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://mmf.wangshuangyany.cn

Ruby: s.lines
来源：http://vhz.jianghu66.top

C#:   s.Split('\n')
来源：http://jup.xinyue.icu

[E20] 判断字符串是否为空
来源：http://ogh.vehdjk.com

Py:   if not s:
来源：http://oib.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbb.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://slg.jianghu66.top

TS:   if (s === "") {}
来源：http://knv.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://fcn.zycfv.cn

Go:   if s == "" {}
来源：http://nqf.ydjk.org.cn

Ruby: if s.empty?
来源：http://ycz.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://grp.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://ocz.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ore.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bmx.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pcv.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjf.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vch.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://znx.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uca.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fzs.bjfxy.top

[E22] 字节长度与字符长度
来源：http://iqy.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bdi.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zvk.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpe.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvm.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ppg.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qfc.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://ujk.xylfe.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vom.zdqjudy.top

================================================================================
来源：http://cmq.sxryk.cn

F. 文件与目录
来源：http://kca.zhengqikj.top

================================================================================
来源：http://zxy.jinqigfzy.top

[F01] 读取整个文件
来源：http://hsu.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tyd.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://hqp.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kha.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xgk.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jfx.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yhr.snrcjt.cn

Ruby: File.read("a.txt")
来源：http://ghi.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://zud.dianchejie.cn

[F02] 逐行读取文件
来源：http://fue.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ucr.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hof.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://frp.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vnq.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jve.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mup.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fwv.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ecx.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://aso.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vff.gzhubu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ghn.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sut.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vhc.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xxm.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gyb.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://vwf.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hsw.chenlongwang.top

[F04] 追加写入文件
来源：http://uxd.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tmk.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jnh.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nkv.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://erj.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bjm.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://osx.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fji.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pep.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://uot.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gxy.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://tsz.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://eug.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://pxo.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://rwt.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zzi.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://bwh.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://wab.jyoumei.cn

[F06] 删除文件
来源：http://olc.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://tlt.yj202588.top

PHP:  unlink("a.txt");
来源：http://emr.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qay.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://aop.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nwa.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://mvp.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://dep.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://xhb.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://zrf.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://udv.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dek.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pdp.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hlm.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://peh.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wpd.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eum.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jce.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://ete.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wiv.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fgz.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://gnv.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://zzw.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ljk.wangdashe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lju.aizwys.cn

Ruby: Dir.children("dir")
来源：http://psg.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://vus.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://jws.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://yab.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://gzs.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://unr.ctjpmb.com


<!-- 参考信息 -->