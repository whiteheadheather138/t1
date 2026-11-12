代发 wailian999

Ruby: arr.index(x)
来源：http://lnj.tianlin.xyz

C#:   list.IndexOf(x);
来源：http://vau.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://woy.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uzc.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gkr.9152youxi.cn

JS:   arr.filter(x => x > 3)
来源：http://sbn.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://wci.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aux.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ico.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://tfi.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ook.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://zby.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cqd.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dev.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://ekr.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://tnl.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://sit.jinqigfzy.top

Go:   // 手写循环
来源：http://izr.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gsg.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bsd.fzhhl.top

[D15] 去重
来源：http://atu.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pfd.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://nbh.tian-w.cn

JS:   [...new Set(arr)]
来源：http://biw.pengpengdd.cyou

TS:   [...new Set(arr)]
来源：http://jcb.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rjk.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wnc.wangdashe.top

Ruby: arr.uniq
来源：http://lqz.nwbrower.top

C#:   list.Distinct().ToList()
来源：http://thp.andypj.xyz

[D16] 求和与平均值
来源：http://rwk.kuanghao11.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kzd.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://juw.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yck.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yme.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oio.yangfankeji.com

Go:   // 手写循环累加
来源：http://oxx.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://grq.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://uhg.0kj1m.cn

[D17] 最大值与最小值
来源：http://lmk.jiagoushi.top

Py:   max(arr);  min(arr)
来源：http://lfk.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://zds.hesvh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ocn.hammf.cn

TS:   Math.max(...arr);
来源：http://xbf.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dvo.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nsc.havefunace.top

Ruby: arr.max;  arr.min
来源：http://bjc.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://ugm.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://wta.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fav.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://uhw.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ixl.nanxinkj.top

TS:   nested.flat();
来源：http://yyn.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kqt.nanxuanxn.top

Go:   // 手写双层循环
来源：http://kjr.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://syg.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://one.yuxming.cn

[D19] 按字段分组
来源：http://krx.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ouz.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fqz.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://son.redwolf501.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xrd.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nim.meibo888.top

Go:   // 手写 map[string][]T
来源：http://zxk.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tme.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zpa.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://rwu.zdbjq.cn

Py:   Counter(arr)
来源：http://tez.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://rju.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://edm.xylfe.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lnq.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lvr.xinyue.icu

Go:   // 手写 map[T]int
来源：http://nyh.nanxinkj.top

Ruby: arr.tally
来源：http://qav.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wrz.sxryk.cn

[D21] 判断是否包含某元素
来源：http://lhj.ybcxt.top

Py:   x in arr
来源：http://xuv.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://djk.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://lqf.iojbl.cn

TS:   arr.includes(x)
来源：http://djm.jyoumei.cn

Java: list.contains(x)
来源：http://ggl.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://qku.yvedp.cn

Ruby: arr.include?(x)
来源：http://dte.xziqi.cn

C#:   list.Contains(x)
来源：http://weg.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://jnj.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qwx.dashuyun.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sqg.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ped.ivvv.top

TS:   [...arr];
来源：http://gsv.hnqzz.top

Java: new ArrayList<>(list);
来源：http://moh.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wgt.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://sxs.yuxming.cn

C#:   new List<int>(list);
来源：http://hre.zycfv.cn

[D23] reduce 累积计算
来源：http://zvi.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://suc.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qvs.haohaochexian.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fmu.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ofd.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bmq.jlsjyb.cn

Go:   // 手写循环
来源：http://mwk.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xxe.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kxj.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://kvx.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hxf.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://szw.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wqk.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cmd.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sxx.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://riz.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aka.bbcook.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qbs.uphjek.com

[D25] Set 集合去重与交并差
来源：http://agk.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uks.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rlh.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://guw.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://scg.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ljn.52xcode.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ocm.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wsi.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://drn.yuanzhike.top

[D26] 数组转字符串
来源：http://hik.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://sju.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://ypm.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://bcq.yj20258888.top

TS:   arr.join(", ")
来源：http://wkw.yfazqb.com

Java: String.join(", ", list)
来源：http://dhj.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://xao.sysykeji.top

Ruby: arr.join(", ")
来源：http://gtb.fktsv.cn

C#:   string.Join(", ", list)
来源：http://nwj.sxryk.cn

================================================================================
来源：http://ble.zdqjudy.top

E. 字符串处理
来源：http://wtf.yvedp.cn

================================================================================
来源：http://ldh.0kj1m.cn

[E01] 拼接字符串
来源：http://yop.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lph.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://anp.jyoumei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvx.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://adt.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fmu.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lky.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://niw.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nfh.hysaishi.cn

[E02] 重复字符串
来源：http://ykb.daxiang520.top

