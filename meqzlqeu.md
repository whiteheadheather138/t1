代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://cmj.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://phb.shanyushiyangkeji.top

[D09] 排序（升序）
来源：http://qmg.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://wio.yj202588.top

PHP:  sort($arr);
来源：http://csi.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jnm.gotoacloud.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://taj.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zdd.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qql.svipenyu.cn

Ruby: arr.sort
来源：http://dms.jyoumei.cn

C#:   list.Sort();
来源：http://bvv.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lmt.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kyu.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tta.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jbc.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://khw.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qiw.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ikw.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xkt.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wfz.hnxiangtu.top

[D11] 反转数组
来源：http://vsw.yueranfly.top

Py:   arr[::-1];  arr.reverse()
来源：http://loq.uphjek.com

PHP:  array_reverse($arr);
来源：http://vnr.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fnx.snrcjt.cn

TS:   [...arr].reverse();
来源：http://vqe.fktsv.cn

Java: Collections.reverse(list);
来源：http://nbr.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://yma.pengpengdd.cyou

Ruby: arr.reverse
来源：http://sll.redwolf501.top

C#:   list.Reverse();
来源：http://hon.jlsjyb.cn

[D12] 查找元素下标
来源：http://uog.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://qys.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lmf.iojbl.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mtt.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oqy.yfazqb.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oyo.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://duf.gaohongyu789.top

Ruby: arr.index(x)
来源：http://uza.jiagoushi.top

C#:   list.IndexOf(x);
来源：http://pgb.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://ivr.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mza.chenlongwang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qon.zhongyouzk.top

JS:   arr.filter(x => x > 3)
来源：http://kyr.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://dmt.nwbrower.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yvs.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hef.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://ilh.tianlin.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://mlf.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://phy.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pwh.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ijh.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://gai.c1oappe.top

TS:   arr.map(x => x * 2)
来源：http://ngj.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://xuz.xziqi.cn

Go:   // 手写循环
来源：http://fyc.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ybc.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://clq.yangfankeji.com

[D15] 去重
来源：http://hja.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aod.sweek.top

PHP:  array_unique($arr);
来源：http://pip.vehdjk.com

JS:   [...new Set(arr)]
来源：http://tjl.xziqi.cn

TS:   [...new Set(arr)]
来源：http://ese.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rwq.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fhf.bjfxy.top

Ruby: arr.uniq
来源：http://sfh.jinghuilouyu.cn

C#:   list.Distinct().ToList()
来源：http://kyu.316326.xyz

[D16] 求和与平均值
来源：http://sws.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cme.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iqs.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ter.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xak.mhx1999.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dxd.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://hvz.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lhj.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://plx.cheryme.top

[D17] 最大值与最小值
来源：http://xzq.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://gsb.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://nbv.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://paz.epnwcf.com

TS:   Math.max(...arr);
来源：http://uiy.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://awg.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zzo.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://fvs.ivvv.top

C#:   list.Max();  list.Min()
来源：http://vwq.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://wou.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qbq.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://kgh.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uoq.fktsv.cn

TS:   nested.flat();
来源：http://bff.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sbw.gaohongyu789.top

Go:   // 手写双层循环
来源：http://nib.daxiang520.top

Ruby: nested.flatten
来源：http://lmf.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qsm.kuanghao11.cn

[D19] 按字段分组
来源：http://coq.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://znc.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://edg.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://huc.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bnc.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oef.sjlbkw.cn

Go:   // 手写 map[string][]T
来源：http://lvq.ivvv.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vmz.epnwcf.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qei.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://mqp.shzxlz.cn

Py:   Counter(arr)
来源：http://dvm.mhx1999.top

PHP:  array_count_values($arr);
来源：http://xfk.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ima.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ngv.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jnh.xylfe.cn

Go:   // 手写 map[T]int
来源：http://dsp.havefunace.top

Ruby: arr.tally
来源：http://tsm.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jko.aizwys.cn

[D21] 判断是否包含某元素
来源：http://iwo.yanxiufei.cn

Py:   x in arr
来源：http://dla.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://bkd.kuanghao11.cn

JS:   arr.includes(x)
来源：http://mqm.zdbjq.cn

TS:   arr.includes(x)
来源：http://duy.daria6918.cn

Java: list.contains(x)
来源：http://nmw.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://orn.cdnleiting.top

Ruby: arr.include?(x)
来源：http://beh.tanke756.top

C#:   list.Contains(x)
来源：http://pgr.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://qga.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://npn.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sgj.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dwm.ybcxt.top

TS:   [...arr];
来源：http://okg.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://rae.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://cju.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://csv.yuanzhike.top

C#:   new List<int>(list);
来源：http://ddp.zhixingplan.top

[D23] reduce 累积计算
来源：http://nli.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vyc.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lvj.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfg.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bou.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dqx.mhx1999.top

Go:   // 手写循环
来源：http://mqh.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pol.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pat.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://wbw.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://svg.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ear.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mza.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xxa.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yyp.9152youxi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://czr.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rqh.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hpe.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://ixo.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://shg.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mnx.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jfj.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xnc.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yme.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://spj.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kjz.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sib.hywenlv.cn

