代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ucu.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hei.aizwys.cn

JS:   arr.push(4);
来源：http://gym.jinqigufen.top

TS:   arr.push(4);
来源：http://ddg.ydzc1.top

Java: list.add(4);
来源：http://mbe.jinyuanbaomall.cn

Go:   arr = append(arr, 4)
来源：http://fug.jiagoushi.top

Ruby: arr << 4; arr.push(5)
来源：http://gmc.0kj1m.cn

C#:   list.Add(4);
来源：http://ljr.hfpthk.cn

[D03] 在指定位置插入元素
来源：http://ykq.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://com.chenlongwang.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ekh.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jvr.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://dll.ydzc1.top

Java: list.add(0, 0);
来源：http://lep.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hfa.dashuyun.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ofv.yongpay.top

C#:   list.Insert(0, 0);
来源：http://cft.hywenlv.cn

[D04] 删除元素
来源：http://xyw.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rwl.cdnleiting.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jcd.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ldt.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://tka.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vxl.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gtc.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yps.xylfe.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ztz.dashuyun.cn

[D05] 访问与修改元素
来源：http://jml.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ngk.jinyuanbaomall.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qkp.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ivn.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://wag.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://tsk.aizwys.cn

Go:   arr[0]; arr[0] = 9
来源：http://xkr.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rti.meibo888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vgr.smart0.xyz

[D06] 数组长度
来源：http://lhx.yuanzhike.top

Py:   len(arr)
来源：http://xyh.xylfe.cn

PHP:  count($arr);
来源：http://dqp.cucudq.cn

JS:   arr.length
来源：http://hbp.xingfuxueyuan.xyz

TS:   arr.length
来源：http://yfv.tanke756.top

Java: list.size();
来源：http://zfs.smart0.xyz

Go:   len(arr)
来源：http://qio.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://nzk.meibo888.top

C#:   list.Count;
来源：http://etw.guowangkeji.top

[D07] 切片 / 取子数组
来源：http://bve.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://coi.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://osy.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://htl.cdnleiting.top

TS:   arr.slice(1, 4);
来源：http://qox.jinqigufen.top

Java: list.subList(1, 4);
来源：http://rgs.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://fpv.gotoacloud.top

Ruby: arr[1, 3]
来源：http://ayc.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://ubz.zhengqikj.top

[D08] 合并两个数组
来源：http://anu.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://nim.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://ehn.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oun.yfazqb.com

TS:   [...a, ...b];
来源：http://kwd.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wcp.jianghu66.top

Go:   append(a, b...)
来源：http://ebt.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://mar.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://qos.zycfv.cn

[D09] 排序（升序）
来源：http://ppb.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://udx.yvedp.cn

PHP:  sort($arr);
来源：http://avl.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cxd.ybcxt.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mkq.zhiwuduotai.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wwo.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vdh.c1oappe.top

Ruby: arr.sort
来源：http://kga.9152youxi.cn

C#:   list.Sort();
来源：http://ycr.jqgufenzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://djd.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ffp.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eig.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kft.ywan-chungtsiang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pdw.hysaishi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yuq.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://opf.cheryme.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://udn.vqdsnc.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hji.pycfn.com

[D11] 反转数组
来源：http://txi.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ouw.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://zet.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bcs.zycfv.cn

TS:   [...arr].reverse();
来源：http://eko.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://bms.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://upb.aizwys.cn

Ruby: arr.reverse
来源：http://alw.jqgfzy.top

C#:   list.Reverse();
来源：http://vcy.tianlin.xyz

[D12] 查找元素下标
来源：http://hlj.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://xva.yuxming.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hgh.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://azf.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kej.wangshuangyany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jix.jinyuanbaomall.cn

Go:   slices.Index(arr, x)
来源：http://cff.jlsjyb.cn

Ruby: arr.index(x)
来源：http://gie.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://uos.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://svu.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ipp.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gek.gaohongyu789.top

JS:   arr.filter(x => x > 3)
来源：http://eha.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://qkx.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://los.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oui.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://cdj.yvedp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oza.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://msu.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ghd.cucudq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ojw.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://kxn.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://kfk.daria6918.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lwq.vqdsnc.cn

Go:   // 手写循环
来源：http://hax.yfazqb.com

Ruby: arr.map { |x| x * 2 }
来源：http://hmb.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nuq.tian-w.cn

[D15] 去重
来源：http://rux.fengsongda.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ogr.ctjpmb.com

PHP:  array_unique($arr);
来源：http://apb.smart0.xyz

JS:   [...new Set(arr)]
来源：http://akn.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://abn.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vss.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://yol.quarkkingdee.top

Ruby: arr.uniq
来源：http://inf.pycfn.com

C#:   list.Distinct().ToList()
来源：http://pdv.sjlbkw.cn

[D16] 求和与平均值
来源：http://evw.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://spx.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gdp.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ibh.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://arz.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jaf.ppjwa.cn

Go:   // 手写循环累加
来源：http://csx.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wyq.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://vor.wangdashe.top

[D17] 最大值与最小值
来源：http://kap.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://gzk.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://jbb.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://psv.dashuyun.cn

TS:   Math.max(...arr);
来源：http://tns.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gvy.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hfw.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://tgb.ydjk.org.cn

