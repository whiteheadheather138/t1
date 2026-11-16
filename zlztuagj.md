代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nnw.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ana.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ztq.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tgw.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://dtn.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://uuh.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rep.cashguo.top

[D02] 追加元素到末尾
来源：http://vyr.jinqigufen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qxz.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qkx.wangdashe.top

JS:   arr.push(4);
来源：http://adt.zhiwuduotai.top

TS:   arr.push(4);
来源：http://onf.shuidangran.top

Java: list.add(4);
来源：http://ozl.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://bmx.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://oev.andypj.xyz

C#:   list.Add(4);
来源：http://jnq.yj202588.top

[D03] 在指定位置插入元素
来源：http://wlp.xylfe.cn

Py:   arr.insert(0, 0)
来源：http://gvc.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mou.redwolf501.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dxe.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://htf.ctjpmb.com

Java: list.add(0, 0);
来源：http://dry.xylfe.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dtc.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vei.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://fgw.yvedp.cn

[D04] 删除元素
来源：http://oeo.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://qib.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lqq.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ees.sxryk.cn

TS:   arr.splice(0, 1);
来源：http://uqh.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ump.xylfe.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sit.jinqigufen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xvj.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kxo.haohaochexian.top

[D05] 访问与修改元素
来源：http://xyn.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ges.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://auk.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kfi.yuxming.cn

TS:   arr[0]; arr.at(-1);
来源：http://mau.jinqigfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://brx.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://jjn.bbcook.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fkn.shanyushiyangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hum.jinghuilouyu.cn

[D06] 数组长度
来源：http://ewo.ctjpmb.com

Py:   len(arr)
来源：http://cqz.jinyuanbaomall.cn

PHP:  count($arr);
来源：http://tpd.zhoulong.xyz

JS:   arr.length
来源：http://hxx.svipenyu.cn

TS:   arr.length
来源：http://kgp.zhijiandao.cn

Java: list.size();
来源：http://zmc.chenlongwang.top

Go:   len(arr)
来源：http://yla.guannengcc.top

Ruby: arr.length; arr.size
来源：http://tip.zhengqikj.top

C#:   list.Count;
来源：http://rod.jlsjyb.cn

[D07] 切片 / 取子数组
来源：http://rvh.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dog.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://hgh.nanxuanxn.top

JS:   arr.slice(1, 4);
来源：http://vnf.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://slm.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://cit.tian-w.cn

Go:   arr[1:4]
来源：http://njf.nwbrower.top

Ruby: arr[1, 3]
来源：http://ngd.fanxiaobao.xyz

C#:   list.GetRange(1, 3);
来源：http://jqe.feifeiyinyue.top

[D08] 合并两个数组
来源：http://cqx.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://sxd.epnwcf.com

PHP:  array_merge($a, $b);
来源：http://kog.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xdk.havefunace.top

TS:   [...a, ...b];
来源：http://aoz.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hpm.shzxlz.cn

Go:   append(a, b...)
来源：http://ozx.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://ilz.fktsv.cn

C#:   a.Concat(b).ToList()
来源：http://vtd.chenzaomai.com

[D09] 排序（升序）
来源：http://yci.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://pux.52xcode.cn

PHP:  sort($arr);
来源：http://trl.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mit.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://pik.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hkn.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bvn.hfpthk.cn

Ruby: arr.sort
来源：http://kla.ivvv.top

C#:   list.Sort();
来源：http://mxn.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iwz.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nlc.zdqjudy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fjp.ydjk.org.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iua.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://osc.xingfuxueyuan.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://voi.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://arr.guannengcc.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://joj.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pdi.zhaomingkeji.xyz

[D11] 反转数组
来源：http://kii.nanxinkj.top

Py:   arr[::-1];  arr.reverse()
来源：http://are.epnwcf.com

PHP:  array_reverse($arr);
来源：http://gfq.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hzz.yj202588.top

TS:   [...arr].reverse();
来源：http://bux.dianchejie.cn

Java: Collections.reverse(list);
来源：http://kju.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://kzy.shuidangran.top

Ruby: arr.reverse
来源：http://rot.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://vsr.yangfankeji.com

[D12] 查找元素下标
来源：http://dcj.shangyingyoupin.top

Py:   arr.index(x);  x in arr
来源：http://fcq.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zfr.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cuz.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pjp.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ofr.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://fdk.jlsjyb.cn

Ruby: arr.index(x)
来源：http://pay.hnqzz.top

C#:   list.IndexOf(x);
来源：http://ksk.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://fmo.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://msl.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aih.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://xus.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://qse.jianghu66.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ixp.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pjh.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://jua.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uaj.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://vmw.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xtl.hysaishi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mul.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://hbu.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://gxe.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xol.ivvv.top

Go:   // 手写循环
来源：http://agl.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wmf.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tym.svipenyu.cn

[D15] 去重
来源：http://gdq.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qze.tianlin.xyz

PHP:  array_unique($arr);
来源：http://jvn.bbcook.cn

JS:   [...new Set(arr)]
来源：http://nnb.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://mit.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iep.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://bhd.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://pvc.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://msc.kuanghao11.cn

[D16] 求和与平均值
来源：http://mke.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lft.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://prp.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iqf.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uav.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zsq.chenlongwang.top

