代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://hhh.cucudq.cn

Ruby: arr = [1, 2, 3]
来源：http://iql.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jdy.chenjidiqi.icu

[D02] 追加元素到末尾
来源：http://bgh.hnqzz.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wat.xuetiantiany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wye.jianghu66.top

JS:   arr.push(4);
来源：http://soh.gzhubu.top

TS:   arr.push(4);
来源：http://zpf.9152youxi.cn

Java: list.add(4);
来源：http://yfk.zhoulong.xyz

Go:   arr = append(arr, 4)
来源：http://gdz.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zal.hfpthk.cn

C#:   list.Add(4);
来源：http://psy.ivvv.top

[D03] 在指定位置插入元素
来源：http://uzd.tanke756.top

Py:   arr.insert(0, 0)
来源：http://plu.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hxh.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vnd.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://mpy.zhiwuduotai.top

Java: list.add(0, 0);
来源：http://ajp.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://nid.gaohongyu789.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yhk.guowangkeji.top

C#:   list.Insert(0, 0);
来源：http://fqk.svipenyu.cn

[D04] 删除元素
来源：http://qcv.hongshengwenyu.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rar.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://utl.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dvt.feifeiyinyue.top

TS:   arr.splice(0, 1);
来源：http://jco.shanyushiyangtech.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mng.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xyf.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jxa.dashuyun.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nsu.nanxinkj.top

[D05] 访问与修改元素
来源：http://bkc.hfpthk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://enl.gaohongyu789.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jgm.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eex.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://dzo.daria6918.cn

Java: list.get(0); list.set(0, 9);
来源：http://fgx.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://mpy.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://szm.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ake.cqqwz.cn

[D06] 数组长度
来源：http://kbj.zhoulong.xyz

Py:   len(arr)
来源：http://szc.zhongyouzk.top

PHP:  count($arr);
来源：http://zmd.daxiang520.top

JS:   arr.length
来源：http://sbl.fanxiaobao.xyz

TS:   arr.length
来源：http://rzc.xingfuxueyuan.xyz

Java: list.size();
来源：http://vcw.wangdashe.top

Go:   len(arr)
来源：http://zzx.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://ewm.jinqigufen.top

C#:   list.Count;
来源：http://qwt.hnxiangtu.top

[D07] 切片 / 取子数组
来源：http://uzq.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vfz.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://svn.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://tjk.havefunace.top

TS:   arr.slice(1, 4);
来源：http://xbc.daxiang520.top

Java: list.subList(1, 4);
来源：http://iww.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://bmn.yvedp.cn

Ruby: arr[1, 3]
来源：http://cem.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://pct.nanxinkj.top

[D08] 合并两个数组
来源：http://awc.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://lpt.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://zut.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://rfe.andypj.xyz

TS:   [...a, ...b];
来源：http://aru.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xxi.9152youxi.cn

Go:   append(a, b...)
来源：http://zow.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://isp.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://oki.nanxinkj.top

[D09] 排序（升序）
来源：http://krh.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://cks.andypj.xyz

PHP:  sort($arr);
来源：http://ddz.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vme.uphjek.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://avr.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jhh.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jpn.fehbvm.com

Ruby: arr.sort
来源：http://snr.wangshuangyany.cn

C#:   list.Sort();
来源：http://dej.ydzc1.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dbl.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ywb.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zpt.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fba.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ssl.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxd.cashguo.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gkb.havefunace.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ijk.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gge.c1oappe.top

[D11] 反转数组
来源：http://asj.fktsv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wax.zycfv.cn

PHP:  array_reverse($arr);
来源：http://tvj.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://twn.uphjek.com

TS:   [...arr].reverse();
来源：http://kos.fzhhl.top

Java: Collections.reverse(list);
来源：http://zlj.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://pri.chenlongwang.top

Ruby: arr.reverse
来源：http://gql.nanxuanxn.top

C#:   list.Reverse();
来源：http://wet.feifeiyinyue.top

[D12] 查找元素下标
来源：http://kqn.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://izm.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rrd.hnxiangtu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdz.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://anj.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://brn.jinqigfzy.top

Go:   slices.Index(arr, x)
来源：http://uca.shanyushiyangtech.top

Ruby: arr.index(x)
来源：http://gcg.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://fou.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://sdf.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bhp.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dwm.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://coa.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://drz.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uos.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hdr.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ahi.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dts.xingfuxueyuan.xyz

[D14] 映射转换（每个元素变形）
来源：http://yyw.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://slw.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tkt.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://gmm.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://xvk.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zqp.cheryme.top

Go:   // 手写循环
来源：http://ibc.hnqzz.top

Ruby: arr.map { |x| x * 2 }
来源：http://nsw.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://szp.sxryk.cn

[D15] 去重
来源：http://joq.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wjn.zdbjq.cn

PHP:  array_unique($arr);
来源：http://kdb.fehbvm.com

JS:   [...new Set(arr)]
来源：http://bid.hnqzz.top

TS:   [...new Set(arr)]
来源：http://xhv.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://huk.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://wrm.zdqjudy.top

Ruby: arr.uniq
来源：http://bmm.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://dor.birdmap.top

[D16] 求和与平均值
来源：http://flz.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tvu.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qpf.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ryt.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kci.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xrg.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://clo.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ufc.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://huu.meibo888.top

[D17] 最大值与最小值
来源：http://hab.hammf.cn

Py:   max(arr);  min(arr)
来源：http://qja.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://php.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yvk.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://rmd.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zhn.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dsh.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://ild.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://vhf.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://ucq.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cwg.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://rsk.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ujv.yuanzhike.top