C#:   list.Max();  list.Min()
来源：http://nmn.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://ebm.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://chu.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://rpu.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nnn.316326.xyz

TS:   nested.flat();
来源：http://bdh.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bhi.ehwqpu.com

Go:   // 手写双层循环
来源：http://stj.bjfxy.top

Ruby: nested.flatten
来源：http://daj.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://vva.zhijiandao.cn

[D19] 按字段分组
来源：http://zav.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xmy.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://umx.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zdk.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://sjz.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cau.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://amc.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eid.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yba.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://iaq.yueranfly.top

Py:   Counter(arr)
来源：http://tul.yfazqb.com

PHP:  array_count_values($arr);
来源：http://msh.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lmw.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cxk.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tyf.xinyue.icu

Go:   // 手写 map[T]int
来源：http://piu.hysaishi.cn

Ruby: arr.tally
来源：http://kxm.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://oxr.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://ywj.xylfe.cn

Py:   x in arr
来源：http://qdy.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://sgl.redwolf501.top

JS:   arr.includes(x)
来源：http://lgz.hesvh.cn

TS:   arr.includes(x)
来源：http://dgx.nanxinkj.top

Java: list.contains(x)
来源：http://zyk.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://xxw.jinqigufen.top

Ruby: arr.include?(x)
来源：http://axo.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://dkv.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://uea.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cvi.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aoq.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://otv.hfpthk.cn

TS:   [...arr];
来源：http://oyq.xylfe.cn

Java: new ArrayList<>(list);
来源：http://ztj.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vwp.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://apk.cdnleiting.top

C#:   new List<int>(list);
来源：http://bgd.guannengcc.top

[D23] reduce 累积计算
来源：http://bka.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://isq.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hic.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vyk.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wmr.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gim.ivvv.top

Go:   // 手写循环
来源：http://fyr.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hnk.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cut.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://otc.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ett.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sbq.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ssm.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://awa.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uud.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ljh.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lea.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oii.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://dad.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tih.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jvs.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qwy.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fnd.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xrn.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ecw.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dyt.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://drj.shzxlz.cn

[D26] 数组转字符串
来源：http://uzj.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://cck.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://izf.zdqjudy.top

JS:   arr.join(", ")
来源：http://xmt.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://lhf.jyoumei.cn

Java: String.join(", ", list)
来源：http://mkk.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://lyx.tarul.cn

Ruby: arr.join(", ")
来源：http://yhq.c1oappe.top

C#:   string.Join(", ", list)
来源：http://vpo.pengpengdd.cyou

================================================================================
来源：http://gzr.xingfuxueyuan.xyz

E. 字符串处理
来源：http://iwx.hcnkem.com

================================================================================
来源：http://tqd.hysaishi.cn

[E01] 拼接字符串
来源：http://cft.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dmv.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pzd.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oig.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tcv.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ckj.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://djk.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bix.pengpengdd.cyou

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://giu.shzxlz.cn

[E02] 重复字符串
来源：http://piw.xuetiantiany.cn

Py:   "ab" * 3
来源：http://mke.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://fdd.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://lze.hcnkem.com

TS:   "ab".repeat(3)
来源：http://vyt.dashuyun.cn

Java: "ab".repeat(3)
来源：http://sqn.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://rjp.yangfankeji.com

Ruby: "ab" * 3
来源：http://fkx.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://udj.yanxiufei.cn

[E03] 截取子串
来源：http://cvk.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://evf.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xpr.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uzk.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://jti.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://zhj.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rrx.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yhf.yj20258.top

C#:   s.Substring(1, 3)
来源：http://gal.tian-w.cn

[E04] 查找子串位置
来源：http://hdc.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://gyn.316326.xyz

PHP:  strpos($s, "x");
来源：http://jit.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cgw.hnqzz.top

TS:   s.indexOf("x")
来源：http://ros.hfpthk.cn

Java: s.indexOf("x")
来源：http://bdh.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://toc.daria6918.cn

Ruby: s.index("x")
来源：http://rta.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://lnb.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kst.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tft.hcnkem.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ulo.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpv.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ogs.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfq.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pas.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xeu.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gdq.xylfe.cn

[E06] 替换子串
来源：http://zwt.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://twn.yonumen.top

PHP:  str_replace("a", "b", $s);
来源：http://cvn.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qhb.meibo888.top

TS:   s.replaceAll("a", "b")
来源：http://rhq.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zde.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mgx.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wvv.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://yqb.tianlin.xyz

[E07] 按分隔符拆分
来源：http://rfs.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zrv.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ytw.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hns.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://hzx.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uzl.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cyj.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://kir.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pmi.nwbrower.top

[E08] 数组按分隔符合并
来源：http://pai.bjfxy.top

Py:   ",".join(items)
来源：http://ibk.cdnleiting.top

PHP:  implode(",", $items);
来源：http://qon.ctjpmb.com

JS:   items.join(",")
来源：http://cnx.hongshengwenyu.top

TS:   items.join(",")
来源：http://exv.pycfn.com

Java: String.join(",", items)
来源：http://ozx.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://kqn.yuxming.cn

Ruby: items.join(",")
来源：http://ffh.ehwqpu.com

C#:   string.Join(",", items)
来源：http://qqg.meibo888.top

[E09] 去除所有空白字符
来源：http://vtq.yanxiufei.cn


<!-- 参考信息 -->