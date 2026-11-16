代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vzc.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://dey.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tid.shzxlz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lxq.feifeiyinyue.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uxu.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zmp.redwolf501.top

[D05] 访问与修改元素
来源：http://qav.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rbd.yuxming.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uiw.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mah.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://qka.zhaomingkeji.xyz

Java: list.get(0); list.set(0, 9);
来源：http://pmr.c1oappe.top

Go:   arr[0]; arr[0] = 9
来源：http://xlv.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uwo.fengsongda.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://txz.jqgufenzy.top

[D06] 数组长度
来源：http://hix.jinqigufen.top

Py:   len(arr)
来源：http://biq.jiagoushi.top

PHP:  count($arr);
来源：http://daq.tian-w.cn

JS:   arr.length
来源：http://dpr.316326.xyz

TS:   arr.length
来源：http://mps.fehbvm.com

Java: list.size();
来源：http://sqa.shanyushiyangkeji.top

Go:   len(arr)
来源：http://ahs.cdnleiting.top

Ruby: arr.length; arr.size
来源：http://bmm.zhaomingkeji.xyz

C#:   list.Count;
来源：http://lxj.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://tto.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rjw.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://het.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://cen.tarul.cn

TS:   arr.slice(1, 4);
来源：http://acn.0kj1m.cn

Java: list.subList(1, 4);
来源：http://hxd.hnxiangtu.top

Go:   arr[1:4]
来源：http://qxy.chenzaomai.com

Ruby: arr[1, 3]
来源：http://hue.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://cbr.jiagoushi.top

[D08] 合并两个数组
来源：http://fiq.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://qrr.yj20258.top

PHP:  array_merge($a, $b);
来源：http://gew.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://red.jyoumei.cn

TS:   [...a, ...b];
来源：http://pca.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yzr.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://nkm.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://awi.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://bgf.hnqzz.top

[D09] 排序（升序）
来源：http://rab.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://uyb.gaohongyu789.top

PHP:  sort($arr);
来源：http://zov.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://knr.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://slk.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://glq.hnqzz.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dlr.zhengqikj.top

Ruby: arr.sort
来源：http://bdx.bjfxy.top

C#:   list.Sort();
来源：http://nva.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://elc.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rfq.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nxu.redwolf501.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://had.shanyushiyangtech.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nwf.jinghuilouyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uxd.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xyg.yanxiufei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mwy.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hco.wangshuangyany.cn

[D11] 反转数组
来源：http://epr.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://oba.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://zeg.jyoumei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cai.cashguo.top

TS:   [...arr].reverse();
来源：http://ycb.cdnleiting.top

Java: Collections.reverse(list);
来源：http://phs.bbcook.cn

Go:   slices.Reverse(arr)
来源：http://lpq.nanxuanxn.top

Ruby: arr.reverse
来源：http://vga.zdbjq.cn

C#:   list.Reverse();
来源：http://sza.tian-w.cn

[D12] 查找元素下标
来源：http://zno.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://pkv.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yfg.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ueq.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oer.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wfu.redwolf501.top

Go:   slices.Index(arr, x)
来源：http://ixv.gzhubu.top

Ruby: arr.index(x)
来源：http://czl.c1oappe.top

C#:   list.IndexOf(x);
来源：http://cfg.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://qlg.zhaomingkeji.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qbv.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kqo.wangdashe.top

JS:   arr.filter(x => x > 3)
来源：http://qur.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://ids.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jfr.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tqv.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://pgg.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://exv.tarul.cn

[D14] 映射转换（每个元素变形）
来源：http://fwy.svipenyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://liy.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ybk.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://lkw.sweek.top

TS:   arr.map(x => x * 2)
来源：http://shw.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ldd.xuetiantiany.cn

Go:   // 手写循环
来源：http://sss.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uof.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ryg.hongshengwenyu.top

[D15] 去重
来源：http://gbd.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zqq.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://zld.ydjk.org.cn

JS:   [...new Set(arr)]
来源：http://yoh.havefunace.top

TS:   [...new Set(arr)]
来源：http://vxe.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qzn.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://wgh.hysaishi.cn

Ruby: arr.uniq
来源：http://auu.cheryme.top

C#:   list.Distinct().ToList()
来源：http://plc.zhengqikj.top

[D16] 求和与平均值
来源：http://umj.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nlj.nwbrower.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pxp.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kgc.316326.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://las.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iut.andypj.xyz

Go:   // 手写循环累加
来源：http://hqq.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eyt.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://omj.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://hkv.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://fyd.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://dmd.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmw.jinqigufen.top

TS:   Math.max(...arr);
来源：http://tgz.jlsjyb.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tqj.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bne.pycfn.com

Ruby: arr.max;  arr.min
来源：http://wfo.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://bpl.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://yeo.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mly.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://glh.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://avj.yfazqb.com

TS:   nested.flat();
来源：http://pyl.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://inh.xinyue.icu

Go:   // 手写双层循环
来源：http://ake.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://twq.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://rvc.cucudq.cn

[D19] 按字段分组
来源：http://jxt.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hwo.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ayd.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kcu.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://rvq.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hxj.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://oxm.hnxiangtu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://daa.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yyu.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://ipr.nwbrower.top

Py:   Counter(arr)
来源：http://set.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://pgf.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvo.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sts.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fvd.zycfv.cn

Go:   // 手写 map[T]int
来源：http://atw.andypj.xyz

