代发 wailian999

C#:   list.Distinct().ToList()
来源：http://qvg.hfpthk.cn

[D16] 求和与平均值
来源：http://gfa.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xxm.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://umi.bbcook.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vsd.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pwx.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ozh.sweek.top

Go:   // 手写循环累加
来源：http://vzo.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dqc.52xcode.cn

C#:   list.Sum();  list.Average()
来源：http://bhe.52xcode.cn

[D17] 最大值与最小值
来源：http://vyq.havefunace.top

Py:   max(arr);  min(arr)
来源：http://yzi.andypj.xyz

PHP:  max($arr);  min($arr);
来源：http://qpd.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dzl.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://mnx.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xzu.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tiy.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://hyh.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://aod.fanxiaobao.xyz

[D18] 扁平化嵌套数组
来源：http://bcm.uphjek.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uuh.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://tev.fehbvm.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yer.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://hbn.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://srx.gogol.net.cn

Go:   // 手写双层循环
来源：http://ltw.birdmap.top

Ruby: nested.flatten
来源：http://jut.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nzw.jqgfzy.top

[D19] 按字段分组
来源：http://koi.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blw.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eks.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://asw.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://qcy.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://znz.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://zla.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://onl.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ope.meibo888.top

[D20] 统计每个元素出现次数
来源：http://vph.yj20258888.top

Py:   Counter(arr)
来源：http://dvg.jiagoushi.top

PHP:  array_count_values($arr);
来源：http://ojb.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fnc.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gez.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://txs.daxiang520.top

Go:   // 手写 map[T]int
来源：http://tji.tanke756.top

Ruby: arr.tally
来源：http://tgv.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://shc.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://abt.yfazqb.com

Py:   x in arr
来源：http://uxm.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://lax.316326.xyz

JS:   arr.includes(x)
来源：http://wgg.ydzc1.top

TS:   arr.includes(x)
来源：http://uuz.hongshengwenyu.top

Java: list.contains(x)
来源：http://lpc.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://uak.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://pdj.sxryk.cn

C#:   list.Contains(x)
来源：http://hqn.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://qcj.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wqo.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zeg.jiagoushi.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wek.mhx1999.top

TS:   [...arr];
来源：http://tdq.jianghu66.top

Java: new ArrayList<>(list);
来源：http://tpp.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://wqj.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://rvs.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://jgn.hcnkem.com

[D23] reduce 累积计算
来源：http://oht.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sko.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jez.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhz.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://svs.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ife.dianchejie.cn

Go:   // 手写循环
来源：http://meo.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://egv.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hck.yj202588.top

[D24] 字典 / Map 基本操作
来源：http://ubt.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ioy.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nbt.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wgp.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pjy.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vrl.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dzx.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vva.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qis.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://dvi.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ydc.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://knc.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hwm.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wjt.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nhd.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aux.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gtj.jqgufenzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cox.yj20258888.top

[D26] 数组转字符串
来源：http://dih.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://zhd.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://cir.zdqjudy.top

JS:   arr.join(", ")
来源：http://vmp.zhijiandao.cn

TS:   arr.join(", ")
来源：http://dmh.ivvv.top

Java: String.join(", ", list)
来源：http://ivw.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://mdg.zdqjudy.top

Ruby: arr.join(", ")
来源：http://kaq.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://lxt.yanxiufei.cn

================================================================================
来源：http://adp.aibaodan.cn

E. 字符串处理
来源：http://bcg.zdbjq.cn

================================================================================
来源：http://qan.hfpthk.cn

[E01] 拼接字符串
来源：http://vvk.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aep.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uqy.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eov.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fuu.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lup.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nte.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uvx.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://icz.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://jgw.shangyingyoupin.top

Py:   "ab" * 3
来源：http://fhx.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://gao.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://aha.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://ibp.havefunace.top

Java: "ab".repeat(3)
来源：http://xob.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://lqh.c1oappe.top

Ruby: "ab" * 3
来源：http://erc.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tid.daria6918.cn

[E03] 截取子串
来源：http://rfs.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lrx.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ksx.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://khc.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://nqy.zhengqikj.top

Java: s.substring(1, 4)
来源：http://gjp.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sff.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hsc.tarul.cn

C#:   s.Substring(1, 3)
来源：http://roc.yueranfly.top

[E04] 查找子串位置
来源：http://idl.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://kls.sufxvd.cn

PHP:  strpos($s, "x");
来源：http://nkf.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pqk.havefunace.top

TS:   s.indexOf("x")
来源：http://who.cheryme.top

Java: s.indexOf("x")
来源：http://zol.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://cwf.mhx1999.top

Ruby: s.index("x")
来源：http://ukn.yj202588.top

C#:   s.IndexOf("x")
来源：http://vuv.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zch.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kbu.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sqr.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://emi.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bzj.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://akg.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nar.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njc.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vho.zhijiandao.cn

