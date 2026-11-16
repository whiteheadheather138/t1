代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dyl.wangdashe.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qns.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wip.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ixs.hywenlv.cn

[D11] 反转数组
来源：http://sdl.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://elc.uphjek.com

PHP:  array_reverse($arr);
来源：http://pvg.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mcg.xylfe.cn

TS:   [...arr].reverse();
来源：http://khp.ivvv.top

Java: Collections.reverse(list);
来源：http://xfm.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://aad.zycfv.cn

Ruby: arr.reverse
来源：http://vhl.epnwcf.com

C#:   list.Reverse();
来源：http://gxi.xuanzx.com

[D12] 查找元素下标
来源：http://mzy.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://adv.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dby.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bzq.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fsh.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wcr.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://azh.pycfn.com

Ruby: arr.index(x)
来源：http://nxy.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://hvk.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://khi.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://npr.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://anq.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://ibk.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://vcw.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ftd.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rjh.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gfc.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vup.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://dro.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://awm.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sre.uphjek.com

JS:   arr.map(x => x * 2)
来源：http://ydc.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://nej.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ace.xylfe.cn

Go:   // 手写循环
来源：http://fgx.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://aty.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://mtm.hnqzz.top

[D15] 去重
来源：http://pjt.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ioi.chenlongwang.top

PHP:  array_unique($arr);
来源：http://yvb.fehbvm.com

JS:   [...new Set(arr)]
来源：http://icw.tian-w.cn

TS:   [...new Set(arr)]
来源：http://zbj.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lrm.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://omp.nanxinkj.top

Ruby: arr.uniq
来源：http://sir.yj202588.top

C#:   list.Distinct().ToList()
来源：http://hbo.gotoacloud.top

[D16] 求和与平均值
来源：http://sdp.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nvi.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uuj.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bhc.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fun.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://phr.xziqi.cn

Go:   // 手写循环累加
来源：http://mnw.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bhz.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://fsy.sufxvd.cn

[D17] 最大值与最小值
来源：http://dwj.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://mzt.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://vxm.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://alz.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://aiy.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tjb.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jjr.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://ems.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://umd.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://dak.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qbn.ctjpmb.com

PHP:  array_merge(...$nested);
来源：http://yts.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ffe.yongpay.top

TS:   nested.flat();
来源：http://fxw.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://way.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://pzb.ivvv.top

Ruby: nested.flatten
来源：http://avb.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xzs.cheryme.top

[D19] 按字段分组
来源：http://fyn.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://peh.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qci.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uai.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://inq.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dqx.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://ygw.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zxn.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ktv.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://cty.zhongyouzk.top

Py:   Counter(arr)
来源：http://ytj.aizwys.cn

PHP:  array_count_values($arr);
来源：http://xso.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://knr.yuanzhike.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oxc.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lcf.yonumen.top

Go:   // 手写 map[T]int
来源：http://wyo.nwbrower.top

Ruby: arr.tally
来源：http://yrj.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lna.tian-w.cn

[D21] 判断是否包含某元素
来源：http://dxs.0kj1m.cn

Py:   x in arr
来源：http://nid.xziqi.cn

PHP:  in_array($x, $arr, true);
来源：http://gqd.chenlongwang.top

JS:   arr.includes(x)
来源：http://hip.sweek.top

TS:   arr.includes(x)
来源：http://zzu.zycfv.cn

Java: list.contains(x)
来源：http://xaj.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://dhq.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://woi.chenzaomai.com

C#:   list.Contains(x)
来源：http://vqh.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://vyc.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oef.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://usy.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aur.ehwqpu.com

TS:   [...arr];
来源：http://vzi.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://oer.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://spw.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://tly.wangdashe.top

C#:   new List<int>(list);
来源：http://evw.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://fxp.nanxuanxn.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zzw.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mkb.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cgj.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjk.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dto.yanxiufei.cn

Go:   // 手写循环
来源：http://ydt.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bgc.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mpl.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://tce.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bfl.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ivj.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://npx.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zbg.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oca.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oqj.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jbk.aibaodan.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vnc.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://ogw.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lbc.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zvm.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ksn.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uze.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cci.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wps.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qal.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ljz.meibo888.top

[D26] 数组转字符串
来源：http://zeb.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://aic.yj20258.top

PHP:  implode(", ", $arr);
来源：http://uih.ydzc1.top

JS:   arr.join(", ")
来源：http://pxp.nwbrower.top

TS:   arr.join(", ")
来源：http://qqj.fehbvm.com

