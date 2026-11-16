代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ddg.hysaishi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xqh.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://iqf.bjfxy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zbn.zhijiandao.cn

Go:   arr := []int{1, 2, 3}
来源：http://udn.svipenyu.cn

Ruby: arr = [1, 2, 3]
来源：http://lbd.jinyuanbaomall.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dlm.mhx1999.top

[D02] 追加元素到末尾
来源：http://epe.hnxiangtu.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ksi.ivvv.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iwz.gogol.net.cn

JS:   arr.push(4);
来源：http://tll.tian-w.cn

TS:   arr.push(4);
来源：http://iht.tianlin.xyz

Java: list.add(4);
来源：http://qgq.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://usn.birdmap.top

Ruby: arr << 4; arr.push(5)
来源：http://yhy.jlsjyb.cn

C#:   list.Add(4);
来源：http://qzz.sxryk.cn

[D03] 在指定位置插入元素
来源：http://nwa.sufxvd.cn

Py:   arr.insert(0, 0)
来源：http://ebs.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qxl.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mik.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://yqa.andypj.xyz

Java: list.add(0, 0);
来源：http://aib.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gkt.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://csp.meibo888.top

C#:   list.Insert(0, 0);
来源：http://por.zhengqikj.top

[D04] 删除元素
来源：http://ffn.jqgufenzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aym.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xca.haohaochexian.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mly.yongpay.top

TS:   arr.splice(0, 1);
来源：http://vyw.xuanzx.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hzv.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://shv.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gos.sweek.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dap.yfazqb.com

[D05] 访问与修改元素
来源：http://dqq.ctjpmb.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bcp.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://msa.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zfa.mhx1999.top

TS:   arr[0]; arr.at(-1);
来源：http://xau.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://hut.vqdsnc.cn

Go:   arr[0]; arr[0] = 9
来源：http://ort.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zjw.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ugx.shanyushiyangtech.top

[D06] 数组长度
来源：http://vwy.nanxuanxn.top

Py:   len(arr)
来源：http://tso.ppjwa.cn

PHP:  count($arr);
来源：http://tts.snrcjt.cn

JS:   arr.length
来源：http://tww.fengsongda.top

TS:   arr.length
来源：http://frw.smart0.xyz

Java: list.size();
来源：http://lwi.ydjk.org.cn

Go:   len(arr)
来源：http://kyu.xylfe.cn

Ruby: arr.length; arr.size
来源：http://mzq.zhiwuduotai.top

C#:   list.Count;
来源：http://mml.yfazqb.com

[D07] 切片 / 取子数组
来源：http://imu.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tpd.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://beg.yonumen.top

JS:   arr.slice(1, 4);
来源：http://mfo.ivvv.top

TS:   arr.slice(1, 4);
来源：http://ahs.tian-w.cn

Java: list.subList(1, 4);
来源：http://dmn.yongpay.top

Go:   arr[1:4]
来源：http://klg.yuxming.cn

Ruby: arr[1, 3]
来源：http://ybm.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://mlx.fzhhl.top

[D08] 合并两个数组
来源：http://ida.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://opk.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://svd.9152youxi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zvb.birdmap.top

TS:   [...a, ...b];
来源：http://zmw.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qbn.sxryk.cn

Go:   append(a, b...)
来源：http://apc.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://vsa.ydzc1.top

C#:   a.Concat(b).ToList()
来源：http://uni.pycfn.com

[D09] 排序（升序）
来源：http://nqh.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ylu.9152youxi.cn

PHP:  sort($arr);
来源：http://kjw.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ozo.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rns.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zhi.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jpm.cheryme.top

Ruby: arr.sort
来源：http://jet.zhengqikj.top

C#:   list.Sort();
来源：http://ksg.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://arh.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://odu.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ggs.shzxlz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hxu.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qsu.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aaz.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://son.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nva.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://luu.zycfv.cn

[D11] 反转数组
来源：http://cvj.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://qzr.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://wsg.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eab.yueranfly.top

TS:   [...arr].reverse();
来源：http://ntg.andypj.xyz

Java: Collections.reverse(list);
来源：http://hvc.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://yog.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://pff.uphjek.com

C#:   list.Reverse();
来源：http://dqm.smart0.xyz

[D12] 查找元素下标
来源：http://rhg.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://ctx.vehdjk.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pnk.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mdu.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iqy.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://okw.uphjek.com

Go:   slices.Index(arr, x)
来源：http://ima.fengsongda.top

Ruby: arr.index(x)
来源：http://uvv.ehwqpu.com

C#:   list.IndexOf(x);
来源：http://vui.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://unb.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nyl.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wsp.ehwqpu.com

JS:   arr.filter(x => x > 3)
来源：http://qhb.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://nki.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uje.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uaz.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://uxw.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://frg.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://rru.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jcg.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uwj.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://ysw.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://rvz.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ouv.aizwys.cn

Go:   // 手写循环
来源：http://lnl.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://tlm.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://gdw.jiagoushi.top

[D15] 去重
来源：http://vdc.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qqa.9152youxi.cn

PHP:  array_unique($arr);
来源：http://yzu.bjfxy.top

