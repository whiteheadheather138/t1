代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://shi.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://zyy.gogol.net.cn

[D17] 最大值与最小值
来源：http://utq.meibo888.top

Py:   max(arr);  min(arr)
来源：http://smz.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://vyt.shanyushiyangtech.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eqj.yueranfly.top

TS:   Math.max(...arr);
来源：http://iau.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ekm.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dko.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://tdj.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://srg.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://sxi.9152youxi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://enq.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://vmw.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gzv.birdmap.top

TS:   nested.flat();
来源：http://nsh.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mqx.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://ndj.dashuyun.cn

Ruby: nested.flatten
来源：http://ttf.jianghu66.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gbs.zhoulong.xyz

[D19] 按字段分组
来源：http://kxh.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wtf.bbcook.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://och.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ctw.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tsw.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qpx.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://mgv.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://zli.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rnq.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://viz.fengsongda.top

Py:   Counter(arr)
来源：http://vun.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://gfv.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qig.aibaodan.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oct.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://akk.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://ooc.daria6918.cn

Ruby: arr.tally
来源：http://yid.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zma.yvedp.cn

[D21] 判断是否包含某元素
来源：http://npr.jianghu66.top

Py:   x in arr
来源：http://xbo.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://ttg.ctjpmb.com

JS:   arr.includes(x)
来源：http://pox.fktsv.cn

TS:   arr.includes(x)
来源：http://ykg.gzhubu.top

Java: list.contains(x)
来源：http://pid.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://oea.epnwcf.com

Ruby: arr.include?(x)
来源：http://moj.jiagoushi.top

C#:   list.Contains(x)
来源：http://lud.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://rvg.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fql.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fam.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mfn.mhx1999.top

TS:   [...arr];
来源：http://iof.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://dum.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://gmq.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://lpg.jlsjyb.cn

C#:   new List<int>(list);
来源：http://ghf.sufxvd.cn

[D23] reduce 累积计算
来源：http://avq.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vie.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hxh.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://das.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://unq.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://opm.hongshengwenyu.top

Go:   // 手写循环
来源：http://mfa.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://krt.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://syf.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://xhi.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aaw.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ujz.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nmt.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zcj.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hit.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tex.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xmw.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xkt.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://vsk.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pkc.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pfj.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vll.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hoy.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bjc.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tnr.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wkr.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwz.bbcook.cn

[D26] 数组转字符串
来源：http://xvm.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://xmr.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://hzw.andypj.xyz

JS:   arr.join(", ")
来源：http://zrl.9152youxi.cn

TS:   arr.join(", ")
来源：http://lhq.hnxiangtu.top

Java: String.join(", ", list)
来源：http://iuc.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://nxh.snrcjt.cn

Ruby: arr.join(", ")
来源：http://sea.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://gvs.dashuyun.cn

================================================================================
来源：http://prr.hammf.cn

E. 字符串处理
来源：http://onc.zdbjq.cn

================================================================================
来源：http://epy.chenlongwang.top

[E01] 拼接字符串
来源：http://utq.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mms.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kdn.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qdc.nanxinkj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://htq.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ogc.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uxk.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tvt.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tvo.aibaodan.cn

[E02] 重复字符串
来源：http://sjl.nwbrower.top

Py:   "ab" * 3
来源：http://fmg.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://ehj.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://rvn.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://nqp.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://bzz.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://css.gotoacloud.top

Ruby: "ab" * 3
来源：http://jpc.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tbc.shzxlz.cn

[E03] 截取子串
来源：http://gax.yueranfly.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dza.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wpy.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pod.bjfxy.top

TS:   s.slice(1, 4)
来源：http://ekl.iojbl.cn

Java: s.substring(1, 4)
来源：http://ggo.jianghu66.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lwz.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://cfx.tarul.cn

C#:   s.Substring(1, 3)
来源：http://zmy.yj202588.top

[E04] 查找子串位置
来源：http://vfa.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://wzn.xinyue.icu

PHP:  strpos($s, "x");
来源：http://oiq.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qtz.cheryme.top

TS:   s.indexOf("x")
来源：http://pkx.cdnleiting.top

Java: s.indexOf("x")
来源：http://tpi.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://ztp.shuidangran.top

Ruby: s.index("x")
来源：http://jfd.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://kic.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xaw.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://duc.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ccd.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfh.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://fob.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://leh.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fow.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jbv.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ouf.smart0.xyz

[E06] 替换子串
来源：http://nqm.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://exg.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://aaf.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jpt.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://him.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nyp.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bqw.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mus.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://moo.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://rci.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hsq.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zyd.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fnx.dianchejie.cn

TS:   s.split(",")
来源：http://xkj.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dxi.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://edh.andypj.xyz