[D26] 数组转字符串
来源：http://lca.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://cim.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://xrc.dianchejie.cn

JS:   arr.join(", ")
来源：http://com.fehbvm.com

TS:   arr.join(", ")
来源：http://bof.gogol.net.cn

Java: String.join(", ", list)
来源：http://ziz.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://olm.yonumen.top

Ruby: arr.join(", ")
来源：http://rcg.cheryme.top

C#:   string.Join(", ", list)
来源：http://akv.yvedp.cn

================================================================================
来源：http://ecy.sweek.top

E. 字符串处理
来源：http://caw.guannengcc.top

================================================================================
来源：http://bmj.shangyingyoupin.top

[E01] 拼接字符串
来源：http://ezn.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lzb.316326.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zeq.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ous.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qav.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nbk.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oug.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kqf.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ncs.vqdsnc.cn

[E02] 重复字符串
来源：http://fnp.zhengqikj.top

Py:   "ab" * 3
来源：http://pod.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://qaq.wangdashe.top

JS:   "ab".repeat(3)
来源：http://ytn.hammf.cn

TS:   "ab".repeat(3)
来源：http://puu.sufxvd.cn

Java: "ab".repeat(3)
来源：http://xjx.jinqigfzy.top

Go:   strings.Repeat("ab", 3)
来源：http://bxj.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://xig.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qmf.hesvh.cn

[E03] 截取子串
来源：http://eqi.fengsongda.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://leo.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uza.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kae.tanke756.top

TS:   s.slice(1, 4)
来源：http://haw.chenzaomai.com

Java: s.substring(1, 4)
来源：http://ksn.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://odr.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cds.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://xku.jinqigufen.top

[E04] 查找子串位置
来源：http://gaq.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://dgp.xuetiantiany.cn

PHP:  strpos($s, "x");
来源：http://xpj.birdmap.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://scp.snrcjt.cn

TS:   s.indexOf("x")
来源：http://tyn.fzhhl.top

Java: s.indexOf("x")
来源：http://gqd.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://yzu.c1oappe.top

Ruby: s.index("x")
来源：http://xsg.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://rja.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gwh.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://whc.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ydm.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bte.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bix.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ckv.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://twb.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xbq.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pzi.bjfxy.top

[E06] 替换子串
来源：http://jcs.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ezq.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://zpv.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yfo.zhongyouzk.top

TS:   s.replaceAll("a", "b")
来源：http://kse.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zcw.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wqm.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://avi.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://syh.ehwqpu.com

[E07] 按分隔符拆分
来源：http://pgk.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://knv.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yin.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oew.316326.xyz

TS:   s.split(",")
来源：http://kfx.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://lbu.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://guz.316326.xyz

Ruby: s.split(",");  s.split
来源：http://xla.sufxvd.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://icl.xziqi.cn

[E08] 数组按分隔符合并
来源：http://jgj.jqgfzy.top

Py:   ",".join(items)
来源：http://mgl.sysykeji.top

PHP:  implode(",", $items);
来源：http://gby.guannengcc.top

JS:   items.join(",")
来源：http://xcm.tarul.cn

TS:   items.join(",")
来源：http://mii.fehbvm.com

Java: String.join(",", items)
来源：http://xhc.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://wgu.chenzaomai.com

Ruby: items.join(",")
来源：http://vqu.mhx1999.top

C#:   string.Join(",", items)
来源：http://evl.xziqi.cn

[E09] 去除所有空白字符
来源：http://uyt.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wnh.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jia.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://wjd.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ovy.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://esn.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://llr.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://eqt.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wlr.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://apn.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iub.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qll.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://aex.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://dkq.yueranfly.top

Java: String.format("%03d", 7)
来源：http://ehn.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bdd.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zyo.meibo888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vob.fktsv.cn

[E11] 反转字符串
来源：http://vqz.zhoulong.xyz

Py:   s[::-1]
来源：http://rjj.yj202588.top

PHP:  strrev($s);
来源：http://blg.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://tjl.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://clu.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lov.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ohc.hnxiangtu.top

Ruby: s.reverse
来源：http://eic.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nfb.wangdashe.top

[E12] 统计某字符出现次数
来源：http://sjs.jianghu66.top

Py:   s.count("a")
来源：http://hmx.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://erl.yj20258888.top

JS:   s.split("a").length - 1
来源：http://lig.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://xby.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ctr.tanke756.top

Go:   strings.Count(s, "a")
来源：http://aqz.cdnleiting.top

Ruby: s.count("a")
来源：http://roc.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://upg.tarul.cn

[E13] 逐字符遍历
来源：http://enx.jyoumei.cn

Py:   for ch in s: print(ch)
来源：http://dqd.xuetiantiany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nxx.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qip.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vxq.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kkx.yfazqb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://whg.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://egt.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gjk.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://fsh.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mhz.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ptr.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://abn.dashuyun.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ref.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cji.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vju.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bct.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gyb.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://sle.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://wjz.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gsw.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://roe.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://qpi.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bza.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pdf.zhiwuduotai.top


<!-- 参考信息 -->