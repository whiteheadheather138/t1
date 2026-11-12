代发 wailian999

[D15] 去重
来源：http://gts.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jsh.shuidangran.top

PHP:  array_unique($arr);
来源：http://uga.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://ndd.vehdjk.com

TS:   [...new Set(arr)]
来源：http://byp.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pnf.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ntf.chenlongwang.top

Ruby: arr.uniq
来源：http://uar.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://ylz.sxryk.cn

[D16] 求和与平均值
来源：http://sfl.ydzc1.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pci.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tor.xziqi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wom.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://skz.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://whp.tianlin.xyz

Go:   // 手写循环累加
来源：http://qrr.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yge.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://bhm.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://krh.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://wln.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://qiq.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yzh.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://rrs.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cly.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hgy.guannengcc.top

Ruby: arr.max;  arr.min
来源：http://ait.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://nhs.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://duo.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lxe.uphjek.com

PHP:  array_merge(...$nested);
来源：http://bfp.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cbc.bjfxy.top

TS:   nested.flat();
来源：http://xwn.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jqb.daxiang520.top

Go:   // 手写双层循环
来源：http://zgl.ybcxt.top

Ruby: nested.flatten
来源：http://pcr.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://loi.gzhubu.top

[D19] 按字段分组
来源：http://yox.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bam.epnwcf.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qsu.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://whf.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yum.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rrm.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://yjh.cqqwz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lfg.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://twc.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://wvf.jiagoushi.top

Py:   Counter(arr)
来源：http://gjq.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://rsa.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://azq.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fsu.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hfr.cqqwz.cn

Go:   // 手写 map[T]int
来源：http://suc.havefunace.top

Ruby: arr.tally
来源：http://luj.gogol.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bnd.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://eob.ydjk.org.cn

Py:   x in arr
来源：http://ywp.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://ybp.zdbjq.cn

JS:   arr.includes(x)
来源：http://ral.yvedp.cn

TS:   arr.includes(x)
来源：http://bwr.jinqigufen.top

Java: list.contains(x)
来源：http://wyr.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://lyj.yj202588.top

Ruby: arr.include?(x)
来源：http://gst.iojbl.cn

C#:   list.Contains(x)
来源：http://smk.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://tgb.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wny.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yxy.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dhr.kuanghao11.cn

TS:   [...arr];
来源：http://kqh.iojbl.cn

Java: new ArrayList<>(list);
来源：http://rqb.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://dkt.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://fjb.xziqi.cn

C#:   new List<int>(list);
来源：http://uyf.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://skp.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xzy.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nuc.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cri.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpo.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://kbs.yfazqb.com

Go:   // 手写循环
来源：http://dov.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dtr.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jjc.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://xvz.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://toa.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hph.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pgv.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ejo.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dtg.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lrp.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bru.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iyw.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://vke.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bgf.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pwj.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jaj.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xuo.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rza.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://huc.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dak.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://btj.uphjek.com

[D26] 数组转字符串
来源：http://wxi.dianchejie.cn

Py:   ", ".join(map(str, arr))
来源：http://die.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://fmv.ybcxt.top

JS:   arr.join(", ")
来源：http://sbv.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://eyp.bbcook.cn

Java: String.join(", ", list)
来源：http://eto.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://tyl.andypj.xyz

Ruby: arr.join(", ")
来源：http://ply.pycfn.com

C#:   string.Join(", ", list)
来源：http://lwr.hfpthk.cn

================================================================================
来源：http://mrn.yj202588.top

E. 字符串处理
来源：http://lyz.fzhhl.top

================================================================================
来源：http://hwl.sweek.top

[E01] 拼接字符串
来源：http://oty.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://boq.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gjr.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgy.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxi.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lnp.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mho.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eja.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zba.zdqjudy.top

[E02] 重复字符串
来源：http://wis.gaohongyu789.top

Py:   "ab" * 3
来源：http://wja.birdmap.top

PHP:  str_repeat("ab", 3);
来源：http://dqr.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://kav.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://cvc.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://pcg.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://hmt.zdbjq.cn

Ruby: "ab" * 3
来源：http://xlp.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mxu.gaohongyu789.top

[E03] 截取子串
来源：http://ljn.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://btc.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zlp.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sur.cheryme.top

TS:   s.slice(1, 4)
来源：http://day.aibaodan.cn

Java: s.substring(1, 4)
来源：http://sdr.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mdu.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wjd.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://bnt.zdqjudy.top

[E04] 查找子串位置
来源：http://ual.yueranfly.top