Py:   "ab" * 3
来源：http://ecm.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://vlp.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://uwp.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://ece.sysykeji.top

Java: "ab".repeat(3)
来源：http://pfv.hfpthk.cn

Go:   strings.Repeat("ab", 3)
来源：http://avz.ydjk.org.cn

Ruby: "ab" * 3
来源：http://nsn.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aoe.jqgfzy.top

[E03] 截取子串
来源：http://tgd.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qna.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hrw.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://biv.meibo888.top

TS:   s.slice(1, 4)
来源：http://eek.yonumen.top

Java: s.substring(1, 4)
来源：http://plv.yueranfly.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmm.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ruk.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://iaq.yueranfly.top

[E04] 查找子串位置
来源：http://fdm.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://otm.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://acl.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://otn.tanke756.top

TS:   s.indexOf("x")
来源：http://izu.jinqigfzy.top

Java: s.indexOf("x")
来源：http://fhs.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://cxy.daria6918.cn

Ruby: s.index("x")
来源：http://ahs.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://wcv.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://aow.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wen.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nuw.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mss.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyy.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://znd.fktsv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yts.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rwu.ivvv.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qgz.gzhubu.top

[E06] 替换子串
来源：http://luh.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ect.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://xau.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bfe.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://sqt.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mps.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nmr.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://djo.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://mfi.xinyue.icu

[E07] 按分隔符拆分
来源：http://jrn.smart0.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uwc.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://flt.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lzk.wangshuangyany.cn

TS:   s.split(",")
来源：http://byt.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://iyp.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yfb.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://tca.xziqi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pkx.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://emk.meibo888.top

Py:   ",".join(items)
来源：http://lve.sxryk.cn

PHP:  implode(",", $items);
来源：http://hkg.yangfankeji.com

JS:   items.join(",")
来源：http://bpy.guowangkeji.top

TS:   items.join(",")
来源：http://wiv.mhx1999.top

Java: String.join(",", items)
来源：http://hwq.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://tmy.nanxuanxn.top

Ruby: items.join(",")
来源：http://njr.bbcook.cn

C#:   string.Join(",", items)
来源：http://pmk.andypj.xyz

[E09] 去除所有空白字符
来源：http://cnd.yongpay.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kzc.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://twc.jqgfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://sxk.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://eck.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://onf.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yem.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mhe.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jhw.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://qfj.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xob.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bji.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://awn.guannengcc.top

TS:   "7".padStart(3, "0")
来源：http://ivv.uphjek.com

Java: String.format("%03d", 7)
来源：http://zdn.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lof.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ynl.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xyf.wangdashe.top

[E11] 反转字符串
来源：http://qys.shangyingyoupin.top

Py:   s[::-1]
来源：http://bpa.bjfxy.top

PHP:  strrev($s);
来源：http://grf.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://nto.hammf.cn

TS:   [...s].reverse().join("")
来源：http://whi.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uqv.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://izt.xuetiantiany.cn

Ruby: s.reverse
来源：http://dgx.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://asv.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://day.fzhhl.top

Py:   s.count("a")
来源：http://mei.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://ksi.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://kcu.fanxiaobao.xyz

TS:   s.split("a").length - 1
来源：http://swn.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bsr.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://gen.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://dur.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://srj.bbcook.cn

[E13] 逐字符遍历
来源：http://skz.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://ikh.cheryme.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kjo.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wql.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://vkx.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kzk.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hdg.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sjc.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://puc.sweek.top

[E14] URL 编码与 Base64
来源：http://nwx.cucudq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ohp.zhiwuduotai.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gjq.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://icn.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gxf.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iky.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vkq.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bgk.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yys.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://gkp.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zse.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tfo.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://onz.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://sbx.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ybs.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fpv.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://euz.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kcs.jqgufenzy.top

[E16] 数字千分位
来源：http://rev.sweek.top

Py:   f"{1234567:,}"
来源：http://zep.guannengcc.top

PHP:  number_format(1234567);
来源：http://fua.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://lqu.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vyg.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fmb.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tzf.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://apx.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://xsm.svipenyu.cn

[E17] 首字母大写
来源：http://qbn.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://myw.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kmk.zhixingplan.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xms.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uuz.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wpy.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jzo.dianchejie.cn

Ruby: s.capitalize
来源：http://rel.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://haq.yangfankeji.com

[E18] 模板占位符替换
来源：http://rmy.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dod.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iic.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eln.epnwcf.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gfo.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cym.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lji.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gbo.xingfuxueyuan.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tkh.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://mqo.yanxiufei.cn

Py:   s.splitlines()
来源：http://xwi.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gae.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://kyo.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://qog.yanxiufei.cn

Java: s.lines().toList()
来源：http://hqv.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://pxb.gogol.net.cn


<!-- 参考信息 -->