代发 wailian999

D. 数组 / 列表 / 集合
来源：http://hwv.haohaochexian.top

================================================================================
来源：http://she.52xcode.cn

[D01] 创建数组 / 列表
来源：http://bxf.sufxvd.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wwz.jyoumei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://btv.xinyue.icu

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qbr.pengpengdd.cyou

TS:   const arr: number[] = [1, 2, 3];
来源：http://eze.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wmb.chenlongwang.top

Go:   arr := []int{1, 2, 3}
来源：http://ych.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://wpx.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://poj.ydjk.org.cn

[D02] 追加元素到末尾
来源：http://mya.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jby.hcnkem.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://txm.gzhubu.top

JS:   arr.push(4);
来源：http://zmf.cucudq.cn

TS:   arr.push(4);
来源：http://css.9152youxi.cn

Java: list.add(4);
来源：http://hrv.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://wqi.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://yhw.xziqi.cn

C#:   list.Add(4);
来源：http://njv.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://eie.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://eyt.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://svo.guannengcc.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tlq.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ril.jqgufenzy.top

Java: list.add(0, 0);
来源：http://vkv.nanxinkj.top

Go:   arr = append([]int{0}, arr...)
来源：http://gtr.hesvh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://byu.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://lek.shanyushiyangtech.top

[D04] 删除元素
来源：http://jsf.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://nwo.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hey.sxryk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kyd.chenjidiqi.icu

TS:   arr.splice(0, 1);
来源：http://mmj.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hmt.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ovw.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ulr.yuanzhike.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rxl.zdbjq.cn

[D05] 访问与修改元素
来源：http://hef.nanxinkj.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ltd.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zct.uphjek.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lyh.sufxvd.cn

TS:   arr[0]; arr.at(-1);
来源：http://gea.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://gkz.cashguo.top

Go:   arr[0]; arr[0] = 9
来源：http://emt.chenlongwang.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xom.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qxx.hnqzz.top

[D06] 数组长度
来源：http://ees.shuidangran.top

Py:   len(arr)
来源：http://vlx.ivvv.top

PHP:  count($arr);
来源：http://wcx.bjfxy.top

JS:   arr.length
来源：http://ppp.yueranfly.top

TS:   arr.length
来源：http://yql.shanyushiyangtech.top

Java: list.size();
来源：http://ztj.svipenyu.cn

Go:   len(arr)
来源：http://bve.tianlin.xyz

Ruby: arr.length; arr.size
来源：http://njd.sxryk.cn

C#:   list.Count;
来源：http://cfz.andypj.xyz

[D07] 切片 / 取子数组
来源：http://uas.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dsa.quarkkingdee.top

PHP:  array_slice($arr, 1, 3);
来源：http://bem.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://hzm.jqgfzy.top

TS:   arr.slice(1, 4);
来源：http://sfc.yuanzhike.top

Java: list.subList(1, 4);
来源：http://fke.jqgufenzy.top

Go:   arr[1:4]
来源：http://jxd.sweek.top

Ruby: arr[1, 3]
来源：http://axd.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://ntu.uphjek.com

[D08] 合并两个数组
来源：http://ady.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://eaq.xinyue.icu

PHP:  array_merge($a, $b);
来源：http://tly.sxryk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kfi.yj202588.top

TS:   [...a, ...b];
来源：http://vbs.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hos.meibo888.top

Go:   append(a, b...)
来源：http://owk.redwolf501.top

Ruby: a + b;  a.concat(b)
来源：http://rcm.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://goh.52xcode.cn

[D09] 排序（升序）
来源：http://wkx.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://kpt.hnxiangtu.top

PHP:  sort($arr);
来源：http://hcr.hammf.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://aug.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bvq.sjlbkw.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://txz.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sbn.ppjwa.cn

Ruby: arr.sort
来源：http://lni.pengpengdd.cyou

C#:   list.Sort();
来源：http://yxb.0kj1m.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vub.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ptu.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rqi.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxf.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://aip.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://siy.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hvp.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rvn.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqg.redwolf501.top

[D11] 反转数组
来源：http://qdg.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://liv.ydzc1.top

PHP:  array_reverse($arr);
来源：http://dyk.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uqe.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://jlj.yvedp.cn

Java: Collections.reverse(list);
来源：http://qtj.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://dox.jqgufenzy.top

Ruby: arr.reverse
来源：http://prk.hysaishi.cn

C#:   list.Reverse();
来源：http://dnl.tian-w.cn

[D12] 查找元素下标
来源：http://iya.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://ipy.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://aub.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nmm.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qgd.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fyn.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://jfz.snrcjt.cn

Ruby: arr.index(x)
来源：http://prx.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://ztx.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://nzy.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yem.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ipa.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://cyz.hnqzz.top

TS:   arr.filter(x => x > 3)
来源：http://ypb.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dxr.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://odh.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://yox.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://duj.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://jtk.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nty.bjfxy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://krb.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://kpt.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://hxq.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://lpz.gzhubu.top

Go:   // 手写循环
来源：http://pxx.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://llb.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lol.yuanzhike.top

[D15] 去重
来源：http://qjk.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bgw.fengsongda.top

PHP:  array_unique($arr);
来源：http://vsw.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://trl.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://yqj.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rtn.jyoumei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://frx.xuanzx.com

