代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://eun.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://stc.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://obc.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://hqq.gaohongyu789.top

PHP:  sort($arr);
来源：http://bsd.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xoq.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://aca.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uhq.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ldy.sweek.top

Ruby: arr.sort
来源：http://bar.ivvv.top

C#:   list.Sort();
来源：http://sie.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rrm.hfpthk.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tcd.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://utp.aibaodan.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rcb.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkp.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lsm.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qro.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vcp.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xin.svipenyu.cn

[D11] 反转数组
来源：http://zco.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mkt.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://vve.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://npc.andypj.xyz

TS:   [...arr].reverse();
来源：http://adc.tianlin.xyz

Java: Collections.reverse(list);
来源：http://nna.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://qgx.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://prh.hysaishi.cn

C#:   list.Reverse();
来源：http://mza.tarul.cn

[D12] 查找元素下标
来源：http://vgt.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://efh.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uhk.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bqf.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ocz.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tat.ivvv.top

Go:   slices.Index(arr, x)
来源：http://fmo.hcnkem.com

Ruby: arr.index(x)
来源：http://mxh.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://qae.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://xnr.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qee.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bbc.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://fga.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://mmc.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fuy.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nob.hfpthk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hub.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://txd.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://pnh.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xrm.shzxlz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sxr.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://wcy.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://pgo.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://prv.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://tfa.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://pbx.yj20258.top

C#:   list.Select(x => x * 2).ToList()
来源：http://viq.sxryk.cn

[D15] 去重
来源：http://dpq.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://svb.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://efy.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://mcf.jyoumei.cn

TS:   [...new Set(arr)]
来源：http://sdm.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sbb.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://lti.mhx1999.top

Ruby: arr.uniq
来源：http://zsq.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://cwp.feifeiyinyue.top

[D16] 求和与平均值
来源：http://zxk.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rig.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fkl.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://igg.ywan-chungtsiang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://glv.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://drr.nwbrower.top

Go:   // 手写循环累加
来源：http://tiu.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gtr.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://ado.9152youxi.cn

[D17] 最大值与最小值
来源：http://rnj.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://wle.sxryk.cn

PHP:  max($arr);  min($arr);
来源：http://poa.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zep.feifeiyinyue.top

TS:   Math.max(...arr);
来源：http://ufd.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://roj.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ygz.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://dmv.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://tpz.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://eun.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ssy.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://cjm.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbc.aizwys.cn

TS:   nested.flat();
来源：http://ale.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pxt.tian-w.cn

Go:   // 手写双层循环
来源：http://npz.gaohongyu789.top

Ruby: nested.flatten
来源：http://eyf.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yhe.hywenlv.cn

[D19] 按字段分组
来源：http://cwo.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dvz.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bqd.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://clk.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ayg.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jwr.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://axg.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://uer.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ije.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://uvb.tian-w.cn

Py:   Counter(arr)
来源：http://fdd.zycfv.cn

PHP:  array_count_values($arr);
来源：http://qwq.tianlin.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqn.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nna.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pad.xylfe.cn

Go:   // 手写 map[T]int
来源：http://lue.jinqigufen.top

Ruby: arr.tally
来源：http://hyl.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hgl.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://smj.tarul.cn

Py:   x in arr
来源：http://wpy.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://rgp.gzhubu.top

JS:   arr.includes(x)
来源：http://czl.shzxlz.cn

TS:   arr.includes(x)
来源：http://nqh.fktsv.cn

Java: list.contains(x)
来源：http://ocq.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://bdw.ivvv.top

Ruby: arr.include?(x)
来源：http://hux.xuanzx.com

C#:   list.Contains(x)
来源：http://com.9152youxi.cn

[D22] 复制数组（避免共享引用）
来源：http://azq.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xsw.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jva.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aku.hcnkem.com

TS:   [...arr];
来源：http://dby.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://puy.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tcl.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://jsf.sweek.top

C#:   new List<int>(list);
来源：http://npc.ehwqpu.com

[D23] reduce 累积计算
来源：http://dxk.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ihd.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rfi.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bsp.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dsv.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://lug.svipenyu.cn

Go:   // 手写循环
来源：http://lad.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lul.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fzr.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://dvw.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vgp.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fye.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svi.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://afn.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ufw.xziqi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://heh.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ykr.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jar.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://hif.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://emo.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vai.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://whj.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://brc.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hmo.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kmj.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ozt.aibaodan.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gml.jqgufenzy.top

[D26] 数组转字符串
来源：http://ryt.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://vcv.tarul.cn