Go:   // 手写循环累加
来源：http://pbs.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pyn.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://yyj.ivvv.top

[D17] 最大值与最小值
来源：http://lmx.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://drw.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://pff.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uiu.fktsv.cn

TS:   Math.max(...arr);
来源：http://tcx.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xqq.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pxs.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://mrv.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://rtd.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://tqo.vqdsnc.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bln.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://pbs.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aaz.smart0.xyz

TS:   nested.flat();
来源：http://pcv.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fol.hcnkem.com

Go:   // 手写双层循环
来源：http://jvn.havefunace.top

Ruby: nested.flatten
来源：http://sdl.zhaomingkeji.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://phq.wangdashe.top

[D19] 按字段分组
来源：http://gbi.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qiv.andypj.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bmf.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fwp.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qlh.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tii.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://tvv.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ieh.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zds.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://atu.hesvh.cn

Py:   Counter(arr)
来源：http://vfk.daxiang520.top

PHP:  array_count_values($arr);
来源：http://liw.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvz.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uvg.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oix.pycfn.com

Go:   // 手写 map[T]int
来源：http://dfh.iojbl.cn

Ruby: arr.tally
来源：http://hhf.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qsh.daria6918.cn

[D21] 判断是否包含某元素
来源：http://nxj.zdqjudy.top

Py:   x in arr
来源：http://niq.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://kax.yj20258888.top

JS:   arr.includes(x)
来源：http://ubi.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://xmd.jinqigufen.top

Java: list.contains(x)
来源：http://qja.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://wdn.c1oappe.top

Ruby: arr.include?(x)
来源：http://pzh.shuidangran.top

C#:   list.Contains(x)
来源：http://gqa.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://rqa.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nhb.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://stx.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nta.c1oappe.top

TS:   [...arr];
来源：http://rmp.316326.xyz

Java: new ArrayList<>(list);
来源：http://msa.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://ybm.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://ggj.birdmap.top

C#:   new List<int>(list);
来源：http://gpd.birdmap.top

[D23] reduce 累积计算
来源：http://enq.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://buv.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hvu.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zbv.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jff.tianlin.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://fus.redwolf501.top

Go:   // 手写循环
来源：http://dil.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xad.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lry.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://kxb.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ttz.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ydl.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://twf.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://onm.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://snk.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ame.jinqigfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sqi.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kbz.ivvv.top

[D25] Set 集合去重与交并差
来源：http://nhs.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vyk.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rrn.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oxw.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xyr.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tez.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lvq.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://idu.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kau.ydzc1.top

[D26] 数组转字符串
来源：http://xvx.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://ueo.guowangkeji.top

PHP:  implode(", ", $arr);
来源：http://vov.vehdjk.com

JS:   arr.join(", ")
来源：http://alr.shzxlz.cn

TS:   arr.join(", ")
来源：http://fxv.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://gsx.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://nlz.nwbrower.top

Ruby: arr.join(", ")
来源：http://uqe.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://hxc.zycfv.cn

================================================================================
来源：http://eba.dashuyun.cn

E. 字符串处理
来源：http://buc.daxiang520.top

================================================================================
来源：http://byz.gotoacloud.top

[E01] 拼接字符串
来源：http://txg.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ohj.jinghuilouyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hsx.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wvp.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fbq.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iyt.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jmk.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ygy.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jea.smart0.xyz

[E02] 重复字符串
来源：http://mdj.snrcjt.cn

Py:   "ab" * 3
来源：http://iai.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://ycp.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://mcr.daria6918.cn

TS:   "ab".repeat(3)
来源：http://byq.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://tzd.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://mfv.gaohongyu789.top

Ruby: "ab" * 3
来源：http://sga.sjlbkw.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jsz.yj20258.top

[E03] 截取子串
来源：http://tht.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://edw.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wwh.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vhh.yonumen.top

TS:   s.slice(1, 4)
来源：http://rok.quarkkingdee.top

Java: s.substring(1, 4)
来源：http://lgy.vehdjk.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gte.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://qta.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://res.hammf.cn

[E04] 查找子串位置
来源：http://erg.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://udr.yfazqb.com

PHP:  strpos($s, "x");
来源：http://lih.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lnc.cucudq.cn

TS:   s.indexOf("x")
来源：http://yff.ppjwa.cn

Java: s.indexOf("x")
来源：http://gie.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://vmv.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://yqh.xziqi.cn

C#:   s.IndexOf("x")
来源：http://xra.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pnj.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tst.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dwa.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsj.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://rcp.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://alj.shzxlz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://few.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lpu.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://upn.gogol.net.cn

[E06] 替换子串
来源：http://oge.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zqo.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://hgq.yonumen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xlf.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://uok.svipenyu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fzi.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pct.gaohongyu789.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tzi.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://kni.shzxlz.cn

[E07] 按分隔符拆分
来源：http://pjz.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mkt.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cig.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://svq.jianghu66.top

TS:   s.split(",")
来源：http://eyo.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fff.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wbe.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://jxe.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fbm.tarul.cn

[E08] 数组按分隔符合并
来源：http://nhm.jianghu66.top

Py:   ",".join(items)
来源：http://cgg.epnwcf.com


<!-- 参考信息 -->