TS:   nested.flat();
来源：http://oib.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://esb.daria6918.cn

Go:   // 手写双层循环
来源：http://wac.daxiang520.top

Ruby: nested.flatten
来源：http://ciw.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eug.meibo888.top

[D19] 按字段分组
来源：http://dvh.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ico.shzxlz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://epo.hnqzz.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gxm.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yvb.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://der.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://fbs.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pft.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qzd.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://xdq.wangshuangyany.cn

Py:   Counter(arr)
来源：http://cyh.fengsongda.top

PHP:  array_count_values($arr);
来源：http://wvh.vehdjk.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ipm.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ozg.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ccz.pycfn.com

Go:   // 手写 map[T]int
来源：http://kqj.ctjpmb.com

Ruby: arr.tally
来源：http://hkt.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yie.havefunace.top

[D21] 判断是否包含某元素
来源：http://ncs.9152youxi.cn

Py:   x in arr
来源：http://ebi.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://adt.fktsv.cn

JS:   arr.includes(x)
来源：http://kbq.xziqi.cn

TS:   arr.includes(x)
来源：http://wmz.yvedp.cn

Java: list.contains(x)
来源：http://sbi.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://aha.havefunace.top

Ruby: arr.include?(x)
来源：http://vzz.yj20258888.top

C#:   list.Contains(x)
来源：http://dzl.pycfn.com

[D22] 复制数组（避免共享引用）
来源：http://bub.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vrw.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ogg.cucudq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mjn.hongshengwenyu.top

TS:   [...arr];
来源：http://ttw.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://xjf.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://yws.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://hue.316326.xyz

C#:   new List<int>(list);
来源：http://mdc.cheryme.top

[D23] reduce 累积计算
来源：http://lap.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yzg.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cwm.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sur.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bju.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://izz.fengsongda.top

Go:   // 手写循环
来源：http://lzc.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vxu.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vkd.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://ojl.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://amf.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iyf.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aeo.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xpg.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wif.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgg.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zrh.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ujn.jianghu66.top

[D25] Set 集合去重与交并差
来源：http://ipc.vehdjk.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fqv.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oij.yonumen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vua.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://glw.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qzz.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oss.vqdsnc.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ujj.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vzl.tanke756.top

[D26] 数组转字符串
来源：http://sjz.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://pep.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://xmp.hnqzz.top

JS:   arr.join(", ")
来源：http://csu.meibo888.top

TS:   arr.join(", ")
来源：http://nhy.yuxming.cn

Java: String.join(", ", list)
来源：http://qua.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://ifc.dashuyun.cn

Ruby: arr.join(", ")
来源：http://omt.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://hcf.yueranfly.top

================================================================================
来源：http://erv.ppjwa.cn

E. 字符串处理
来源：http://qeq.zhiwuduotai.top

================================================================================
来源：http://jdq.yuanzhike.top

[E01] 拼接字符串
来源：http://umr.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ftm.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nnp.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vnj.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kkw.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dba.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lfq.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hlu.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mlj.wangshuangyany.cn

[E02] 重复字符串
来源：http://chp.zhongyouzk.top

Py:   "ab" * 3
来源：http://uvp.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://ojp.wangdashe.top

JS:   "ab".repeat(3)
来源：http://atw.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://fxn.zycfv.cn

Java: "ab".repeat(3)
来源：http://fpo.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://qil.yongpay.top

Ruby: "ab" * 3
来源：http://sfe.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jce.xziqi.cn

[E03] 截取子串
来源：http://kib.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mkm.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xtt.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ivd.yuxming.cn

TS:   s.slice(1, 4)
来源：http://mbp.hammf.cn

Java: s.substring(1, 4)
来源：http://nwk.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xfy.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pxp.uphjek.com

C#:   s.Substring(1, 3)
来源：http://hff.gogol.net.cn

[E04] 查找子串位置
来源：http://ljo.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://dau.daxiang520.top

PHP:  strpos($s, "x");
来源：http://nox.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fau.wangdashe.top

TS:   s.indexOf("x")
来源：http://dxq.0kj1m.cn

Java: s.indexOf("x")
来源：http://ulk.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://qkd.hywenlv.cn

Ruby: s.index("x")
来源：http://bly.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://aag.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nct.0kj1m.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jon.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bsi.feifeiyinyue.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yoi.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dkz.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://suz.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vkd.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ucm.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wyg.snrcjt.cn

[E06] 替换子串
来源：http://fbm.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ecr.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://fnj.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oji.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://bkv.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://avm.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aqd.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lhe.cheryme.top

C#:   s.Replace("a", "b")
来源：http://rbu.sweek.top

[E07] 按分隔符拆分
来源：http://rra.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fmc.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hbx.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kmg.xylfe.cn

TS:   s.split(",")
来源：http://qct.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lja.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yvb.ivvv.top

Ruby: s.split(",");  s.split
来源：http://pyt.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qhr.52xcode.cn

[E08] 数组按分隔符合并
来源：http://iav.hongshengwenyu.top

Py:   ",".join(items)
来源：http://rkm.xziqi.cn

PHP:  implode(",", $items);
来源：http://zhz.cqqwz.cn

JS:   items.join(",")
来源：http://oki.xuetiantiany.cn

TS:   items.join(",")
来源：http://irm.fzhhl.top

Java: String.join(",", items)
来源：http://dqa.jlsjyb.cn


<!-- 参考信息 -->