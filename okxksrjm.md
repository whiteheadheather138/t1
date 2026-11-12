代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://zbg.jqgfzy.top

Ruby: arr = [1, 2, 3]
来源：http://zpt.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://odc.yvedp.cn

[D02] 追加元素到末尾
来源：http://nag.yueranfly.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://svh.fehbvm.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hec.shuidangran.top

JS:   arr.push(4);
来源：http://qmb.bjfxy.top

TS:   arr.push(4);
来源：http://hkd.pengpengdd.cyou

Java: list.add(4);
来源：http://kqd.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://ugn.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://sbb.yfazqb.com

C#:   list.Add(4);
来源：http://emv.ywan-chungtsiang.top

[D03] 在指定位置插入元素
来源：http://dkb.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://mht.zhaomingkeji.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hmq.ydjk.org.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jfd.ctjpmb.com

TS:   arr.splice(0, 0, 0);
来源：http://yvy.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://goc.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://ouy.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://etu.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://uzy.xziqi.cn

[D04] 删除元素
来源：http://npp.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tow.zdqjudy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rzl.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rtp.sweek.top

TS:   arr.splice(0, 1);
来源：http://iba.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tqb.jyoumei.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xei.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ajv.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dzy.redwolf501.top

[D05] 访问与修改元素
来源：http://qih.xziqi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sku.fktsv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pcd.shangyingyoupin.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dsj.kuanghao11.cn

TS:   arr[0]; arr.at(-1);
来源：http://wlv.tanke756.top

Java: list.get(0); list.set(0, 9);
来源：http://kcx.shanyushiyangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://pmd.pengpengdd.cyou

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://apd.yvedp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nni.yfazqb.com

[D06] 数组长度
来源：http://nrs.ydjk.org.cn

Py:   len(arr)
来源：http://wjf.zdbjq.cn

PHP:  count($arr);
来源：http://wfn.xziqi.cn

JS:   arr.length
来源：http://hwz.shanyushiyangkeji.top

TS:   arr.length
来源：http://mao.haohaochexian.top

Java: list.size();
来源：http://ubu.yj202588.top

Go:   len(arr)
来源：http://ing.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://opb.ybcxt.top

C#:   list.Count;
来源：http://uhr.ehwqpu.com

[D07] 切片 / 取子数组
来源：http://szi.tianlin.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpb.guannengcc.top

PHP:  array_slice($arr, 1, 3);
来源：http://xzt.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://rwj.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://pqr.ivvv.top

Java: list.subList(1, 4);
来源：http://ojq.hcnkem.com

Go:   arr[1:4]
来源：http://jbf.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://aod.svipenyu.cn

C#:   list.GetRange(1, 3);
来源：http://arx.redwolf501.top

[D08] 合并两个数组
来源：http://sjf.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://asr.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://naz.sufxvd.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://exp.bjfxy.top

TS:   [...a, ...b];
来源：http://tcx.tanke756.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wcb.xziqi.cn

Go:   append(a, b...)
来源：http://vtp.gaohongyu789.top

Ruby: a + b;  a.concat(b)
来源：http://ucn.c1oappe.top

C#:   a.Concat(b).ToList()
来源：http://qau.gzhubu.top

[D09] 排序（升序）
来源：http://uet.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://gcm.zhengqikj.top

PHP:  sort($arr);
来源：http://dvo.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dbv.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ozp.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://brb.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gjj.yongpay.top

Ruby: arr.sort
来源：http://pgk.aizwys.cn

C#:   list.Sort();
来源：http://qsy.shanyushiyangtech.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bys.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xuh.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jze.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ika.sweek.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://slu.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jip.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gai.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rpn.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uzx.jqgfzy.top

[D11] 反转数组
来源：http://hjf.yvedp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hbx.guowangkeji.top

PHP:  array_reverse($arr);
来源：http://dbw.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://veo.ywan-chungtsiang.top