Ruby: arr.uniq
来源：http://ndf.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://cmx.hnxiangtu.top

[D16] 求和与平均值
来源：http://vms.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://min.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wea.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://alw.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rig.xuanzx.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ggk.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://dnt.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eqd.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://nck.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://tne.fanxiaobao.xyz

Py:   max(arr);  min(arr)
来源：http://oqk.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://tzg.aizwys.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eax.dianchejie.cn

TS:   Math.max(...arr);
来源：http://hfb.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qac.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baj.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://bhk.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://mib.cashguo.top

[D18] 扁平化嵌套数组
来源：http://qcp.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dnb.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://hwy.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lgi.jqgfzy.top

TS:   nested.flat();
来源：http://cez.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xzp.cqqwz.cn

Go:   // 手写双层循环
来源：http://zim.nanxinkj.top

Ruby: nested.flatten
来源：http://aai.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wgf.feifeiyinyue.top

[D19] 按字段分组
来源：http://zuw.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://heo.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fbd.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nlu.yvedp.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kyk.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://udp.pycfn.com

Go:   // 手写 map[string][]T
来源：http://isr.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mwg.kuanghao11.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wof.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://bwh.tian-w.cn

Py:   Counter(arr)
来源：http://oge.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://shv.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ght.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyy.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aeo.0kj1m.cn

Go:   // 手写 map[T]int
来源：http://nlc.cucudq.cn

Ruby: arr.tally
来源：http://ede.wangdashe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mct.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://iot.yfazqb.com

Py:   x in arr
来源：http://wjc.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://etw.316326.xyz

JS:   arr.includes(x)
来源：http://aqx.cheryme.top

TS:   arr.includes(x)
来源：http://oyb.0kj1m.cn

Java: list.contains(x)
来源：http://mfq.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://dgl.yfazqb.com

Ruby: arr.include?(x)
来源：http://djv.yfazqb.com

C#:   list.Contains(x)
来源：http://upk.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://gmo.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ghw.xingfuxueyuan.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://edg.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gez.zhoulong.xyz

TS:   [...arr];
来源：http://nsq.xuanzx.com

Java: new ArrayList<>(list);
来源：http://tyt.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://tsg.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://wwh.aizwys.cn

C#:   new List<int>(list);
来源：http://pke.yj20258888.top

[D23] reduce 累积计算
来源：http://inu.jiagoushi.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ngo.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jal.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vdn.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vol.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jop.zycfv.cn

Go:   // 手写循环
来源：http://xyy.yuxming.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://apv.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kfh.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://yjy.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://icm.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ksd.zhongyouzk.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ord.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ewk.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jum.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tzr.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hoo.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lda.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://xuh.jqgfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xcv.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rga.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tjk.smart0.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jhy.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wfq.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jql.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jya.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwb.redwolf501.top

[D26] 数组转字符串
来源：http://jxl.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://jjg.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://ggd.uphjek.com

JS:   arr.join(", ")
来源：http://moc.bbcook.cn

TS:   arr.join(", ")
来源：http://foq.jqgfzy.top

Java: String.join(", ", list)
来源：http://tkx.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://zjd.hongshengwenyu.top

Ruby: arr.join(", ")
来源：http://uco.chenjidiqi.icu

C#:   string.Join(", ", list)
来源：http://bpv.uphjek.com

================================================================================
来源：http://ige.aizwys.cn

E. 字符串处理
来源：http://vdm.jyoumei.cn

================================================================================
来源：http://ody.zdbjq.cn

[E01] 拼接字符串
来源：http://kwm.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://enr.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wmj.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://exz.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bcm.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vsi.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lic.xuetiantiany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qvu.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rhw.gaohongyu789.top

[E02] 重复字符串
来源：http://nal.nwbrower.top

Py:   "ab" * 3
来源：http://tbw.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://emi.birdmap.top

JS:   "ab".repeat(3)
来源：http://vsc.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://ste.bjfxy.top

Java: "ab".repeat(3)
来源：http://qbi.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://fsx.ydjk.org.cn

Ruby: "ab" * 3
来源：http://soa.9152youxi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://weu.guowangkeji.top

[E03] 截取子串
来源：http://ufx.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mhr.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eob.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gzh.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://rzc.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://bim.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://erp.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://gcj.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://ucp.yuanzhike.top

[E04] 查找子串位置
来源：http://kpp.xuanzx.com

Py:   s.find("x");  s.index("x")
来源：http://avd.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://fji.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tjw.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://tlx.gzhubu.top

Java: s.indexOf("x")
来源：http://jmr.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://vsf.epnwcf.com

Ruby: s.index("x")
来源：http://gln.iojbl.cn

C#:   s.IndexOf("x")
来源：http://ras.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pij.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rev.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sah.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://efz.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cfm.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ytn.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dmy.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jdf.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bvv.yueranfly.top

[E06] 替换子串
来源：http://kfl.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ycl.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dgr.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jfd.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://evi.sjlbkw.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nrf.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yff.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xlm.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://cnx.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://fca.cqqwz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vtx.gogol.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vex.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lxy.yj20258888.top

TS:   s.split(",")
来源：http://vqk.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bzw.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://khg.gzhubu.top


<!-- 参考信息 -->