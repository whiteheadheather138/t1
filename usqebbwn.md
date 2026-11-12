代发 wailian999

Java: list.size();
来源：http://xlo.tarul.cn

Go:   len(arr)
来源：http://hrk.yj20258.top

Ruby: arr.length; arr.size
来源：http://jzb.sysykeji.top

C#:   list.Count;
来源：http://ity.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://vqf.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tzo.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://yyb.pycfn.com

JS:   arr.slice(1, 4);
来源：http://odz.gogol.net.cn

TS:   arr.slice(1, 4);
来源：http://qnk.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://nla.fengsongda.top

Go:   arr[1:4]
来源：http://kvk.pycfn.com

Ruby: arr[1, 3]
来源：http://ibf.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://puu.yanxiufei.cn

[D08] 合并两个数组
来源：http://pdj.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://izk.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://lkv.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://feh.cqqwz.cn

TS:   [...a, ...b];
来源：http://kvk.hesvh.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wnw.guowangkeji.top

Go:   append(a, b...)
来源：http://mmk.birdmap.top

Ruby: a + b;  a.concat(b)
来源：http://ilo.bjfxy.top

C#:   a.Concat(b).ToList()
来源：http://kqr.nanxinkj.top

[D09] 排序（升序）
来源：http://ahf.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://zpz.svipenyu.cn

PHP:  sort($arr);
来源：http://ufm.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://haw.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ksr.jinqigfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eut.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lxs.jlsjyb.cn

Ruby: arr.sort
来源：http://mpg.fktsv.cn

C#:   list.Sort();
来源：http://xqf.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ghr.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://akk.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lxy.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yvq.cqqwz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyb.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hpb.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zhc.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pfn.fehbvm.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nde.jinghuilouyu.cn

[D11] 反转数组
来源：http://qjo.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://iia.ydjk.org.cn

PHP:  array_reverse($arr);
来源：http://smw.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ago.xuanzx.com

TS:   [...arr].reverse();
来源：http://ljv.hnxiangtu.top

Java: Collections.reverse(list);
来源：http://xsx.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://hrd.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://jmj.smart0.xyz

C#:   list.Reverse();
来源：http://ekl.yj202588.top

[D12] 查找元素下标
来源：http://uso.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://vpm.zhijiandao.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fma.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjc.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcb.aizwys.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tdw.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://qzi.tianlin.xyz

Ruby: arr.index(x)
来源：http://swu.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://eqp.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://mik.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lds.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qhm.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://xcx.52xcode.cn

TS:   arr.filter(x => x > 3)
来源：http://jhl.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ran.zhengqikj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wvh.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://wix.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fkt.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://zce.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yvj.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://htd.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://lez.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://rdc.tianlin.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://emt.meibo888.top

Go:   // 手写循环
来源：http://xxs.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://svk.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jwr.nwbrower.top

[D15] 去重
来源：http://qbd.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iod.yfazqb.com

PHP:  array_unique($arr);
来源：http://kuc.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://gmx.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://jtm.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vdp.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cwd.redwolf501.top

Ruby: arr.uniq
来源：http://vkj.pycfn.com

C#:   list.Distinct().ToList()
来源：http://gxu.zhoulong.xyz

[D16] 求和与平均值
来源：http://jvf.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yxj.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qja.ywan-chungtsiang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uem.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iot.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogn.dashuyun.cn

Go:   // 手写循环累加
来源：http://ogs.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bwm.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://mgv.hesvh.cn

[D17] 最大值与最小值
来源：http://nbz.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://lhi.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://jfd.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://egv.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://syh.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rlh.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pcs.zhiwuduotai.top

Ruby: arr.max;  arr.min
来源：http://ifc.cashguo.top

C#:   list.Max();  list.Min()
来源：http://ahb.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://gyx.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xyx.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://xbt.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mzg.daxiang520.top

TS:   nested.flat();
来源：http://eio.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bme.bbcook.cn

Go:   // 手写双层循环
来源：http://qbp.yanxiufei.cn

Ruby: nested.flatten
来源：http://kef.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xex.svipenyu.cn

[D19] 按字段分组
来源：http://tgb.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://csn.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://anu.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wjr.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zwk.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://szj.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://dym.jqgfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://prd.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nzq.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://rjg.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://rqe.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://epv.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gkd.tarul.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cih.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nge.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://urd.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://nfr.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zbb.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://hdg.chenlongwang.top

Py:   x in arr
来源：http://hoe.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://hsi.havefunace.top

JS:   arr.includes(x)
来源：http://pdl.jinqigufen.top

TS:   arr.includes(x)
来源：http://stv.fanxiaobao.xyz

Java: list.contains(x)
来源：http://iia.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://pqa.tianlin.xyz

Ruby: arr.include?(x)
来源：http://coj.zdqjudy.top

C#:   list.Contains(x)
来源：http://lgw.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://xrn.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hfp.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ppn.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zlu.jinqigufen.top

TS:   [...arr];
来源：http://pkd.yongpay.top

Java: new ArrayList<>(list);
来源：http://ymd.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://ass.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://hmg.gotoacloud.top

C#:   new List<int>(list);
来源：http://kbd.jianghu66.top

[D23] reduce 累积计算
来源：http://vxq.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ubb.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xgy.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://txk.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bfs.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wtt.cheryme.top