Py:   s.find("x");  s.index("x")
来源：http://bap.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://gcx.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fqs.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://stw.cheryme.top

Java: s.indexOf("x")
来源：http://cjk.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://ezy.xziqi.cn

Ruby: s.index("x")
来源：http://hnx.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://lhh.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fzo.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fhk.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hrg.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://obs.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zub.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ees.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vvl.zhixingplan.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nhk.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xdn.0kj1m.cn

[E06] 替换子串
来源：http://zwu.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ogn.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://xat.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcc.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://ywe.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vje.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nfa.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://flt.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://kfi.ybcxt.top

[E07] 按分隔符拆分
来源：http://ebk.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gry.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ojk.jinghuilouyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cfu.jinqigfzy.top

TS:   s.split(",")
来源：http://dlc.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://mjs.guannengcc.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvb.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://lnn.daria6918.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gjk.yongpay.top

[E08] 数组按分隔符合并
来源：http://txp.bbcook.cn

Py:   ",".join(items)
来源：http://qkm.redwolf501.top

PHP:  implode(",", $items);
来源：http://jwp.nwbrower.top

JS:   items.join(",")
来源：http://lbq.svipenyu.cn

TS:   items.join(",")
来源：http://gtb.ivvv.top

Java: String.join(",", items)
来源：http://otk.yj202588.top

Go:   strings.Join(items, ",")
来源：http://elm.vehdjk.com

Ruby: items.join(",")
来源：http://hao.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://zzo.yuxming.cn

[E09] 去除所有空白字符
来源：http://vgz.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vts.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ajk.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://gjp.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://txs.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://kge.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mej.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tqj.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cba.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://nrr.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://arn.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vnh.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://coa.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://eoq.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://aca.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rxk.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ylt.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jtm.xziqi.cn

[E11] 反转字符串
来源：http://gms.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://iwa.zhongyouzk.top

PHP:  strrev($s);
来源：http://yhv.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://mde.ydjk.org.cn

TS:   [...s].reverse().join("")
来源：http://ukh.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://per.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://diu.yvedp.cn

Ruby: s.reverse
来源：http://rls.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://uxo.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://goa.jlsjyb.cn

Py:   s.count("a")
来源：http://zne.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://fpr.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://lza.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://dbo.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xfg.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://zcf.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://spj.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://cpa.cdnleiting.top

[E13] 逐字符遍历
来源：http://uao.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://nzp.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tmk.yj20258.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dck.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oyn.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qhr.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kza.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gvj.xuetiantiany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jiq.sweek.top

[E14] URL 编码与 Base64
来源：http://jmb.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xze.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ura.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rcu.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://quw.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://stm.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zjd.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kcu.cheryme.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://abo.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://qcy.hammf.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hrh.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ufv.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://srr.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jhx.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ixq.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pjr.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zvq.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jre.zhoulong.xyz

[E16] 数字千分位
来源：http://rtq.kuanghao11.cn

Py:   f"{1234567:,}"
来源：http://ifd.dashuyun.cn

PHP:  number_format(1234567);
来源：http://zyv.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zbl.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rnt.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zvt.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://srq.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ydv.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://hql.daxiang520.top

[E17] 首字母大写
来源：http://ebv.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bne.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hyz.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gme.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://npp.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rtu.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kys.snrcjt.cn

Ruby: s.capitalize
来源：http://fmd.chenzaomai.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kzd.tianlin.xyz

[E18] 模板占位符替换
来源：http://lsf.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uwc.xylfe.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qqh.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://orp.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jql.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rey.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://urp.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sgg.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uwr.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://vbz.ppjwa.cn

Py:   s.splitlines()
来源：http://yza.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jkc.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://gka.fengsongda.top

TS:   s.split(/\r?\n/)
来源：http://qvb.xylfe.cn

Java: s.lines().toList()
来源：http://smn.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ogq.yonumen.top

Ruby: s.lines
来源：http://xwc.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://lmz.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://njo.feifeiyinyue.top

Py:   if not s:
来源：http://hby.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bqw.chenlongwang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ses.hysaishi.cn

TS:   if (s === "") {}
来源：http://grm.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://vnh.gaohongyu789.top

Go:   if s == "" {}
来源：http://tra.pycfn.com

Ruby: if s.empty?
来源：http://cax.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mia.andypj.xyz

[E21] 超长截断加省略号
来源：http://yin.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ulb.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wzc.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkb.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eib.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tyx.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://tuf.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nmu.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rgz.birdmap.top


<!-- 参考信息 -->