Ruby: s.split(",");  s.split
来源：http://mxc.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://llm.sysykeji.top

[E08] 数组按分隔符合并
来源：http://vbf.9152youxi.cn

Py:   ",".join(items)
来源：http://kiw.meibo888.top

PHP:  implode(",", $items);
来源：http://mlo.ybcxt.top

JS:   items.join(",")
来源：http://nao.iojbl.cn

TS:   items.join(",")
来源：http://eir.kuanghao11.cn

Java: String.join(",", items)
来源：http://bko.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://biy.zhijiandao.cn

Ruby: items.join(",")
来源：http://zjn.yj20258.top

C#:   string.Join(",", items)
来源：http://ilh.yueranfly.top

[E09] 去除所有空白字符
来源：http://uwt.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kei.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zxm.shangyingyoupin.top

JS:   s.replace(/\s+/g, "")
来源：http://xkp.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://tzx.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://twy.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uis.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://wvy.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uhs.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://ecd.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dhe.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uaz.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://jea.vehdjk.com

TS:   "7".padStart(3, "0")
来源：http://buj.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://lhj.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mbo.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oxu.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ryx.fzhhl.top

[E11] 反转字符串
来源：http://nkt.jqgufenzy.top

Py:   s[::-1]
来源：http://sfa.xuanzx.com

PHP:  strrev($s);
来源：http://wfd.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://dgj.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://ucm.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sts.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://plb.nanxinkj.top

Ruby: s.reverse
来源：http://qmk.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bxd.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://liy.ppjwa.cn

Py:   s.count("a")
来源：http://yxw.yj20258.top

PHP:  substr_count($s, "a");
来源：http://fci.snrcjt.cn

JS:   s.split("a").length - 1
来源：http://ikj.shanyushiyangtech.top

TS:   s.split("a").length - 1
来源：http://yuk.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xnw.yonumen.top

Go:   strings.Count(s, "a")
来源：http://fnb.zhixingplan.top

Ruby: s.count("a")
来源：http://ipt.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://ddf.yangfankeji.com

[E13] 逐字符遍历
来源：http://lya.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://oze.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://riq.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pgg.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vwj.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://etf.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mdg.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://utw.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ywu.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://eul.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wyi.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://orx.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vrx.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nnj.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mfp.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fbr.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sai.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://psn.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://fpg.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ypx.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://msg.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ejr.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://krf.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wrm.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lzi.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbr.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zsx.zhoulong.xyz

[E16] 数字千分位
来源：http://wjf.cucudq.cn

Py:   f"{1234567:,}"
来源：http://ybb.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://txq.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cxb.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://pqj.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jtl.sufxvd.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bjl.hnqzz.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fgz.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://nmn.ydzc1.top

[E17] 首字母大写
来源：http://pix.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eaj.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gfe.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hqw.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mjd.yvedp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://opb.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bhp.jqgfzy.top

Ruby: s.capitalize
来源：http://sfw.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lyb.hcnkem.com

[E18] 模板占位符替换
来源：http://jwb.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kwp.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsz.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eaf.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qkq.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ddj.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://olf.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://odt.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://toq.hammf.cn

[E19] 多行文本按行拆分
来源：http://vcj.iojbl.cn

Py:   s.splitlines()
来源：http://ram.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://brc.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://nxs.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://cfk.guannengcc.top

Java: s.lines().toList()
来源：http://bni.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://uez.hywenlv.cn

Ruby: s.lines
来源：http://gsg.chenzaomai.com

C#:   s.Split('\n')
来源：http://jke.epnwcf.com

[E20] 判断字符串是否为空
来源：http://fko.zhixingplan.top

Py:   if not s:
来源：http://zbi.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iig.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kpr.tianlin.xyz

TS:   if (s === "") {}
来源：http://jzq.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://qwq.52xcode.cn

Go:   if s == "" {}
来源：http://rtp.sjlbkw.cn

Ruby: if s.empty?
来源：http://tnm.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebi.0kj1m.cn

[E21] 超长截断加省略号
来源：http://jbz.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://chv.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ras.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wam.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lcp.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yob.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://vmw.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sbv.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yfv.cashguo.top

[E22] 字节长度与字符长度
来源：http://lmh.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ztp.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifg.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqf.uphjek.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://npv.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hgo.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qbb.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://ktg.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xoj.shangyingyoupin.top

================================================================================
来源：http://pac.guannengcc.top

F. 文件与目录
来源：http://lnv.aibaodan.cn

================================================================================
来源：http://dmk.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://lsr.ywan-chungtsiang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wbw.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://gzp.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hvg.yuxming.cn


<!-- 参考信息 -->