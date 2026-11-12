代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pdl.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://qjl.dianchejie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://anb.yangfankeji.com

[D14] 映射转换（每个元素变形）
来源：http://npv.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lqo.havefunace.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lzp.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://kzv.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://wrx.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ejh.svipenyu.cn

Go:   // 手写循环
来源：http://gzd.yj20258.top

Ruby: arr.map { |x| x * 2 }
来源：http://lwf.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tdn.cucudq.cn

[D15] 去重
来源：http://wuw.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tdg.hysaishi.cn

PHP:  array_unique($arr);
来源：http://nub.zycfv.cn

JS:   [...new Set(arr)]
来源：http://tqm.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://nwy.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pye.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://chg.yuxming.cn

Ruby: arr.uniq
来源：http://unu.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://ybz.bbcook.cn

[D16] 求和与平均值
来源：http://zlg.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wzf.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://whj.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wzh.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tiw.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bok.aibaodan.cn

Go:   // 手写循环累加
来源：http://yxg.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://taf.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://zfo.redwolf501.top

[D17] 最大值与最小值
来源：http://qoa.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://cag.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://lke.wangshuangyany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iyj.52xcode.cn

TS:   Math.max(...arr);
来源：http://jvu.yfazqb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://icv.gaohongyu789.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iun.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://glv.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://wwy.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://jin.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://udn.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://gux.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iit.0kj1m.cn

TS:   nested.flat();
来源：http://zzo.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://byh.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://blp.hfpthk.cn

Ruby: nested.flatten
来源：http://wdw.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wfu.ydzc1.top

[D19] 按字段分组
来源：http://qry.vehdjk.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oyt.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qxy.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://men.quarkkingdee.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yeb.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zbx.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://ukf.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://swj.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fnc.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://dss.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://qbx.hammf.cn

PHP:  array_count_values($arr);
来源：http://vdi.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npg.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzh.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sfr.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://yyk.cdnleiting.top

Ruby: arr.tally
来源：http://aho.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qcp.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://ucj.jianghu66.top

Py:   x in arr
来源：http://fgn.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://hjf.yj20258888.top

JS:   arr.includes(x)
来源：http://cjr.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://tew.yj20258.top

Java: list.contains(x)
来源：http://ojg.yfazqb.com

Go:   slices.Contains(arr, x)
来源：http://ccm.andypj.xyz

Ruby: arr.include?(x)
来源：http://hyj.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://hwx.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://oes.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://apj.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xar.haohaochexian.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jza.yuanzhike.top

TS:   [...arr];
来源：http://znl.ivvv.top

Java: new ArrayList<>(list);
来源：http://gyv.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://lpj.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://pct.guannengcc.top

C#:   new List<int>(list);
来源：http://nsh.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://lrc.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://flv.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://opu.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hwx.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xgi.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://sjb.zhongyouzk.top

Go:   // 手写循环
来源：http://xbv.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://elq.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mdg.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://kuq.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://onr.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tiy.chenlongwang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nwy.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pdb.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eto.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lmm.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://arf.jinyuanbaomall.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sha.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://cie.yj202588.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tdy.yuanzhike.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qkj.jianghu66.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://txg.daria6918.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mjg.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cja.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qst.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hoe.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ygx.andypj.xyz

[D26] 数组转字符串
来源：http://ing.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://szh.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://yfa.vqdsnc.cn

JS:   arr.join(", ")
来源：http://xby.ybcxt.top

TS:   arr.join(", ")
来源：http://wgq.zdbjq.cn

Java: String.join(", ", list)
来源：http://hjo.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://qwi.cucudq.cn

Ruby: arr.join(", ")
来源：http://mdd.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://riz.xingfuxueyuan.xyz

================================================================================
来源：http://yvk.ivvv.top

E. 字符串处理
来源：http://bmt.cucudq.cn

================================================================================
来源：http://spj.andypj.xyz

[E01] 拼接字符串
来源：http://mfi.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jap.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bli.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qdv.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gwl.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ukw.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eqn.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xeq.zhixingplan.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tvq.yvedp.cn

[E02] 重复字符串
来源：http://aue.dashuyun.cn

Py:   "ab" * 3
来源：http://ygn.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://kbk.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://mja.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://glu.sweek.top

Java: "ab".repeat(3)
来源：http://mjj.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://ent.jyoumei.cn

Ruby: "ab" * 3
来源：http://bvc.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dsi.hcnkem.com

[E03] 截取子串
来源：http://zhs.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zue.yuxming.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lps.gotoacloud.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://amx.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://bqy.gogol.net.cn