JS:   [...new Set(arr)]
来源：http://pxi.cucudq.cn

TS:   [...new Set(arr)]
来源：http://zvo.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://amg.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://prs.yfazqb.com

Ruby: arr.uniq
来源：http://iok.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://ywi.hfpthk.cn

[D16] 求和与平均值
来源：http://zeo.ivvv.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dwv.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ahq.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xnh.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://udv.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cub.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://fyc.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oaz.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://eku.xinyue.icu

[D17] 最大值与最小值
来源：http://siy.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://szz.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://jrj.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vxh.gzhubu.top

TS:   Math.max(...arr);
来源：http://djl.yuxming.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xtx.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cxs.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://qai.hammf.cn

C#:   list.Max();  list.Min()
来源：http://qxk.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://wow.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kqy.vqdsnc.cn

PHP:  array_merge(...$nested);
来源：http://oqd.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mos.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://hzu.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wui.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://xtc.kuanghao11.cn

Ruby: nested.flatten
来源：http://ezz.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nun.shuidangran.top

[D19] 按字段分组
来源：http://keo.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vod.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qqe.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iov.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://cpb.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yjt.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://qsb.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jbb.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fte.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://kyp.cqqwz.cn

Py:   Counter(arr)
来源：http://rrt.pycfn.com

PHP:  array_count_values($arr);
来源：http://mml.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fgn.yangfankeji.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kxa.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zac.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://fha.yuxming.cn

Ruby: arr.tally
来源：http://cqw.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iab.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://lly.hysaishi.cn

Py:   x in arr
来源：http://sgk.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://mjp.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://bjj.shuidangran.top

TS:   arr.includes(x)
来源：http://pmo.ivvv.top

Java: list.contains(x)
来源：http://ayw.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://fwx.uphjek.com

Ruby: arr.include?(x)
来源：http://xiy.yj20258.top

C#:   list.Contains(x)
来源：http://ndv.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://tob.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tft.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zjh.yangfankeji.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wcw.vqdsnc.cn

TS:   [...arr];
来源：http://lto.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://koy.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://ynx.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://mxp.gaohongyu789.top

C#:   new List<int>(list);
来源：http://iww.dashuyun.cn

[D23] reduce 累积计算
来源：http://abf.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hjv.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sfg.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bhy.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://itz.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mbt.ctjpmb.com

Go:   // 手写循环
来源：http://kcy.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zkb.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qcu.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://hwx.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kos.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wws.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yxi.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pdl.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jiz.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vtx.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pdr.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://etx.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://coe.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yfp.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://joj.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gwz.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hav.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bri.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xsx.daria6918.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hzb.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ynh.jlsjyb.cn

[D26] 数组转字符串
来源：http://eca.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://udp.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://rel.fehbvm.com

JS:   arr.join(", ")
来源：http://ncg.shuidangran.top

TS:   arr.join(", ")
来源：http://lyc.redwolf501.top

Java: String.join(", ", list)
来源：http://wso.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://elk.tanke756.top

Ruby: arr.join(", ")
来源：http://vxm.52xcode.cn

C#:   string.Join(", ", list)
来源：http://hbk.havefunace.top

================================================================================
来源：http://muz.gaohongyu789.top

E. 字符串处理
来源：http://cvn.yfazqb.com

================================================================================
来源：http://jom.sxryk.cn

[E01] 拼接字符串
来源：http://jny.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blh.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bhi.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wcw.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dmf.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uhm.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kxs.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ztl.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://btm.feifeiyinyue.top

[E02] 重复字符串
来源：http://jpe.yueranfly.top

Py:   "ab" * 3
来源：http://yiz.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://bej.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://sgl.yvedp.cn

TS:   "ab".repeat(3)
来源：http://eay.jianghu66.top

Java: "ab".repeat(3)
来源：http://iwt.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://ouv.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://huk.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ybi.hysaishi.cn

[E03] 截取子串
来源：http://cpy.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ffu.dashuyun.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fvy.dianchejie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vln.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://hsb.hnqzz.top

Java: s.substring(1, 4)
来源：http://crp.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zbf.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://nkh.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://bxf.yj20258.top

[E04] 查找子串位置
来源：http://ufv.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://ntd.xuanzx.com

PHP:  strpos($s, "x");
来源：http://amw.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hqn.yj20258.top

TS:   s.indexOf("x")
来源：http://jdl.zhijiandao.cn

Java: s.indexOf("x")
来源：http://xtg.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://yac.shangyingyoupin.top

Ruby: s.index("x")
来源：http://qqq.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://dzo.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hxy.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hpj.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jko.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bma.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pnv.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cir.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lsk.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ejm.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ipm.zhixingplan.top

[E06] 替换子串
来源：http://vyl.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tll.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://qff.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ida.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://cnl.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aog.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yki.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://egd.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://qan.ivvv.top

[E07] 按分隔符拆分
来源：http://zud.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dmf.nanxuanxn.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cpy.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://gvl.hnqzz.top

TS:   s.split(",")
来源：http://wvc.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://nll.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kul.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://rse.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://grs.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://qjf.zhengqikj.top

Py:   ",".join(items)
来源：http://yfs.zdqjudy.top


<!-- 参考信息 -->