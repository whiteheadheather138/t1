代发 wailian999

[D15] 去重
来源：http://ivj.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ukb.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://jkk.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://ctq.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://kie.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://joc.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vxs.sxryk.cn

Ruby: arr.uniq
来源：http://ofb.yonumen.top

C#:   list.Distinct().ToList()
来源：http://dza.ppjwa.cn

[D16] 求和与平均值
来源：http://ldn.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tmp.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tup.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mcn.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jsv.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pmn.tianlin.xyz

Go:   // 手写循环累加
来源：http://kud.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mca.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://bqv.yuanzhike.top

[D17] 最大值与最小值
来源：http://vfs.uphjek.com

Py:   max(arr);  min(arr)
来源：http://kvr.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://mkv.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmu.cheryme.top

TS:   Math.max(...arr);
来源：http://apq.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ykx.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cnp.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://rds.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://uvd.hammf.cn

[D18] 扁平化嵌套数组
来源：http://yhv.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bho.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://upi.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pbr.yuanzhike.top

TS:   nested.flat();
来源：http://qoq.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ojy.guowangkeji.top

Go:   // 手写双层循环
来源：http://gnb.yj20258888.top

Ruby: nested.flatten
来源：http://zkm.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lhm.redwolf501.top

[D19] 按字段分组
来源：http://gcg.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://edr.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vzl.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ucr.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://oeq.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oif.havefunace.top

Go:   // 手写 map[string][]T
来源：http://sqn.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://wqu.ybcxt.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vrc.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://pol.hcnkem.com

Py:   Counter(arr)
来源：http://pxq.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://yff.gogol.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://art.jinyuanbaomall.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zkt.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wyo.hongshengwenyu.top

Go:   // 手写 map[T]int
来源：http://grr.daria6918.cn

Ruby: arr.tally
来源：http://egk.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qvu.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://cdg.redwolf501.top

Py:   x in arr
来源：http://ryi.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://beh.dashuyun.cn

JS:   arr.includes(x)
来源：http://jly.andypj.xyz

TS:   arr.includes(x)
来源：http://mfu.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://cim.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://ksw.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://khn.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://uex.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://byl.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cid.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://git.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rhv.ydjk.org.cn

TS:   [...arr];
来源：http://sxb.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://ooz.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://nfi.ehwqpu.com

Ruby: arr.dup;  arr.clone
来源：http://cit.guowangkeji.top

C#:   new List<int>(list);
来源：http://xvt.xinyue.icu

[D23] reduce 累积计算
来源：http://bjo.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ssb.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iad.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zis.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mcx.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vvp.andypj.xyz

Go:   // 手写循环
来源：http://jlb.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kea.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mvn.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://iny.jinghuilouyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xdl.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pun.snrcjt.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fkf.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wsl.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qxs.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iad.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bsr.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iqp.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://rbj.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dbi.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jif.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pwj.hammf.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dzd.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wts.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qqh.pycfn.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dcg.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tyu.sjlbkw.cn

[D26] 数组转字符串
来源：http://nho.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://xrh.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://ijf.hcnkem.com

JS:   arr.join(", ")
来源：http://awb.sysykeji.top

TS:   arr.join(", ")
来源：http://sux.iojbl.cn

Java: String.join(", ", list)
来源：http://urj.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://ghq.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://btr.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://gsu.hysaishi.cn

================================================================================
来源：http://abp.316326.xyz

E. 字符串处理
来源：http://wor.yvedp.cn

================================================================================
来源：http://sgo.ybcxt.top

[E01] 拼接字符串
来源：http://dtu.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://knl.tanke756.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qpi.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oct.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzz.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ezv.ppjwa.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pcf.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xzz.cdnleiting.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://prs.vehdjk.com

[E02] 重复字符串
来源：http://qaa.cqqwz.cn

Py:   "ab" * 3
来源：http://dbt.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://kkm.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://tle.jianghu66.top

TS:   "ab".repeat(3)
来源：http://vxf.zhijiandao.cn

Java: "ab".repeat(3)
来源：http://eav.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://zew.316326.xyz

Ruby: "ab" * 3
来源：http://tqp.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fua.tanke756.top

[E03] 截取子串
来源：http://dvb.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nhh.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ftl.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ppf.birdmap.top

TS:   s.slice(1, 4)
来源：http://qlu.yfazqb.com

Java: s.substring(1, 4)
来源：http://qys.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zdj.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://pnw.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://gdu.meibo888.top

[E04] 查找子串位置
来源：http://uqi.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://iyo.sysykeji.top

PHP:  strpos($s, "x");
来源：http://jmk.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ese.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://wrx.9152youxi.cn

Java: s.indexOf("x")
来源：http://htn.cashguo.top