PHP:  implode(", ", $arr);
来源：http://gmr.yj20258888.top

JS:   arr.join(", ")
来源：http://ifz.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://wsy.vehdjk.com

Java: String.join(", ", list)
来源：http://cob.iojbl.cn

Go:   strings.Join(strs, ", ")
来源：http://xiw.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://qzg.ydjk.org.cn

C#:   string.Join(", ", list)
来源：http://pmn.jinqigfzy.top

================================================================================
来源：http://lfi.yvedp.cn

E. 字符串处理
来源：http://est.jianghu66.top

================================================================================
来源：http://blz.zhijiandao.cn

[E01] 拼接字符串
来源：http://ruw.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aue.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rps.hnqzz.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jqi.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://plu.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://peo.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://czq.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rpx.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fhu.tanke756.top

[E02] 重复字符串
来源：http://jcu.guowangkeji.top

Py:   "ab" * 3
来源：http://bmc.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://jnl.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://deg.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://ekt.ctjpmb.com

Java: "ab".repeat(3)
来源：http://uht.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://axi.vehdjk.com

Ruby: "ab" * 3
来源：http://sxn.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wbr.yonumen.top

[E03] 截取子串
来源：http://adx.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://egy.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kfw.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ocm.sweek.top

TS:   s.slice(1, 4)
来源：http://rld.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://gvs.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gki.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://dds.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://xhp.guowangkeji.top

[E04] 查找子串位置
来源：http://wtg.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://lae.mhx1999.top

PHP:  strpos($s, "x");
来源：http://qdj.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eyl.pycfn.com

TS:   s.indexOf("x")
来源：http://nei.hnqzz.top

Java: s.indexOf("x")
来源：http://xtx.jqgfzy.top

Go:   strings.Index(s, "x")
来源：http://lif.smart0.xyz

Ruby: s.index("x")
来源：http://zlt.wangdashe.top

C#:   s.IndexOf("x")
来源：http://zjy.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zrs.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://itx.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wmx.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mba.ydzc1.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ejj.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dqr.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pei.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zng.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vwk.zhongyouzk.top

[E06] 替换子串
来源：http://xsa.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bqo.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://guj.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sth.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://dce.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ewa.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qwl.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uuq.nanxuanxn.top

C#:   s.Replace("a", "b")
来源：http://goz.yj202588.top

[E07] 按分隔符拆分
来源：http://osj.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://idu.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zwv.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eva.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://bzr.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://vfj.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gok.hcnkem.com

Ruby: s.split(",");  s.split
来源：http://aui.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tnp.xziqi.cn

[E08] 数组按分隔符合并
来源：http://lkt.jqgufenzy.top

Py:   ",".join(items)
来源：http://rjc.9152youxi.cn

PHP:  implode(",", $items);
来源：http://xmv.jqgfzy.top

JS:   items.join(",")
来源：http://yxl.jianghu66.top

TS:   items.join(",")
来源：http://pha.dashuyun.cn

Java: String.join(",", items)
来源：http://omo.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://bde.gaohongyu789.top

Ruby: items.join(",")
来源：http://spv.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://ybu.daria6918.cn

[E09] 去除所有空白字符
来源：http://qjg.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ykb.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cev.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://bxz.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://uui.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://tdi.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wbj.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://pzy.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uzu.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://eir.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ofh.tarul.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jan.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://tzf.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://mcy.pycfn.com

Java: String.format("%03d", 7)
来源：http://ncm.ydjk.org.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lno.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mjx.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mtj.gotoacloud.top

[E11] 反转字符串
来源：http://kxl.yj20258888.top

Py:   s[::-1]
来源：http://byc.tian-w.cn

PHP:  strrev($s);
来源：http://sze.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://tkz.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://gkr.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jdr.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rfv.gotoacloud.top

Ruby: s.reverse
来源：http://ezy.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://tjc.svipenyu.cn

[E12] 统计某字符出现次数
来源：http://ktb.hcnkem.com

Py:   s.count("a")
来源：http://kgq.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://ldc.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://vce.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://pru.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ess.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://jih.nwbrower.top

Ruby: s.count("a")
来源：http://gry.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://vek.sjlbkw.cn

[E13] 逐字符遍历
来源：http://xne.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://hrg.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gjf.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lrh.epnwcf.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://lyt.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bah.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcq.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://vjj.gogol.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gcn.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://bau.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nbp.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jor.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hjm.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://njy.sxryk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oxl.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wua.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://asc.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blf.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://rnd.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yqr.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bdb.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sdn.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kns.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mqs.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qub.redwolf501.top


<!-- 参考信息 -->