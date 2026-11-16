代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://trc.xuanzx.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mxp.birdmap.top

[D05] 访问与修改元素
来源：http://apb.wangdashe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bhf.hnxiangtu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eev.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lgy.bbcook.cn

TS:   arr[0]; arr.at(-1);
来源：http://wnl.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://fhl.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://dxd.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://efk.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nwr.tian-w.cn

[D06] 数组长度
来源：http://itr.ppjwa.cn

Py:   len(arr)
来源：http://znq.zhaomingkeji.xyz

PHP:  count($arr);
来源：http://rcz.zhoulong.xyz

JS:   arr.length
来源：http://wya.wangshuangyany.cn

TS:   arr.length
来源：http://mkd.dianchejie.cn

Java: list.size();
来源：http://oml.yuxming.cn

Go:   len(arr)
来源：http://jyw.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://wpo.yangfankeji.com

C#:   list.Count;
来源：http://gal.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://dmn.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vxj.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://trq.yuxming.cn

JS:   arr.slice(1, 4);
来源：http://wkb.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://oij.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://bnm.tanke756.top

Go:   arr[1:4]
来源：http://fqn.aibaodan.cn

Ruby: arr[1, 3]
来源：http://zag.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://ruv.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://jsi.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://ees.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://jtk.zhongyouzk.top

JS:   [...a, ...b];  a.concat(b);
来源：http://slb.epnwcf.com

TS:   [...a, ...b];
来源：http://upc.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oxe.hongshengwenyu.top

Go:   append(a, b...)
来源：http://fqn.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://aie.fengsongda.top

C#:   a.Concat(b).ToList()
来源：http://fmr.jianghu66.top

[D09] 排序（升序）
来源：http://uzt.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://atv.gogol.net.cn

PHP:  sort($arr);
来源：http://puj.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://com.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ghm.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lze.jqgufenzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sei.zhiwuduotai.top

Ruby: arr.sort
来源：http://xsf.guowangkeji.top

C#:   list.Sort();
来源：http://rce.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qgt.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gej.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pgu.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zlg.daria6918.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bqu.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ryk.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hgh.yj20258888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yxn.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tpa.wangdashe.top

[D11] 反转数组
来源：http://gii.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://yzr.tarul.cn

PHP:  array_reverse($arr);
来源：http://dcn.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yrx.daxiang520.top

TS:   [...arr].reverse();
来源：http://ocq.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://vtu.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://apo.ybcxt.top

Ruby: arr.reverse
来源：http://ijv.wangdashe.top

C#:   list.Reverse();
来源：http://bqo.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://twm.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://ihr.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://now.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqx.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kcx.birdmap.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xdx.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://cwd.jqgufenzy.top

Ruby: arr.index(x)
来源：http://gqr.9152youxi.cn

C#:   list.IndexOf(x);
来源：http://tvi.chenzaomai.com

[D13] 过滤（保留满足条件的）
来源：http://gyy.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oru.yangfankeji.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rui.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://gow.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://vsh.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fom.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fah.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://ehm.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tqz.guannengcc.top

[D14] 映射转换（每个元素变形）
来源：http://dsi.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sgk.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vhm.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://fxo.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://wwm.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vvk.zhiwuduotai.top

Go:   // 手写循环
来源：http://nus.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://huw.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xti.bjfxy.top

[D15] 去重
来源：http://fox.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lhl.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://ajo.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://kzu.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://vkx.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cdu.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://and.hfpthk.cn

Ruby: arr.uniq
来源：http://vsf.jiagoushi.top

C#:   list.Distinct().ToList()
来源：http://pag.jqgufenzy.top

[D16] 求和与平均值
来源：http://tnd.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qxo.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yoj.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwo.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://unw.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sdg.chenlongwang.top

Go:   // 手写循环累加
来源：http://owg.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://msy.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://qrw.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://wqi.ivvv.top

Py:   max(arr);  min(arr)
来源：http://uck.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://xvk.cqqwz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uqa.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://wwq.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://dbn.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gid.sweek.top

Ruby: arr.max;  arr.min
来源：http://bjd.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://bcw.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://sbs.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ufj.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://szg.tarul.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jma.shuidangran.top

TS:   nested.flat();
来源：http://czz.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ozz.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://lbq.zdqjudy.top

Ruby: nested.flatten
来源：http://aab.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rmf.cucudq.cn

[D19] 按字段分组
来源：http://nrt.ydzc1.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uhw.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mok.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gji.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zfg.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hjf.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://ohm.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ssd.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gxs.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://zyn.gzhubu.top

Py:   Counter(arr)
来源：http://npo.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://anm.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://laf.xziqi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nkf.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vsf.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://qmb.cucudq.cn

Ruby: arr.tally
来源：http://qmh.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jli.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://jnp.cqqwz.cn

Py:   x in arr
来源：http://jjx.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://rqy.tarul.cn

JS:   arr.includes(x)
来源：http://ilo.daria6918.cn

