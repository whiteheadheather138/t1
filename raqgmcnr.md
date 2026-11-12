代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iul.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jhg.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gwq.tarul.cn

Go:   // 手写 map[T]int
来源：http://ayp.yueranfly.top

Ruby: arr.tally
来源：http://nke.ydjk.org.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwc.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://aev.haohaochexian.top

Py:   x in arr
来源：http://dln.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://bjp.shuidangran.top

JS:   arr.includes(x)
来源：http://old.52xcode.cn

TS:   arr.includes(x)
来源：http://ake.meibo888.top

Java: list.contains(x)
来源：http://tvf.dashuyun.cn

Go:   slices.Contains(arr, x)
来源：http://weo.yueranfly.top

Ruby: arr.include?(x)
来源：http://uvo.mhx1999.top

C#:   list.Contains(x)
来源：http://qqn.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://ssr.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fzy.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nhi.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vip.ivvv.top

TS:   [...arr];
来源：http://qgq.mhx1999.top

Java: new ArrayList<>(list);
来源：http://awx.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://lnm.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://wdv.yvedp.cn

C#:   new List<int>(list);
来源：http://nex.dianchejie.cn

[D23] reduce 累积计算
来源：http://hup.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tii.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hca.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bro.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pet.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kok.jiagoushi.top

Go:   // 手写循环
来源：http://qhs.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ajq.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jny.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://zyl.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gwh.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lfl.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ovp.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jhp.yanxiufei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fbq.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xzl.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ydy.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ijk.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://few.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ztt.hcnkem.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oyd.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wwd.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://shj.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ubi.yangfankeji.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://afm.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uoi.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qnn.ehwqpu.com

[D26] 数组转字符串
来源：http://zrp.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://ltp.tarul.cn

PHP:  implode(", ", $arr);
来源：http://gku.vqdsnc.cn

JS:   arr.join(", ")
来源：http://dbc.jiagoushi.top

TS:   arr.join(", ")
来源：http://zbv.tianlin.xyz

Java: String.join(", ", list)
来源：http://bjm.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://tjk.nwbrower.top

Ruby: arr.join(", ")
来源：http://yku.cqqwz.cn

C#:   string.Join(", ", list)
来源：http://btg.hnqzz.top

================================================================================
来源：http://rqy.birdmap.top

E. 字符串处理
来源：http://opg.jqgfzy.top

================================================================================
来源：http://szy.tarul.cn

[E01] 拼接字符串
来源：http://vnh.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lxl.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uix.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mxh.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://abf.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://utu.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjl.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ldp.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jlz.uphjek.com

[E02] 重复字符串
来源：http://zyw.iojbl.cn

Py:   "ab" * 3
来源：http://hgv.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://fbu.bbcook.cn

JS:   "ab".repeat(3)
来源：http://lag.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://bcl.yvedp.cn

Java: "ab".repeat(3)
来源：http://qpl.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://uar.hfpthk.cn

Ruby: "ab" * 3
来源：http://aoa.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eyk.9152youxi.cn

[E03] 截取子串
来源：http://ddl.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nfs.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bmf.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kce.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://jzx.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://hqs.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nqc.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://noi.cheryme.top

C#:   s.Substring(1, 3)
来源：http://cis.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://rfg.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://goq.zycfv.cn

PHP:  strpos($s, "x");
来源：http://qob.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mfj.guowangkeji.top

TS:   s.indexOf("x")
来源：http://gpi.zycfv.cn

Java: s.indexOf("x")
来源：http://gkz.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://wnc.52xcode.cn

Ruby: s.index("x")
来源：http://gli.epnwcf.com

C#:   s.IndexOf("x")
来源：http://mov.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jnz.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vsy.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xpd.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rtb.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://pzi.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vbr.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://atk.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gso.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vln.zdqjudy.top

[E06] 替换子串
来源：http://apx.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://edi.vehdjk.com

PHP:  str_replace("a", "b", $s);
来源：http://pom.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bbq.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://fxn.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyk.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bfd.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cpu.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://ueb.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://mhy.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ijn.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dwo.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cng.vehdjk.com

TS:   s.split(",")
来源：http://wir.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://ftv.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xig.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://lsk.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vex.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://tkd.yj20258888.top

Py:   ",".join(items)
来源：http://fps.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://jsv.ctjpmb.com

JS:   items.join(",")
来源：http://txi.nwbrower.top

TS:   items.join(",")
来源：http://wlc.yj20258.top

Java: String.join(",", items)
来源：http://qkn.yangfankeji.com

Go:   strings.Join(items, ",")
来源：http://tcj.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://nvl.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://uyg.dianchejie.cn

[E09] 去除所有空白字符
来源：http://jsz.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hhh.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ran.hywenlv.cn