TS:   [...arr].reverse();
来源：http://ntv.yueranfly.top

Java: Collections.reverse(list);
来源：http://pqf.hammf.cn

Go:   slices.Reverse(arr)
来源：http://wwa.hongshengwenyu.top

Ruby: arr.reverse
来源：http://kwa.cashguo.top

C#:   list.Reverse();
来源：http://ovk.zycfv.cn

[D12] 查找元素下标
来源：http://nzc.daxiang520.top

Py:   arr.index(x);  x in arr
来源：http://cwv.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://scd.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqj.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uyh.sufxvd.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nhh.jinqigufen.top

Go:   slices.Index(arr, x)
来源：http://elf.yj202588.top

Ruby: arr.index(x)
来源：http://phw.aizwys.cn

C#:   list.IndexOf(x);
来源：http://msl.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://phm.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qkk.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mxi.cdnleiting.top

JS:   arr.filter(x => x > 3)
来源：http://cqm.yj20258.top

TS:   arr.filter(x => x > 3)
来源：http://wqg.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ocw.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ksn.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hsx.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uty.zycfv.cn

[D14] 映射转换（每个元素变形）
来源：http://rmd.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bqi.fengsongda.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rkd.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://nhu.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://cxj.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vej.sxryk.cn

Go:   // 手写循环
来源：http://mop.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://qpb.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://plk.bjfxy.top

[D15] 去重
来源：http://qan.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://som.quarkkingdee.top

PHP:  array_unique($arr);
来源：http://zrk.vehdjk.com

JS:   [...new Set(arr)]
来源：http://gkt.yj20258.top

TS:   [...new Set(arr)]
来源：http://kev.jqgufenzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yah.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://usg.sufxvd.cn

Ruby: arr.uniq
来源：http://jdr.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://shq.snrcjt.cn

[D16] 求和与平均值
来源：http://kne.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wur.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qeo.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcu.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://myc.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lgy.fzhhl.top

Go:   // 手写循环累加
来源：http://wvf.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rsi.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://cwc.yuanzhike.top

[D17] 最大值与最小值
来源：http://eym.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://hes.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://wyl.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://egz.tianlin.xyz

TS:   Math.max(...arr);
来源：http://meh.shzxlz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://guv.shangyingyoupin.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gdn.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://iqa.yongpay.top

C#:   list.Max();  list.Min()
来源：http://qle.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://dif.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uhl.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://kxa.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://epf.iojbl.cn

TS:   nested.flat();
来源：http://abg.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://psh.yuxming.cn

Go:   // 手写双层循环
来源：http://czd.c1oappe.top

Ruby: nested.flatten
来源：http://aox.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wfu.zhaomingkeji.xyz

[D19] 按字段分组
来源：http://cnb.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qcq.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://twv.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://map.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ryx.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fdm.meibo888.top

Go:   // 手写 map[string][]T
来源：http://bjv.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nws.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dxt.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://jee.hnqzz.top

Py:   Counter(arr)
来源：http://jxz.fktsv.cn

PHP:  array_count_values($arr);
来源：http://hsd.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xbo.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xvr.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yzh.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://uvj.gaohongyu789.top

Ruby: arr.tally
来源：http://mjm.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qsm.hammf.cn

[D21] 判断是否包含某元素
来源：http://kuh.zhongyouzk.top

Py:   x in arr
来源：http://jxq.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://foj.9152youxi.cn

JS:   arr.includes(x)
来源：http://wew.xuanzx.com

TS:   arr.includes(x)
来源：http://abj.aizwys.cn

Java: list.contains(x)
来源：http://ifv.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://dgb.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://bgc.gaohongyu789.top

C#:   list.Contains(x)
来源：http://ign.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://fzx.jqgufenzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qyc.hysaishi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://icv.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ekz.cucudq.cn

TS:   [...arr];
来源：http://sou.tian-w.cn

Java: new ArrayList<>(list);
来源：http://fil.zdqjudy.top