Go:   // 手写循环
来源：http://jqj.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bsk.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://flu.shanyushiyangkeji.top

[D24] 字典 / Map 基本操作
来源：http://ejt.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mkn.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vnr.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gyj.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fev.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://thi.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zwr.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rxe.jqgufenzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pbi.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://nko.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qzg.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ils.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fwb.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mtl.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uyk.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xii.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cel.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mxz.ppjwa.cn

[D26] 数组转字符串
来源：http://lka.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://mgz.daxiang520.top

PHP:  implode(", ", $arr);
来源：http://abk.daria6918.cn

JS:   arr.join(", ")
来源：http://loc.hnxiangtu.top

TS:   arr.join(", ")
来源：http://ksq.gzhubu.top

Java: String.join(", ", list)
来源：http://tpt.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://avp.ivvv.top

Ruby: arr.join(", ")
来源：http://hhf.andypj.xyz

C#:   string.Join(", ", list)
来源：http://zqu.fengsongda.top

================================================================================
来源：http://xjo.zhengqikj.top

E. 字符串处理
来源：http://gfg.hysaishi.cn

================================================================================
来源：http://lwm.dashuyun.cn

[E01] 拼接字符串
来源：http://ppu.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ika.hnqzz.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://twx.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hhb.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://opk.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jyq.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fcf.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uls.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://npo.nanxinkj.top

[E02] 重复字符串
来源：http://sxg.c1oappe.top

Py:   "ab" * 3
来源：http://poh.jyoumei.cn

PHP:  str_repeat("ab", 3);
来源：http://vjf.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://ntu.sxryk.cn

TS:   "ab".repeat(3)
来源：http://zgl.xylfe.cn

Java: "ab".repeat(3)
来源：http://pra.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://vcq.ydjk.org.cn

Ruby: "ab" * 3
来源：http://zqs.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kyn.hesvh.cn

[E03] 截取子串
来源：http://miz.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://khc.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cxm.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://igq.fengsongda.top

TS:   s.slice(1, 4)
来源：http://voj.vehdjk.com

Java: s.substring(1, 4)
来源：http://xhm.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aln.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://cbr.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://hrf.fzhhl.top

[E04] 查找子串位置
来源：http://otw.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://qzh.daxiang520.top

PHP:  strpos($s, "x");
来源：http://zuu.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lzw.vehdjk.com

TS:   s.indexOf("x")
来源：http://tiw.yueranfly.top

Java: s.indexOf("x")
来源：http://dvt.xziqi.cn

Go:   strings.Index(s, "x")
来源：http://puh.kuanghao11.cn

Ruby: s.index("x")
来源：http://xkq.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://xks.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://onx.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qzx.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://llb.9152youxi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bbm.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kez.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zrb.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zoy.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fbo.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbr.jiagoushi.top

[E06] 替换子串
来源：http://fvy.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gjz.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://glh.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mma.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://wyl.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kkm.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kew.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ibq.meibo888.top

C#:   s.Replace("a", "b")
来源：http://gpj.svipenyu.cn

[E07] 按分隔符拆分
来源：http://yln.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zqx.yj20258888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kvu.zdqjudy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://srh.yj202588.top

TS:   s.split(",")
来源：http://age.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://cpy.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bry.meibo888.top

Ruby: s.split(",");  s.split
来源：http://thf.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ftu.ybcxt.top

[E08] 数组按分隔符合并
来源：http://rij.jyoumei.cn

Py:   ",".join(items)
来源：http://pzd.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://elx.shangyingyoupin.top

JS:   items.join(",")
来源：http://yds.yuxming.cn

TS:   items.join(",")
来源：http://wyh.jyoumei.cn

Java: String.join(",", items)
来源：http://lks.tanke756.top

Go:   strings.Join(items, ",")
来源：http://oof.svipenyu.cn

Ruby: items.join(",")
来源：http://cxs.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://nuk.iojbl.cn

[E09] 去除所有空白字符
来源：http://zok.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wab.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fbd.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://wmx.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://xcq.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://mxs.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://alo.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://als.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lub.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://ray.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vwb.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qny.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://tzw.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://wtu.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://din.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xog.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xlf.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ips.hcnkem.com

[E11] 反转字符串
来源：http://oln.cqqwz.cn

Py:   s[::-1]
来源：http://joo.jiagoushi.top

PHP:  strrev($s);
来源：http://hgj.tarul.cn

JS:   [...s].reverse().join("")
来源：http://vna.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://zxj.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://zbh.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oet.jqgfzy.top

Ruby: s.reverse
来源：http://eso.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://itr.yfazqb.com

[E12] 统计某字符出现次数
来源：http://elk.jiagoushi.top

Py:   s.count("a")
来源：http://wtr.pycfn.com

PHP:  substr_count($s, "a");
来源：http://fxt.jlsjyb.cn

JS:   s.split("a").length - 1
来源：http://nvw.ivvv.top

TS:   s.split("a").length - 1
来源：http://txp.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://goh.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://ylf.smart0.xyz

Ruby: s.count("a")
来源：http://ean.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://jkg.jqgufenzy.top

[E13] 逐字符遍历
来源：http://hpj.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://hix.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kev.aizwys.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gss.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jcg.jyoumei.cn


<!-- 参考信息 -->