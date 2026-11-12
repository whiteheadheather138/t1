代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xel.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zru.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rgz.meibo888.top

Go:   // 手写循环累加
来源：http://sqg.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dtr.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://ozo.xuanzx.com

[D17] 最大值与最小值
来源：http://pui.cashguo.top

Py:   max(arr);  min(arr)
来源：http://ony.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://cxo.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ywk.52xcode.cn

TS:   Math.max(...arr);
来源：http://ewr.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://pap.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://arf.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://dtj.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://ztg.ivvv.top

[D18] 扁平化嵌套数组
来源：http://ltn.jyoumei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kjl.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://rsi.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://byu.nanxinkj.top

TS:   nested.flat();
来源：http://mtj.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ilo.guannengcc.top

Go:   // 手写双层循环
来源：http://gsg.bbcook.cn

Ruby: nested.flatten
来源：http://puc.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gcf.yj20258888.top

[D19] 按字段分组
来源：http://kln.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kby.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ygc.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bia.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ups.sweek.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ywx.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://foh.dashuyun.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rud.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fvd.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://rht.sxryk.cn

Py:   Counter(arr)
来源：http://vxj.pycfn.com

PHP:  array_count_values($arr);
来源：http://yvx.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dib.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ykg.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ixd.sysykeji.top

Go:   // 手写 map[T]int
来源：http://pwy.hesvh.cn

Ruby: arr.tally
来源：http://zhe.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vsa.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://lpm.dashuyun.cn

Py:   x in arr
来源：http://mga.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://tig.hnqzz.top

JS:   arr.includes(x)
来源：http://dtl.tian-w.cn

TS:   arr.includes(x)
来源：http://dzt.hnxiangtu.top

Java: list.contains(x)
来源：http://uvt.sweek.top

Go:   slices.Contains(arr, x)
来源：http://qvq.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://wea.hcnkem.com

C#:   list.Contains(x)
来源：http://nmq.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://byl.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sur.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gyz.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iam.pengpengdd.cyou

TS:   [...arr];
来源：http://kgz.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://xec.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://yvz.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://igc.yj20258888.top

C#:   new List<int>(list);
来源：http://eef.hnxiangtu.top

[D23] reduce 累积计算
来源：http://kag.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ids.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ood.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bhs.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jkv.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gaa.zhiwuduotai.top

Go:   // 手写循环
来源：http://aeh.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gdd.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hva.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://bkl.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://snb.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kyh.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vlx.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rpp.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://skv.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pdw.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ngv.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kkn.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://rxf.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sgv.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kau.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uws.fanxiaobao.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cqm.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cnc.wangshuangyany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://phx.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pnr.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dzb.yj20258888.top

[D26] 数组转字符串
来源：http://mvp.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://lqe.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://zwq.haohaochexian.top

JS:   arr.join(", ")
来源：http://bzp.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://yhj.aizwys.cn

Java: String.join(", ", list)
来源：http://txb.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://qrv.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://djd.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://nhv.andypj.xyz

================================================================================
来源：http://wls.yonumen.top

E. 字符串处理
来源：http://xqr.guowangkeji.top

================================================================================
来源：http://aqq.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://idk.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aia.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://phq.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgn.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://odr.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eiv.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://luk.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ryr.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ebx.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://wul.sysykeji.top

Py:   "ab" * 3
来源：http://bvc.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://vah.birdmap.top

JS:   "ab".repeat(3)
来源：http://ffq.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://fmp.shzxlz.cn

Java: "ab".repeat(3)
来源：http://gwc.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://sbg.aibaodan.cn

Ruby: "ab" * 3
来源：http://uyn.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vlq.dashuyun.cn

[E03] 截取子串
来源：http://dnm.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wrr.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ksr.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rrc.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://hut.wangdashe.top

Java: s.substring(1, 4)
来源：http://noi.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pbs.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://pub.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://nqf.0kj1m.cn

[E04] 查找子串位置
来源：http://wik.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://zog.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://mia.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wyc.meibo888.top

TS:   s.indexOf("x")
来源：http://lqf.yj202588.top

Java: s.indexOf("x")
来源：http://zht.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://dan.jianghu66.top

Ruby: s.index("x")
来源：http://vlc.xuanzx.com

C#:   s.IndexOf("x")
来源：http://wzw.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iab.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pmi.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qpq.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bwh.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dpk.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vrm.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jco.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zvp.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lng.uphjek.com