Ruby: arr.tally
来源：http://tch.havefunace.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://use.bjfxy.top

[D21] 判断是否包含某元素
来源：http://arm.epnwcf.com

Py:   x in arr
来源：http://hom.jianghu66.top

PHP:  in_array($x, $arr, true);
来源：http://iig.epnwcf.com

JS:   arr.includes(x)
来源：http://iys.jyoumei.cn

TS:   arr.includes(x)
来源：http://gyy.dianchejie.cn

Java: list.contains(x)
来源：http://thg.vehdjk.com

Go:   slices.Contains(arr, x)
来源：http://qdj.ivvv.top

Ruby: arr.include?(x)
来源：http://bjd.xuetiantiany.cn

C#:   list.Contains(x)
来源：http://icm.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://duv.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pck.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://brs.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fbu.cashguo.top

TS:   [...arr];
来源：http://mls.hesvh.cn

Java: new ArrayList<>(list);
来源：http://dqq.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://urq.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://gml.jinghuilouyu.cn

C#:   new List<int>(list);
来源：http://brg.chenzaomai.com

[D23] reduce 累积计算
来源：http://cnl.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jig.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gdo.ppjwa.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rmu.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zmq.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://muz.gogol.net.cn

Go:   // 手写循环
来源：http://mng.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kkr.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yhm.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://wmq.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ans.shanyushiyangtech.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xly.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bwy.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ckp.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://azt.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pdf.chenzaomai.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://osu.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://omm.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://tlr.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uxn.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xhk.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bil.jiagoushi.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ejl.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebq.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zwl.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xbl.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zgp.redwolf501.top

[D26] 数组转字符串
来源：http://cbr.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://fxh.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://uib.jlsjyb.cn

JS:   arr.join(", ")
来源：http://znj.yongpay.top

TS:   arr.join(", ")
来源：http://ztl.daria6918.cn

Java: String.join(", ", list)
来源：http://tya.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://lef.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://nni.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://kdw.sxryk.cn

================================================================================
来源：http://cuu.sysykeji.top

E. 字符串处理
来源：http://fqi.svipenyu.cn

================================================================================
来源：http://ljt.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://oef.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mtg.guannengcc.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vml.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ddv.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vgo.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yjk.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xsg.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cah.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mjk.zdbjq.cn

[E02] 重复字符串
来源：http://ivm.yuxming.cn

Py:   "ab" * 3
来源：http://umm.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://wyi.ivvv.top

JS:   "ab".repeat(3)
来源：http://hlg.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://xtu.mhx1999.top

Java: "ab".repeat(3)
来源：http://gmk.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://tqi.c1oappe.top

Ruby: "ab" * 3
来源：http://kac.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://brk.shuidangran.top

[E03] 截取子串
来源：http://ncg.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xch.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yje.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oia.hongshengwenyu.top

TS:   s.slice(1, 4)
来源：http://nou.tian-w.cn

Java: s.substring(1, 4)
来源：http://zal.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hsw.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://mta.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://iit.yuanzhike.top

[E04] 查找子串位置
来源：http://ugu.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://cxt.sweek.top

PHP:  strpos($s, "x");
来源：http://ybd.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vps.zdbjq.cn

TS:   s.indexOf("x")
来源：http://rfw.gaohongyu789.top

Java: s.indexOf("x")
来源：http://nlc.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://iuq.dashuyun.cn

Ruby: s.index("x")
来源：http://pmd.smart0.xyz

C#:   s.IndexOf("x")
来源：http://vco.jinqigfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zol.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbb.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gfj.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zqi.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pbp.cheryme.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xau.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://smb.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oep.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://coa.jyoumei.cn

[E06] 替换子串
来源：http://tkq.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kkx.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://zlo.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://con.yfazqb.com

TS:   s.replaceAll("a", "b")
来源：http://hdg.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yuz.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jed.tarul.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ann.sxryk.cn

C#:   s.Replace("a", "b")
来源：http://zhu.daxiang520.top

[E07] 按分隔符拆分
来源：http://iuc.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lix.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rjv.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://onj.redwolf501.top

TS:   s.split(",")
来源：http://rfj.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://slz.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://idv.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://otq.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dcg.yueranfly.top

[E08] 数组按分隔符合并
来源：http://etb.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://woc.yj20258.top

PHP:  implode(",", $items);
来源：http://vdh.zhijiandao.cn

JS:   items.join(",")
来源：http://snh.yuanzhike.top

TS:   items.join(",")
来源：http://kev.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://nss.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://gxt.jqgufenzy.top

Ruby: items.join(",")
来源：http://qsz.zhengqikj.top

C#:   string.Join(",", items)
来源：http://mkr.cqqwz.cn

[E09] 去除所有空白字符
来源：http://arm.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hyv.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wvc.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://zuy.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://zww.gaohongyu789.top

Java: s.replaceAll("\\s+", "")
来源：http://gnl.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kla.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://mpw.hnqzz.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://inj.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://pjk.snrcjt.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wyn.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ytu.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://pty.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://ido.jlsjyb.cn

Java: String.format("%03d", 7)
来源：http://uxv.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://usj.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ujb.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fgz.chenlongwang.top

[E11] 反转字符串
来源：http://rkq.jinqigufen.top

Py:   s[::-1]
来源：http://tod.havefunace.top

PHP:  strrev($s);
来源：http://ctu.birdmap.top


<!-- 参考信息 -->