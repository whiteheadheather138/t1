代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ywb.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://srt.zhoulong.xyz

Go:   // 手写循环
来源：http://rev.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vph.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rrw.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://bdk.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vwi.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://onb.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fat.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lqu.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://okk.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zrt.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dzi.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zhf.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://abe.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fdk.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sns.havefunace.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://arx.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hot.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eux.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ubk.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wxj.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aws.yueranfly.top

[D26] 数组转字符串
来源：http://zga.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://lyk.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://obi.zhixingplan.top

JS:   arr.join(", ")
来源：http://omk.c1oappe.top

TS:   arr.join(", ")
来源：http://drp.bbcook.cn

Java: String.join(", ", list)
来源：http://znu.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://ybg.yuanzhike.top

Ruby: arr.join(", ")
来源：http://zzo.cheryme.top

C#:   string.Join(", ", list)
来源：http://lhe.chenlongwang.top

================================================================================
来源：http://gzk.ivvv.top

E. 字符串处理
来源：http://ecu.andypj.xyz

================================================================================
来源：http://bgz.mhx1999.top

[E01] 拼接字符串
来源：http://vvt.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nwy.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hdb.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xzr.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fmn.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ued.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ptf.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jsg.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mfa.fengsongda.top

[E02] 重复字符串
来源：http://ioq.yueranfly.top

Py:   "ab" * 3
来源：http://kpb.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://tfz.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://jtz.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://eci.ehwqpu.com

Java: "ab".repeat(3)
来源：http://wkx.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://vlb.jinqigfzy.top

Ruby: "ab" * 3
来源：http://yfw.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dhh.yanxiufei.cn

[E03] 截取子串
来源：http://epn.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://two.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fuc.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxc.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://gnq.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://lcv.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fhs.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://qix.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://uvl.tarul.cn

[E04] 查找子串位置
来源：http://cwx.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://hxp.meibo888.top

PHP:  strpos($s, "x");
来源：http://nld.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kfi.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://vtj.sweek.top

Java: s.indexOf("x")
来源：http://jpk.hammf.cn

Go:   strings.Index(s, "x")
来源：http://kdb.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://ncl.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://pmj.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://inz.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jbv.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ydb.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sdq.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://swk.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wns.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jah.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dtc.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wfs.hcnkem.com

[E06] 替换子串
来源：http://gca.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pwc.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://syu.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://msb.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://aem.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iem.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tas.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rzf.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://nst.havefunace.top

[E07] 按分隔符拆分
来源：http://yjr.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uby.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qwh.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nyw.xingfuxueyuan.xyz

TS:   s.split(",")
来源：http://loj.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zmh.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ymt.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://hnn.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vjn.fktsv.cn

[E08] 数组按分隔符合并
来源：http://gih.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://oms.hysaishi.cn

PHP:  implode(",", $items);
来源：http://xgj.gogol.net.cn

JS:   items.join(",")
来源：http://gjk.zhixingplan.top

TS:   items.join(",")
来源：http://tck.yj202588.top

Java: String.join(",", items)
来源：http://lqa.tarul.cn

Go:   strings.Join(items, ",")
来源：http://vzy.xinyue.icu

Ruby: items.join(",")
来源：http://ijj.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://ssp.shzxlz.cn

[E09] 去除所有空白字符
来源：http://rxl.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://otf.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rfr.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://pqd.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ubi.yj20258888.top

Java: s.replaceAll("\\s+", "")
来源：http://blz.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lvp.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://ppy.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vpv.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://yos.guannengcc.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gyb.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zay.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://cvx.dianchejie.cn

TS:   "7".padStart(3, "0")
来源：http://yxj.ybcxt.top

Java: String.format("%03d", 7)
来源：http://cxa.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zwh.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dnb.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fra.ivvv.top

[E11] 反转字符串
来源：http://iko.fehbvm.com

Py:   s[::-1]
来源：http://hkx.fktsv.cn

PHP:  strrev($s);
来源：http://rci.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://rwa.birdmap.top

TS:   [...s].reverse().join("")
来源：http://ild.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ijd.jyoumei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wez.9152youxi.cn

Ruby: s.reverse
来源：http://ryn.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://fps.cheryme.top

[E12] 统计某字符出现次数
来源：http://vsf.hnqzz.top