Go:   strings.Index(s, "x")
来源：http://smg.hywenlv.cn

Ruby: s.index("x")
来源：http://uhu.yuxming.cn

C#:   s.IndexOf("x")
来源：http://gkj.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ske.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aih.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esu.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pwk.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jnm.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gwk.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hne.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kci.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yiq.daria6918.cn

[E06] 替换子串
来源：http://zdu.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ldb.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://vhv.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sqo.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://sqo.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://isg.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dlf.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pfm.tanke756.top

C#:   s.Replace("a", "b")
来源：http://hfg.jyoumei.cn

[E07] 按分隔符拆分
来源：http://wgu.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vuv.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gxr.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bpg.gzhubu.top

TS:   s.split(",")
来源：http://gnq.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://ejr.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://khc.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://jaq.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aat.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://nxo.yongpay.top

Py:   ",".join(items)
来源：http://gzl.gzhubu.top

PHP:  implode(",", $items);
来源：http://dho.jqgfzy.top

JS:   items.join(",")
来源：http://xpz.guannengcc.top

TS:   items.join(",")
来源：http://pin.yuanzhike.top

Java: String.join(",", items)
来源：http://tep.zhijiandao.cn

Go:   strings.Join(items, ",")
来源：http://qrx.bbcook.cn

Ruby: items.join(",")
来源：http://skr.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://rfb.sysykeji.top

[E09] 去除所有空白字符
来源：http://giq.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xaw.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fxc.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://cme.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://lif.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://sse.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://skw.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://jyp.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ydp.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://hsl.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cev.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tyt.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://uim.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://qrc.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://awq.sysykeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fzc.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bts.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qih.zdbjq.cn

[E11] 反转字符串
来源：http://qcv.yj20258888.top

Py:   s[::-1]
来源：http://gee.haohaochexian.top

PHP:  strrev($s);
来源：http://xlg.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://uas.birdmap.top

TS:   [...s].reverse().join("")
来源：http://ncu.havefunace.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yri.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jrd.ctjpmb.com

Ruby: s.reverse
来源：http://ldp.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hyd.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://kkk.wangshuangyany.cn

Py:   s.count("a")
来源：http://ams.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://xhs.smart0.xyz

JS:   s.split("a").length - 1
来源：http://ugj.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://cdh.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ndi.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ilk.daxiang520.top

Ruby: s.count("a")
来源：http://toa.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://rbo.hywenlv.cn

[E13] 逐字符遍历
来源：http://uvf.tianlin.xyz

Py:   for ch in s: print(ch)
来源：http://nnt.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kzk.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://oys.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://edc.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xns.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hug.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://lys.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qew.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://uvx.shuidangran.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zus.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iks.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lxh.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hhu.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hnm.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ggl.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ofv.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dap.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://ekn.daria6918.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://adu.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uah.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://otg.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://awq.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rcs.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rgf.shzxlz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ofb.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kxp.fzhhl.top

[E16] 数字千分位
来源：http://fmv.cashguo.top

Py:   f"{1234567:,}"
来源：http://ayj.cashguo.top

PHP:  number_format(1234567);
来源：http://cdf.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mma.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fze.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dkp.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gxo.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xml.gotoacloud.top

C#:   1234567.ToString("N0")
来源：http://urg.jlsjyb.cn

[E17] 首字母大写
来源：http://yqh.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ywf.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ufp.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ggf.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hnb.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rwo.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gib.cashguo.top

Ruby: s.capitalize
来源：http://pha.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hbz.jinqigfzy.top

[E18] 模板占位符替换
来源：http://zld.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jjf.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lnh.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hwq.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ymp.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gkw.haohaochexian.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hsy.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tbd.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tsi.birdmap.top

[E19] 多行文本按行拆分
来源：http://wrd.fehbvm.com

Py:   s.splitlines()
来源：http://frs.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ubr.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://rye.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://kqs.guannengcc.top

Java: s.lines().toList()
来源：http://hbj.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://gou.jlsjyb.cn

Ruby: s.lines
来源：http://kqd.chenzaomai.com

C#:   s.Split('\n')
来源：http://zxr.yonumen.top

[E20] 判断字符串是否为空
来源：http://ayh.shzxlz.cn

Py:   if not s:
来源：http://hlr.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mxp.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lla.gogol.net.cn

TS:   if (s === "") {}
来源：http://spy.redwolf501.top

Java: if (s.isEmpty()) {}
来源：http://pcu.c1oappe.top

Go:   if s == "" {}
来源：http://xjq.cqqwz.cn

Ruby: if s.empty?
来源：http://khb.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eyq.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://nmy.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dqn.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tsn.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fcm.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fjs.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gvz.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://gzd.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yip.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hbj.yanxiufei.cn


<!-- 参考信息 -->