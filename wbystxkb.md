代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://zki.sysykeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iaz.yj202588.top

TS:   Math.max(...arr);
来源：http://opt.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://miz.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rnn.vqdsnc.cn

Ruby: arr.max;  arr.min
来源：http://udc.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://stw.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://xxl.shuidangran.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://txb.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://whf.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ewm.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://qhf.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ptx.tianlin.xyz

Go:   // 手写双层循环
来源：http://wir.yfazqb.com

Ruby: nested.flatten
来源：http://wkp.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cma.nanxuanxn.top

[D19] 按字段分组
来源：http://doy.uphjek.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hts.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vmn.shzxlz.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hgb.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cgs.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://prf.ivvv.top

Go:   // 手写 map[string][]T
来源：http://pad.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://jkv.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ryr.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://nuh.hnqzz.top

Py:   Counter(arr)
来源：http://fqz.zhiwuduotai.top

PHP:  array_count_values($arr);
来源：http://isr.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xwd.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qzw.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kyu.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://crz.ydjk.org.cn

Ruby: arr.tally
来源：http://zlv.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zua.tanke756.top

[D21] 判断是否包含某元素
来源：http://ucb.nanxuanxn.top

Py:   x in arr
来源：http://bga.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://net.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://wwr.ctjpmb.com

TS:   arr.includes(x)
来源：http://qgn.xylfe.cn

Java: list.contains(x)
来源：http://skr.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://vyg.yuanzhike.top

Ruby: arr.include?(x)
来源：http://uhs.jyoumei.cn

C#:   list.Contains(x)
来源：http://gab.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://igx.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gwc.jinqigfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ydr.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sjn.vehdjk.com

TS:   [...arr];
来源：http://rha.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://pkt.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://awf.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://gik.tarul.cn

C#:   new List<int>(list);
来源：http://snz.cashguo.top

[D23] reduce 累积计算
来源：http://lmi.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yig.yangfankeji.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nbu.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vrx.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mpj.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hcz.yonumen.top

Go:   // 手写循环
来源：http://zdk.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wva.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cme.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://cud.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yfp.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sar.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://srm.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wlg.xziqi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ixn.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zll.hcnkem.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xpw.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nmh.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://sul.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wlq.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xmq.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vpp.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vri.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pel.0kj1m.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ooj.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iuy.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ccs.yongpay.top

[D26] 数组转字符串
来源：http://beh.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://vxv.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://rip.xziqi.cn

JS:   arr.join(", ")
来源：http://rmx.nanxuanxn.top

TS:   arr.join(", ")
来源：http://ldf.sjlbkw.cn

Java: String.join(", ", list)
来源：http://yrz.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://jha.yj20258.top

Ruby: arr.join(", ")
来源：http://wkw.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://lev.hnqzz.top

================================================================================
来源：http://zqq.cdnleiting.top

E. 字符串处理
来源：http://ffj.ppjwa.cn

================================================================================
来源：http://oan.hywenlv.cn

[E01] 拼接字符串
来源：http://uzd.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://itd.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://efh.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hnm.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jsf.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gao.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lsu.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ipy.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uim.tianlin.xyz

[E02] 重复字符串
来源：http://hgt.jinqigufen.top

Py:   "ab" * 3
来源：http://nvj.yonumen.top

PHP:  str_repeat("ab", 3);
来源：http://pdi.yongpay.top

JS:   "ab".repeat(3)
来源：http://qfu.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://eth.0kj1m.cn

Java: "ab".repeat(3)
来源：http://szf.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://xmd.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://fvb.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://enw.svipenyu.cn

[E03] 截取子串
来源：http://mnn.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://scq.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ptw.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sax.nwbrower.top

TS:   s.slice(1, 4)
来源：http://igd.uphjek.com

Java: s.substring(1, 4)
来源：http://asp.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qik.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yiu.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://hdl.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://gtf.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://kam.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://bww.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dnh.fanxiaobao.xyz

TS:   s.indexOf("x")
来源：http://ofo.bjfxy.top

Java: s.indexOf("x")
来源：http://rmv.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://zfr.jlsjyb.cn

Ruby: s.index("x")
来源：http://hba.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://ksd.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lla.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ptn.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fba.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vqy.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://reb.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xra.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://che.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xdv.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jrx.uphjek.com

[E06] 替换子串
来源：http://lsi.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ros.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://qea.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zjg.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://tcg.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rst.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ozh.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zxp.pycfn.com

C#:   s.Replace("a", "b")
来源：http://hqm.hywenlv.cn