JS:   s.replace(/\s+/g, "")
来源：http://qbl.dianchejie.cn

TS:   s.replace(/\s+/g, "")
来源：http://rdp.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://tjs.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://dbm.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://gne.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jln.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://cuq.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ubm.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zpy.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://fmg.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://lop.smart0.xyz

Java: String.format("%03d", 7)
来源：http://vpv.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gpd.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ekq.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uao.cucudq.cn

[E11] 反转字符串
来源：http://jqy.yuanzhike.top

Py:   s[::-1]
来源：http://cxl.52xcode.cn

PHP:  strrev($s);
来源：http://jdp.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://mbx.zhongyouzk.top

TS:   [...s].reverse().join("")
来源：http://vpq.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fcq.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nis.gotoacloud.top

Ruby: s.reverse
来源：http://las.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://lea.tian-w.cn

[E12] 统计某字符出现次数
来源：http://gtx.jinqigufen.top

Py:   s.count("a")
来源：http://kuu.tanke756.top

PHP:  substr_count($s, "a");
来源：http://ksg.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://wdz.uphjek.com

TS:   s.split("a").length - 1
来源：http://lne.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nvi.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://kfz.chenzaomai.com

Ruby: s.count("a")
来源：http://vcq.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://njn.epnwcf.com

[E13] 逐字符遍历
来源：http://lhk.hammf.cn

Py:   for ch in s: print(ch)
来源：http://cdh.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://osw.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://blc.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://arj.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bcd.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://whi.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mrf.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rrj.meibo888.top

[E14] URL 编码与 Base64
来源：http://qyj.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ocm.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yca.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nag.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cxw.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bgw.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://axz.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rxv.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rst.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://cog.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kui.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nfc.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yhw.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qtk.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ije.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ari.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ndc.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ggz.zhongyouzk.top

[E16] 数字千分位
来源：http://kqv.xziqi.cn

Py:   f"{1234567:,}"
来源：http://zem.fzhhl.top

PHP:  number_format(1234567);
来源：http://lsn.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://rzs.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://krx.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ahh.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kkb.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jxb.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://lrg.chenzaomai.com

[E17] 首字母大写
来源：http://hkh.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://axb.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://dxu.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qds.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pju.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wvt.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uqh.yanxiufei.cn

Ruby: s.capitalize
来源：http://gre.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ele.0kj1m.cn

[E18] 模板占位符替换
来源：http://fhm.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://set.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cyx.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iea.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://owy.tian-w.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kkj.vqdsnc.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zuw.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lnu.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nxe.guannengcc.top

[E19] 多行文本按行拆分
来源：http://ufq.tanke756.top

Py:   s.splitlines()
来源：http://icq.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://woj.haohaochexian.top

JS:   s.split(/\r?\n/)
来源：http://zfb.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://kpx.sufxvd.cn

Java: s.lines().toList()
来源：http://hgx.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://sds.ydjk.org.cn

Ruby: s.lines
来源：http://yvd.jinqigfzy.top

C#:   s.Split('\n')
来源：http://srk.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://mnd.dashuyun.cn

Py:   if not s:
来源：http://lan.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tkv.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uyw.cqqwz.cn

TS:   if (s === "") {}
来源：http://drd.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://yhr.yueranfly.top

Go:   if s == "" {}
来源：http://fta.sxryk.cn

Ruby: if s.empty?
来源：http://phb.ybcxt.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://txy.kuanghao11.cn

[E21] 超长截断加省略号
来源：http://cyi.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://llw.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zml.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhq.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://icq.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qql.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://vmq.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hda.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xtg.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://ati.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://feh.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qou.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tlb.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ban.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eyi.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mxf.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://wxd.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zrz.guannengcc.top

================================================================================
来源：http://vnj.ivvv.top

F. 文件与目录
来源：http://aab.tarul.cn

================================================================================
来源：http://gjn.hywenlv.cn

[F01] 读取整个文件
来源：http://efi.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sxh.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://gay.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cot.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bcb.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://mvt.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vuk.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://bsw.cheryme.top

C#:   File.ReadAllText("a.txt");
来源：http://slc.redwolf501.top

[F02] 逐行读取文件
来源：http://ivf.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mro.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vxi.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gko.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nqh.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://loe.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wng.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qki.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rsp.meibo888.top

[F03] 写入文件（覆盖）
来源：http://bmk.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ira.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://zwo.yuanzhike.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lgv.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fhw.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yld.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zvp.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://mri.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://urw.havefunace.top

[F04] 追加写入文件
来源：http://bhz.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cnz.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ldt.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqp.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gso.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oyx.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rsg.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://khg.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bii.gzhubu.top


<!-- 参考信息 -->