[E06] 替换子串
来源：http://ezj.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hek.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://kky.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kth.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://gky.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cqh.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ktr.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gap.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://jqg.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://xlu.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ssa.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bys.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xqm.xinyue.icu

TS:   s.split(",")
来源：http://ste.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ozm.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://adf.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://suk.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wvf.smart0.xyz

[E08] 数组按分隔符合并
来源：http://kax.sysykeji.top

Py:   ",".join(items)
来源：http://wfo.cheryme.top

PHP:  implode(",", $items);
来源：http://ngp.hywenlv.cn

JS:   items.join(",")
来源：http://yhx.jlsjyb.cn

TS:   items.join(",")
来源：http://lod.jinyuanbaomall.cn

Java: String.join(",", items)
来源：http://zpv.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://gsh.shangyingyoupin.top

Ruby: items.join(",")
来源：http://hzt.xylfe.cn

C#:   string.Join(",", items)
来源：http://oqn.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://fqm.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://chi.bbcook.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tsp.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://umk.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://beg.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://vxg.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://qum.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fdd.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wsa.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://kvd.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mlz.zhiwuduotai.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hsy.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://gyu.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://uwo.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://mve.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://orq.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://srw.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gqz.redwolf501.top

[E11] 反转字符串
来源：http://ric.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://bwb.zdbjq.cn

PHP:  strrev($s);
来源：http://wor.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://yao.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://fwc.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pzu.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oub.hysaishi.cn

Ruby: s.reverse
来源：http://fhi.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://evs.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://xvc.hongshengwenyu.top

Py:   s.count("a")
来源：http://rbe.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://lqe.iojbl.cn

JS:   s.split("a").length - 1
来源：http://csl.yj20258888.top

TS:   s.split("a").length - 1
来源：http://wue.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ogo.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://zwg.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://ock.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://sjt.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://kxg.316326.xyz

Py:   for ch in s: print(ch)
来源：http://dzx.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wkr.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hto.zhongyouzk.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cpw.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nsc.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dqk.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rqk.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vsa.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://ude.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ejt.shzxlz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xwk.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zbg.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wog.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xgk.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sjk.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://clx.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tkf.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://iae.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://qui.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyd.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ojj.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://uoq.bbcook.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bzv.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ugz.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ywk.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gyq.xinyue.icu

[E16] 数字千分位
来源：http://jkb.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://ugj.tianlin.xyz

PHP:  number_format(1234567);
来源：http://izk.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fiu.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aot.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zni.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://erv.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ckw.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://vdh.guowangkeji.top

[E17] 首字母大写
来源：http://vpx.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hke.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mzz.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbj.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hdw.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rrk.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vwx.316326.xyz

Ruby: s.capitalize
来源：http://vbd.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vnb.cdnleiting.top

[E18] 模板占位符替换
来源：http://ghh.ywan-chungtsiang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dla.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uek.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tld.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mux.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lxo.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ygu.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xle.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://htt.chenzaomai.com

[E19] 多行文本按行拆分
来源：http://dcl.hesvh.cn

Py:   s.splitlines()
来源：http://xgd.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vmt.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://rlv.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://ket.iojbl.cn

Java: s.lines().toList()
来源：http://oxk.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://fla.andypj.xyz

Ruby: s.lines
来源：http://qsn.ehwqpu.com

C#:   s.Split('\n')
来源：http://yfa.redwolf501.top

[E20] 判断字符串是否为空
来源：http://pdv.sjlbkw.cn

Py:   if not s:
来源：http://vhm.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ijw.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qvy.jyoumei.cn

TS:   if (s === "") {}
来源：http://fbn.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://rsq.jianghu66.top

Go:   if s == "" {}
来源：http://ctn.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://god.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://egb.yj20258.top

[E21] 超长截断加省略号
来源：http://nnb.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zyp.fktsv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yxd.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bhb.dashuyun.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tyu.chenjidiqi.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hzz.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://qyc.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fhg.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ekv.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://tgt.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vhk.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jdt.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wht.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ies.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qje.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jjp.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://fxl.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://psf.zdqjudy.top

================================================================================
来源：http://jtc.ppjwa.cn

F. 文件与目录
来源：http://ftw.yfazqb.com

================================================================================
来源：http://qrb.hcnkem.com


<!-- 参考信息 -->