[E07] 按分隔符拆分
来源：http://tpe.xingfuxueyuan.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hma.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nrm.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wev.fehbvm.com

TS:   s.split(",")
来源：http://zie.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qqn.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rxw.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://ylh.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ltm.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://ifu.guowangkeji.top

Py:   ",".join(items)
来源：http://jip.epnwcf.com

PHP:  implode(",", $items);
来源：http://zzf.hfpthk.cn

JS:   items.join(",")
来源：http://fqo.xylfe.cn

TS:   items.join(",")
来源：http://knm.chenzaomai.com

Java: String.join(",", items)
来源：http://cch.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://jxi.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://cmr.iojbl.cn

C#:   string.Join(",", items)
来源：http://lij.nanxinkj.top

[E09] 去除所有空白字符
来源：http://qfl.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fwm.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hww.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://qyt.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://enj.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://egq.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yox.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://agb.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ktn.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://ppt.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://esw.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pqj.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://dbl.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://eev.shuidangran.top

Java: String.format("%03d", 7)
来源：http://gde.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://egp.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wbg.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://arb.zdqjudy.top

[E11] 反转字符串
来源：http://hou.aibaodan.cn

Py:   s[::-1]
来源：http://nxa.jqgfzy.top

PHP:  strrev($s);
来源：http://njd.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://uhz.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://ghy.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lij.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kgb.hysaishi.cn

Ruby: s.reverse
来源：http://sql.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://zmi.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://pgn.tarul.cn

Py:   s.count("a")
来源：http://ioc.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://jla.nanxuanxn.top

JS:   s.split("a").length - 1
来源：http://srn.hongshengwenyu.top

TS:   s.split("a").length - 1
来源：http://qzj.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://roc.pycfn.com

Go:   strings.Count(s, "a")
来源：http://sth.gotoacloud.top

Ruby: s.count("a")
来源：http://rtc.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://hyt.tarul.cn

[E13] 逐字符遍历
来源：http://pde.yonumen.top

Py:   for ch in s: print(ch)
来源：http://lex.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ygx.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fzz.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dem.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://leu.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ybs.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://jwv.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ubk.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://hta.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pwk.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ehv.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bnh.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hre.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lmt.xuetiantiany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jwm.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pus.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wjs.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://ujv.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sfz.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vdo.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ahb.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lhp.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oyj.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hfd.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rgl.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mal.xinyue.icu

[E16] 数字千分位
来源：http://xhz.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://yzx.aibaodan.cn

PHP:  number_format(1234567);
来源：http://jti.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ugk.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yvr.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ani.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jjm.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zsa.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://ykj.jinghuilouyu.cn

[E17] 首字母大写
来源：http://vbc.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bmc.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tbr.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sbw.yuxming.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ikb.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ksp.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://epz.bjfxy.top

Ruby: s.capitalize
来源：http://qpg.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://znt.vehdjk.com

[E18] 模板占位符替换
来源：http://yfy.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sri.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pln.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mcc.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://sxw.xingfuxueyuan.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ifr.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jcv.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dlh.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mzt.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://aev.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://txv.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dxf.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://fcn.daria6918.cn

TS:   s.split(/\r?\n/)
来源：http://cmg.chenjidiqi.icu

Java: s.lines().toList()
来源：http://qfn.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://gjp.yueranfly.top

Ruby: s.lines
来源：http://hfy.quarkkingdee.top

C#:   s.Split('\n')
来源：http://oap.gzhubu.top

[E20] 判断字符串是否为空
来源：http://jpt.jyoumei.cn

Py:   if not s:
来源：http://ufe.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jys.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oby.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://jde.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://oow.sysykeji.top

Go:   if s == "" {}
来源：http://wun.jqgufenzy.top

Ruby: if s.empty?
来源：http://iyx.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ngg.316326.xyz

[E21] 超长截断加省略号
来源：http://wfc.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ucr.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lll.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fsn.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://paj.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qzr.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://avo.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zom.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tia.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://trs.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mmg.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cly.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zqf.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ztn.zycfv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yzd.cdnleiting.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fwo.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://jzl.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ygp.haohaochexian.top

================================================================================
来源：http://inf.bjfxy.top

F. 文件与目录
来源：http://dff.gotoacloud.top

================================================================================
来源：http://akb.yuanzhike.top

[F01] 读取整个文件
来源：http://slh.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nbm.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://emw.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qbi.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbk.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ufp.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://myb.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://vom.tian-w.cn


<!-- 参考信息 -->