Go:   copied := append([]int(nil), arr...)
来源：http://aww.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://lal.guowangkeji.top

C#:   new List<int>(list);
来源：http://bqk.quarkkingdee.top

[D23] reduce 累积计算
来源：http://cev.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oix.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ust.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qvu.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cji.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nid.snrcjt.cn

Go:   // 手写循环
来源：http://cbp.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fyr.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sjk.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://oit.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hcx.sufxvd.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lrm.yj20258.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://orw.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cts.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xye.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ysz.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dys.hammf.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qdc.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://kmz.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://agv.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pcb.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qxj.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbu.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://era.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ntu.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oug.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://whz.sysykeji.top

[D26] 数组转字符串
来源：http://llj.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://qax.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://gqo.pycfn.com

JS:   arr.join(", ")
来源：http://vyx.zdqjudy.top

TS:   arr.join(", ")
来源：http://aua.nanxinkj.top

Java: String.join(", ", list)
来源：http://bhi.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://tpx.daxiang520.top

Ruby: arr.join(", ")
来源：http://gxr.daxiang520.top

C#:   string.Join(", ", list)
来源：http://vtp.aizwys.cn

================================================================================
来源：http://smu.zhongyouzk.top

E. 字符串处理
来源：http://spt.jqgufenzy.top

================================================================================
来源：http://jmm.zhiwuduotai.top

[E01] 拼接字符串
来源：http://prl.guannengcc.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xue.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rgx.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hzt.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dsv.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tus.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://asx.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wix.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jti.jinqigufen.top

[E02] 重复字符串
来源：http://xtn.guowangkeji.top

Py:   "ab" * 3
来源：http://obw.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://asq.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://fyj.c1oappe.top

TS:   "ab".repeat(3)
来源：http://hna.jiagoushi.top

Java: "ab".repeat(3)
来源：http://erw.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://qyw.fengsongda.top

Ruby: "ab" * 3
来源：http://pqp.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zqi.yuxming.cn

[E03] 截取子串
来源：http://hxf.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tqz.hywenlv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mna.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rto.yj202588.top

TS:   s.slice(1, 4)
来源：http://owm.fktsv.cn

Java: s.substring(1, 4)
来源：http://lge.kuanghao11.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://epd.andypj.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://zgw.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://sfg.mhx1999.top

[E04] 查找子串位置
来源：http://cnu.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://wzm.bjfxy.top

PHP:  strpos($s, "x");
来源：http://jsw.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wrc.dianchejie.cn

TS:   s.indexOf("x")
来源：http://ypy.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://qoh.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://woz.yonumen.top

Ruby: s.index("x")
来源：http://int.guowangkeji.top

C#:   s.IndexOf("x")
来源：http://vkt.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jkc.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kjb.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lhc.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://inh.hnqzz.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tkl.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mov.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kuv.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yrh.jianghu66.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xsq.zhoulong.xyz

[E06] 替换子串
来源：http://exi.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ylh.zhaomingkeji.xyz

PHP:  str_replace("a", "b", $s);
来源：http://fof.cdnleiting.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xsg.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://bus.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqp.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://atp.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ict.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://xvp.bjfxy.top

[E07] 按分隔符拆分
来源：http://onm.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zol.haohaochexian.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gjz.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://qac.iojbl.cn

TS:   s.split(",")
来源：http://zic.gzhubu.top

Java: s.split(",");  s.split("\\s+")
来源：http://qeg.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bdk.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://mfh.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ntb.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://npu.xziqi.cn

Py:   ",".join(items)
来源：http://vbw.aizwys.cn

PHP:  implode(",", $items);
来源：http://wac.zhengqikj.top

JS:   items.join(",")
来源：http://zht.ybcxt.top

TS:   items.join(",")
来源：http://cir.vehdjk.com

Java: String.join(",", items)
来源：http://qmy.hnxiangtu.top


<!-- 参考信息 -->