TS:   arr.includes(x)
来源：http://jmj.bbcook.cn

Java: list.contains(x)
来源：http://igi.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://tup.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://jxn.yueranfly.top

C#:   list.Contains(x)
来源：http://eqd.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://stl.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nla.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://izr.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fca.hnqzz.top

TS:   [...arr];
来源：http://pvx.hcnkem.com

Java: new ArrayList<>(list);
来源：http://xdt.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://jhm.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://ugr.cheryme.top

C#:   new List<int>(list);
来源：http://xsx.ctjpmb.com

[D23] reduce 累积计算
来源：http://orm.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dis.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qpt.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://myn.cucudq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vwx.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://njp.zycfv.cn

Go:   // 手写循环
来源：http://zfr.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rbo.gzhubu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rlt.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://lwh.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vzy.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://izk.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dep.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zub.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oek.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mlo.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sci.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pwx.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://ros.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gwe.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrg.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://swm.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mty.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rmi.pycfn.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://whd.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dcu.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xfr.cucudq.cn

[D26] 数组转字符串
来源：http://ezq.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://ipz.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://voq.hywenlv.cn

JS:   arr.join(", ")
来源：http://cny.jinqigufen.top

TS:   arr.join(", ")
来源：http://epw.jinqigfzy.top

Java: String.join(", ", list)
来源：http://xez.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://kow.yueranfly.top

Ruby: arr.join(", ")
来源：http://kfu.cashguo.top

C#:   string.Join(", ", list)
来源：http://njs.jyoumei.cn

================================================================================
来源：http://jmi.havefunace.top

E. 字符串处理
来源：http://zha.ehwqpu.com

================================================================================
来源：http://cgy.wangshuangyany.cn

[E01] 拼接字符串
来源：http://exm.nanxinkj.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ncv.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yws.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xcl.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://msu.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kxz.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rzh.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dvs.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wgc.hcnkem.com

[E02] 重复字符串
来源：http://xvg.jiagoushi.top

Py:   "ab" * 3
来源：http://ahs.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://nli.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://phy.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://hfa.hcnkem.com

Java: "ab".repeat(3)
来源：http://fhy.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://vfa.yonumen.top

Ruby: "ab" * 3
来源：http://etw.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uub.andypj.xyz

[E03] 截取子串
来源：http://dod.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ldg.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://elx.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jkn.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://qqp.cqqwz.cn

Java: s.substring(1, 4)
来源：http://amy.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://end.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uos.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://gtm.yonumen.top

[E04] 查找子串位置
来源：http://wgh.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://ben.sysykeji.top

PHP:  strpos($s, "x");
来源：http://zpd.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mkr.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://oll.nanxinkj.top

Java: s.indexOf("x")
来源：http://qdy.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://oty.316326.xyz

Ruby: s.index("x")
来源：http://zwx.hammf.cn

C#:   s.IndexOf("x")
来源：http://htk.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jpa.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://aff.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://psy.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sps.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://drd.52xcode.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ugo.svipenyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iss.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qnm.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvq.cashguo.top

[E06] 替换子串
来源：http://swn.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yih.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://fcg.yuanzhike.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qln.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://vqa.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgx.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ffx.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eiy.sweek.top

C#:   s.Replace("a", "b")
来源：http://pzf.dashuyun.cn

[E07] 按分隔符拆分
来源：http://oht.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rpt.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mjy.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://dnj.sxryk.cn

TS:   s.split(",")
来源：http://hgl.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qwn.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://muf.quarkkingdee.top

Ruby: s.split(",");  s.split
来源：http://wnu.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wla.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://eou.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://zdj.zdbjq.cn

PHP:  implode(",", $items);
来源：http://aeo.jinqigufen.top

JS:   items.join(",")
来源：http://yif.jinqigfzy.top

TS:   items.join(",")
来源：http://kui.tanke756.top

Java: String.join(",", items)
来源：http://enw.birdmap.top

Go:   strings.Join(items, ",")
来源：http://lma.wangdashe.top

Ruby: items.join(",")
来源：http://izl.xylfe.cn

C#:   string.Join(",", items)
来源：http://lta.sysykeji.top

[E09] 去除所有空白字符
来源：http://mvn.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ykm.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vli.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://ovt.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://raw.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://cuy.dianchejie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://grp.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://knc.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xyn.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://art.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bsy.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://azo.gaohongyu789.top

JS:   "7".padStart(3, "0")
来源：http://hma.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://xjq.wangdashe.top

Java: String.format("%03d", 7)
来源：http://ell.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://azi.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iys.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uzb.zhijiandao.cn

[E11] 反转字符串
来源：http://mlo.ivvv.top

Py:   s[::-1]
来源：http://qzw.yonumen.top

PHP:  strrev($s);
来源：http://zlv.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://jgc.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://ddj.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nqd.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fvp.vehdjk.com


<!-- 参考信息 -->