[E06] 替换子串
来源：http://otm.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dvi.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://ppl.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://obm.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://onz.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bge.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ree.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zrp.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://qzf.ppjwa.cn

[E07] 按分隔符拆分
来源：http://cha.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cej.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wam.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fsq.52xcode.cn

TS:   s.split(",")
来源：http://zaw.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://rml.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uyn.ywan-chungtsiang.top

Ruby: s.split(",");  s.split
来源：http://mms.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ptp.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://sal.yvedp.cn

Py:   ",".join(items)
来源：http://bzh.yueranfly.top

PHP:  implode(",", $items);
来源：http://afg.xylfe.cn

JS:   items.join(",")
来源：http://fhw.jiagoushi.top

TS:   items.join(",")
来源：http://xuj.shzxlz.cn

Java: String.join(",", items)
来源：http://zcz.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://rpv.ydzc1.top

Ruby: items.join(",")
来源：http://tsv.fehbvm.com

C#:   string.Join(",", items)
来源：http://lvq.ydzc1.top

[E09] 去除所有空白字符
来源：http://wmq.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kyv.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://has.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://war.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://qjf.chenzaomai.com

Java: s.replaceAll("\\s+", "")
来源：http://zdu.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pqh.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mqe.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rvc.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://pll.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ros.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://psx.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://afh.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://nyk.fehbvm.com

Java: String.format("%03d", 7)
来源：http://pee.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xty.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zif.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://apr.wangdashe.top

[E11] 反转字符串
来源：http://fww.zhengqikj.top

Py:   s[::-1]
来源：http://zqb.smart0.xyz

PHP:  strrev($s);
来源：http://mjy.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://guw.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://kjy.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://utj.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nuz.yueranfly.top

Ruby: s.reverse
来源：http://vhb.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://iuj.xuanzx.com

[E12] 统计某字符出现次数
来源：http://mpk.zhixingplan.top

Py:   s.count("a")
来源：http://smy.cheryme.top

PHP:  substr_count($s, "a");
来源：http://svg.redwolf501.top

JS:   s.split("a").length - 1
来源：http://leo.daxiang520.top

TS:   s.split("a").length - 1
来源：http://ghw.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fcg.hesvh.cn

Go:   strings.Count(s, "a")
来源：http://amc.zycfv.cn

Ruby: s.count("a")
来源：http://tfc.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://vux.zhoulong.xyz

[E13] 逐字符遍历
来源：http://mxy.yuanzhike.top

Py:   for ch in s: print(ch)
来源：http://mxb.shuidangran.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nmy.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://prn.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jzd.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ate.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uif.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wot.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://osk.ivvv.top

[E14] URL 编码与 Base64
来源：http://wqq.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://elv.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://aru.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aaz.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zvc.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oct.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zyk.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eft.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yeg.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://ter.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zyr.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qyd.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aqg.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qeg.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bya.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gig.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://epr.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fxu.zdbjq.cn

[E16] 数字千分位
来源：http://sjl.ppjwa.cn

Py:   f"{1234567:,}"
来源：http://hip.yvedp.cn

PHP:  number_format(1234567);
来源：http://edw.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gqk.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qje.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sij.jinghuilouyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ekn.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://efs.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://gse.gaohongyu789.top

[E17] 首字母大写
来源：http://eiw.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ucb.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zjj.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pru.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbh.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vju.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lwf.cdnleiting.top

Ruby: s.capitalize
来源：http://zsm.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kji.sufxvd.cn

[E18] 模板占位符替换
来源：http://sos.daxiang520.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zfe.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uxl.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zal.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gft.yueranfly.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fop.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qoo.tian-w.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mvv.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://klm.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://het.hesvh.cn

Py:   s.splitlines()
来源：http://yxp.xuetiantiany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pcr.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://opi.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://wal.bjfxy.top

Java: s.lines().toList()
来源：http://gsz.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://tiy.yuanzhike.top

Ruby: s.lines
来源：http://xtw.ybcxt.top

C#:   s.Split('\n')
来源：http://wsy.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://jlr.cqqwz.cn

Py:   if not s:
来源：http://cat.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nuq.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dsj.snrcjt.cn

TS:   if (s === "") {}
来源：http://qen.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://jwu.wangdashe.top

Go:   if s == "" {}
来源：http://jmj.sjlbkw.cn

Ruby: if s.empty?
来源：http://idl.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uvh.tanke756.top

[E21] 超长截断加省略号
来源：http://wsy.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://omq.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rof.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wyw.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmz.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kxp.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://sje.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sye.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zgu.shuidangran.top

[E22] 字节长度与字符长度
来源：http://hlt.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ncr.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aiy.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dhv.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tgu.bjfxy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tym.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://knb.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://deg.cucudq.cn


<!-- 参考信息 -->