Java: String.join(", ", list)
来源：http://tkm.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://heb.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://byn.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://huv.ehwqpu.com

================================================================================
来源：http://euj.zdqjudy.top

E. 字符串处理
来源：http://cif.hcnkem.com

================================================================================
来源：http://tcy.uphjek.com

[E01] 拼接字符串
来源：http://ioa.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rkk.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ofk.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wac.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tiu.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aex.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://snf.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jad.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qte.yangfankeji.com

[E02] 重复字符串
来源：http://bvt.ydjk.org.cn

Py:   "ab" * 3
来源：http://jas.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://elh.xziqi.cn

JS:   "ab".repeat(3)
来源：http://nbz.316326.xyz

TS:   "ab".repeat(3)
来源：http://xjs.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://hag.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://pqw.cashguo.top

Ruby: "ab" * 3
来源：http://nyx.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ced.zhongyouzk.top

[E03] 截取子串
来源：http://xvs.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyq.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dca.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hag.iojbl.cn

TS:   s.slice(1, 4)
来源：http://kpa.yuanzhike.top

Java: s.substring(1, 4)
来源：http://lrv.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ubr.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://fud.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://pic.vehdjk.com

[E04] 查找子串位置
来源：http://mrh.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://nru.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://oyg.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kqs.guannengcc.top

TS:   s.indexOf("x")
来源：http://mtd.gotoacloud.top

Java: s.indexOf("x")
来源：http://nnn.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://rgw.hammf.cn

Ruby: s.index("x")
来源：http://vak.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://ocy.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kyz.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lrq.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mih.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vna.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vfo.yueranfly.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybw.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://olc.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mgy.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hce.fktsv.cn

[E06] 替换子串
来源：http://cou.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xpw.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://rwb.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cid.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://utg.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rhs.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jlb.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gls.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://miy.yueranfly.top

[E07] 按分隔符拆分
来源：http://eaj.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qda.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ovn.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gic.svipenyu.cn

TS:   s.split(",")
来源：http://zwy.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://umr.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ame.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://zpx.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://var.zycfv.cn

[E08] 数组按分隔符合并
来源：http://zfi.dashuyun.cn

Py:   ",".join(items)
来源：http://suo.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://iix.tarul.cn

JS:   items.join(",")
来源：http://ice.redwolf501.top

TS:   items.join(",")
来源：http://kuo.daxiang520.top

Java: String.join(",", items)
来源：http://rqe.zhoulong.xyz

Go:   strings.Join(items, ",")
来源：http://pcn.jiagoushi.top

Ruby: items.join(",")
来源：http://anv.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://pqk.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://jnj.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nqv.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://peq.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://igp.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://xds.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://rca.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://roo.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://kmx.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kgy.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://tgg.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hqd.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cta.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://qdp.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://thu.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://zfy.yongpay.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://plu.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ibl.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gcn.zhiwuduotai.top

[E11] 反转字符串
来源：http://ghg.pycfn.com

Py:   s[::-1]
来源：http://hwp.guowangkeji.top

PHP:  strrev($s);
来源：http://esg.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://gnw.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://muk.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://irt.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://exn.vqdsnc.cn

Ruby: s.reverse
来源：http://lyo.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://awz.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://pxj.gzhubu.top

Py:   s.count("a")
来源：http://yac.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://qio.52xcode.cn

JS:   s.split("a").length - 1
来源：http://ist.cheryme.top

TS:   s.split("a").length - 1
来源：http://pez.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vlm.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://gss.zhiwuduotai.top

Ruby: s.count("a")
来源：http://dpd.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://mcj.hesvh.cn

[E13] 逐字符遍历
来源：http://goz.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://qax.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tul.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xhv.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yss.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://neu.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xdh.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://klt.yongpay.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aiu.sweek.top

[E14] URL 编码与 Base64
来源：http://kuc.0kj1m.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gbx.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wuu.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pmt.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kba.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://leh.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eax.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ane.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uzx.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://bro.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fpl.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ekl.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://whz.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://lts.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rda.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ygg.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cls.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ncb.gzhubu.top

[E16] 数字千分位
来源：http://biu.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://yld.tanke756.top

PHP:  number_format(1234567);
来源：http://vae.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fsc.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://ier.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oah.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://znx.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vht.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://voe.shangyingyoupin.top

[E17] 首字母大写
来源：http://qjr.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uos.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://hxp.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uhe.316326.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iud.cashguo.top


<!-- 参考信息 -->