Java: s.substring(1, 4)
来源：http://ydc.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aql.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://miz.sweek.top

C#:   s.Substring(1, 3)
来源：http://thd.dianchejie.cn

[E04] 查找子串位置
来源：http://rdq.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://orp.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://mcw.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qzw.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://rvm.haohaochexian.top

Java: s.indexOf("x")
来源：http://lub.meibo888.top

Go:   strings.Index(s, "x")
来源：http://wov.wangdashe.top

Ruby: s.index("x")
来源：http://uay.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://ova.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zll.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qtc.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nlw.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnq.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xmg.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppe.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hak.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zgx.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cmz.haohaochexian.top

[E06] 替换子串
来源：http://gfh.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://azz.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://gur.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hkc.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://lsi.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tho.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xvo.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://flo.yongpay.top

C#:   s.Replace("a", "b")
来源：http://dkj.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://gys.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xly.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xyn.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zvk.52xcode.cn

TS:   s.split(",")
来源：http://gft.cashguo.top

Java: s.split(",");  s.split("\\s+")
来源：http://xpn.chenlongwang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ynq.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://uzm.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hvg.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://ykk.vehdjk.com

Py:   ",".join(items)
来源：http://knn.cucudq.cn

PHP:  implode(",", $items);
来源：http://mmu.gaohongyu789.top

JS:   items.join(",")
来源：http://mev.hammf.cn

TS:   items.join(",")
来源：http://guo.yanxiufei.cn

Java: String.join(",", items)
来源：http://oix.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://bnr.havefunace.top

Ruby: items.join(",")
来源：http://erq.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://slu.xziqi.cn

[E09] 去除所有空白字符
来源：http://pwj.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://knk.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qmn.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://bqe.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://iwb.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://uvg.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qra.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://jww.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dct.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://ltw.hnqzz.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ffo.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ioi.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://chq.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://xrw.daxiang520.top

Java: String.format("%03d", 7)
来源：http://pac.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hdf.cashguo.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fdr.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wca.jinqigfzy.top

[E11] 反转字符串
来源：http://mbx.hcnkem.com

Py:   s[::-1]
来源：http://upj.52xcode.cn

PHP:  strrev($s);
来源：http://ctx.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://xsa.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://iig.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gmb.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zgj.guowangkeji.top

Ruby: s.reverse
来源：http://uni.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://yts.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://ghj.dashuyun.cn

Py:   s.count("a")
来源：http://smg.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://evq.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://tnv.316326.xyz

TS:   s.split("a").length - 1
来源：http://ajx.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ied.sweek.top

Go:   strings.Count(s, "a")
来源：http://ajr.yuxming.cn

Ruby: s.count("a")
来源：http://qds.guannengcc.top

C#:   s.Count(c => c == 'a')
来源：http://ufv.fzhhl.top

[E13] 逐字符遍历
来源：http://hfe.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://blq.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mhm.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qoy.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://epc.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fox.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rgj.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lvb.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhf.wangdashe.top

[E14] URL 编码与 Base64
来源：http://psx.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hnp.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zyt.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqp.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yxv.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vso.gaohongyu789.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cwl.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://alb.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tjg.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://vjn.fanxiaobao.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://aza.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ejj.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pos.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://izp.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yvx.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rwu.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vtj.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ywz.yfazqb.com

[E16] 数字千分位
来源：http://nac.aizwys.cn

Py:   f"{1234567:,}"
来源：http://iwz.uphjek.com

PHP:  number_format(1234567);
来源：http://wxb.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cie.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yji.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gdf.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iln.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jam.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://lhc.zdbjq.cn

[E17] 首字母大写
来源：http://vqi.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://stg.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qzb.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nzs.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ugo.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nue.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yne.hammf.cn

Ruby: s.capitalize
来源：http://dnt.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rjn.daxiang520.top

[E18] 模板占位符替换
来源：http://gws.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xiw.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzo.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hrc.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://isd.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pzb.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jma.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kkh.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bip.cucudq.cn

[E19] 多行文本按行拆分
来源：http://hto.ydzc1.top

Py:   s.splitlines()
来源：http://smi.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mdh.jinghuilouyu.cn

JS:   s.split(/\r?\n/)
来源：http://zsk.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://vky.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://mzd.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://bia.316326.xyz

Ruby: s.lines
来源：http://hrb.zhixingplan.top

C#:   s.Split('\n')
来源：http://gvm.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://gqx.zdqjudy.top

Py:   if not s:
来源：http://rof.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xbq.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zky.hnqzz.top

TS:   if (s === "") {}
来源：http://ipn.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://qfu.jyoumei.cn


<!-- 参考信息 -->