Py:   s.count("a")
来源：http://zts.kuanghao11.cn

PHP:  substr_count($s, "a");
来源：http://lva.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://ytv.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://mgz.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://itk.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://bix.yj20258.top

Ruby: s.count("a")
来源：http://mxd.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://qhg.yj20258.top

[E13] 逐字符遍历
来源：http://fkj.yonumen.top

Py:   for ch in s: print(ch)
来源：http://vro.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bci.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zbm.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://nlv.snrcjt.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wbt.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eac.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pjq.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jck.smart0.xyz

[E14] URL 编码与 Base64
来源：http://did.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kes.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vql.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://syi.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tzr.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://etz.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dhv.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ned.zhoulong.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://maw.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://wje.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hbe.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qaq.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qnq.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://acx.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uhr.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iep.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://irg.quarkkingdee.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qbm.yueranfly.top

[E16] 数字千分位
来源：http://cip.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://xfj.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://uid.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://obu.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hws.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kpk.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wsp.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oro.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://tbs.gaohongyu789.top

[E17] 首字母大写
来源：http://xab.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zob.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://edz.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ink.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jhu.daxiang520.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kbj.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iay.hcnkem.com

Ruby: s.capitalize
来源：http://zvi.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lab.sjlbkw.cn

[E18] 模板占位符替换
来源：http://tzt.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pex.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iuw.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hll.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vyp.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vjb.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jzv.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xmr.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sja.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://yzx.snrcjt.cn

Py:   s.splitlines()
来源：http://cpr.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chr.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://zra.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://cwi.chenjidiqi.icu

Java: s.lines().toList()
来源：http://tuk.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://nkn.iojbl.cn

Ruby: s.lines
来源：http://ayu.cqqwz.cn

C#:   s.Split('\n')
来源：http://qvy.fehbvm.com

[E20] 判断字符串是否为空
来源：http://wpu.tanke756.top

Py:   if not s:
来源：http://asy.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://izi.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uox.jqgufenzy.top

TS:   if (s === "") {}
来源：http://qxp.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://yuh.hammf.cn

Go:   if s == "" {}
来源：http://xuj.dianchejie.cn

Ruby: if s.empty?
来源：http://tyu.daria6918.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xcx.daria6918.cn

[E21] 超长截断加省略号
来源：http://bdi.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://esg.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rjk.cashguo.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ilf.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hrw.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cnf.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://xpr.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xri.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nnw.nwbrower.top

[E22] 字节长度与字符长度
来源：http://eyx.ybcxt.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zcs.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apz.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oso.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ogq.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pxi.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://irc.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://kez.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oge.gogol.net.cn

================================================================================
来源：http://ppf.gaohongyu789.top

F. 文件与目录
来源：http://ejc.daria6918.cn

================================================================================
来源：http://nms.pycfn.com

[F01] 读取整个文件
来源：http://sux.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fcv.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://aca.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://meu.kuanghao11.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pln.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hxz.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tuy.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://pgf.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://jqe.yuanzhike.top

[F02] 逐行读取文件
来源：http://lqd.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sij.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vvy.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opr.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rbm.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://isi.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nhz.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rvt.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gzs.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://njd.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jhz.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://syx.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pft.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://arv.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xje.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cgh.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://piw.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lrd.hnqzz.top

[F04] 追加写入文件
来源：http://ljo.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rig.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vpy.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnu.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cci.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ont.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cjw.chenlongwang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wds.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dqi.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://ssb.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vdb.yj20258888.top

PHP:  file_exists("a.txt");
来源：http://lgz.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://vad.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://ule.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://exi.mhx1999.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hqh.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://gnq.aizwys.cn

C#:   File.Exists("a.txt")
来源：http://crl.fanxiaobao.xyz

[F06] 删除文件
来源：http://ipf.cashguo.top

Py:   os.remove("a.txt")
来源：http://dtv.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://kal.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://jkm.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rhw.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vlt.meibo888.top

Go:   os.Remove("a.txt")
来源：http://pyz.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://bbg.meibo888.top

C#:   File.Delete("a.txt");
来源：http://rqp.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://rlg.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mvh.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vxf.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nms.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cmx.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://unk.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sld.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pet.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hpb.mhx1999.top

[F08] 遍历目录
来源：http://oer.mhx1999.top


<!-- 参考信息 -->