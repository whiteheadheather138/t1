代发 wailian999

D. 数组 / 列表 / 集合
来源：http://sul.shanyushiyangkeji.top

================================================================================
来源：http://hdc.xinyue.icu

[D01] 创建数组 / 列表
来源：http://ppt.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ldx.zycfv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tfz.316326.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pjh.0kj1m.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oze.aizwys.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kih.c1oappe.top

Go:   arr := []int{1, 2, 3}
来源：http://lec.ydjk.org.cn

Ruby: arr = [1, 2, 3]
来源：http://nnd.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cuz.ybcxt.top

[D02] 追加元素到末尾
来源：http://ivq.pycfn.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nsh.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oyp.xuanzx.com

JS:   arr.push(4);
来源：http://zrc.xinyue.icu

TS:   arr.push(4);
来源：http://wjg.daxiang520.top

Java: list.add(4);
来源：http://tor.sufxvd.cn

Go:   arr = append(arr, 4)
来源：http://uoq.xingfuxueyuan.xyz

Ruby: arr << 4; arr.push(5)
来源：http://pou.hywenlv.cn

C#:   list.Add(4);
来源：http://cbh.hcnkem.com

[D03] 在指定位置插入元素
来源：http://pvc.nwbrower.top

Py:   arr.insert(0, 0)
来源：http://sxy.yueranfly.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wwx.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfl.zdqjudy.top

TS:   arr.splice(0, 0, 0);
来源：http://tmz.zhaomingkeji.xyz

Java: list.add(0, 0);
来源：http://ztj.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vjg.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hol.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://diw.shzxlz.cn

[D04] 删除元素
来源：http://enn.yuxming.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hsj.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ktl.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zzw.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://gqw.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://coh.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pct.xinyue.icu

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://esi.quarkkingdee.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ctg.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://brk.shuidangran.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tvj.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mai.yuxming.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fyz.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://hdu.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://zml.shuidangran.top

Go:   arr[0]; arr[0] = 9
来源：http://xmv.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fju.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mox.fktsv.cn

[D06] 数组长度
来源：http://ijh.ctjpmb.com

Py:   len(arr)
来源：http://enk.shanyushiyangtech.top

PHP:  count($arr);
来源：http://rzm.cucudq.cn

JS:   arr.length
来源：http://txy.sxryk.cn

TS:   arr.length
来源：http://wsg.epnwcf.com

Java: list.size();
来源：http://liy.hesvh.cn

Go:   len(arr)
来源：http://sva.svipenyu.cn

Ruby: arr.length; arr.size
来源：http://yia.shangyingyoupin.top

C#:   list.Count;
来源：http://tlp.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://mlx.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://eea.andypj.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://oym.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://ibb.316326.xyz

TS:   arr.slice(1, 4);
来源：http://dzd.aizwys.cn

Java: list.subList(1, 4);
来源：http://zjg.cheryme.top

Go:   arr[1:4]
来源：http://eoo.sufxvd.cn

Ruby: arr[1, 3]
来源：http://ddc.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://hli.sufxvd.cn

[D08] 合并两个数组
来源：http://wtc.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://kja.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://ozb.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rat.yuxming.cn

TS:   [...a, ...b];
来源：http://nmw.ctjpmb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xvw.hongshengwenyu.top

Go:   append(a, b...)
来源：http://dox.xuanzx.com

Ruby: a + b;  a.concat(b)
来源：http://jzo.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://whq.gogol.net.cn

[D09] 排序（升序）
来源：http://hpl.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://qqr.yuxming.cn

PHP:  sort($arr);
来源：http://cew.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lrw.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://nnn.guowangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vjw.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fbn.tarul.cn

Ruby: arr.sort
来源：http://ydj.haohaochexian.top

C#:   list.Sort();
来源：http://eds.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://ies.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dfe.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://loo.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bst.nanxuanxn.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zjy.tarul.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://for.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wcw.gaohongyu789.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vif.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cfn.fanxiaobao.xyz

[D11] 反转数组
来源：http://cgd.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://oww.xylfe.cn

PHP:  array_reverse($arr);
来源：http://fix.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yba.andypj.xyz

TS:   [...arr].reverse();
来源：http://xtx.0kj1m.cn

Java: Collections.reverse(list);
来源：http://zii.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://mim.kuanghao11.cn

Ruby: arr.reverse
来源：http://boe.daxiang520.top

C#:   list.Reverse();
来源：http://rjd.fengsongda.top

[D12] 查找元素下标
来源：http://cyh.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://vrq.xingfuxueyuan.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ymy.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qph.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zce.shanyushiyangtech.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bud.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://yaz.smart0.xyz

Ruby: arr.index(x)
来源：http://qij.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://tpt.gaohongyu789.top

[D13] 过滤（保留满足条件的）
来源：http://rqi.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ied.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zvi.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://pmu.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://bai.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bka.jianghu66.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qyj.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gwv.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://reu.yfazqb.com

[D14] 映射转换（每个元素变形）
来源：http://mhz.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zmn.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rgr.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://pvg.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://zng.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://dpj.sysykeji.top

Go:   // 手写循环
来源：http://jew.zhongyouzk.top

Ruby: arr.map { |x| x * 2 }
来源：http://dvm.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kfp.gzhubu.top

[D15] 去重
来源：http://tej.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://quq.9152youxi.cn

PHP:  array_unique($arr);
来源：http://bde.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://gqt.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://wdl.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nsw.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fwx.bbcook.cn

Ruby: arr.uniq
来源：http://jlp.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://ken.zdqjudy.top

[D16] 求和与平均值
来源：http://uim.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oao.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iwc.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qtv.dashuyun.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://osi.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://izq.ydzc1.top

Go:   // 手写循环累加
来源：http://pwo.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://phz.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://xlc.gaohongyu789.top

[D17] 最大值与最小值
来源：http://wzt.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://pzk.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://aez.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sky.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://gmc.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cee.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dag.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://qmc.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://fna.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://iha.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kej.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://rhn.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vah.nanxuanxn.top

TS:   nested.flat();
来源：http://cee.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ftq.jqgufenzy.top

Go:   // 手写双层循环
来源：http://mka.fengsongda.top

Ruby: nested.flatten
来源：http://ebl.gogol.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tkx.yfazqb.com

[D19] 按字段分组
来源：http://ugv.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iaj.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rvw.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cwe.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gyu.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bod.yongpay.top

Go:   // 手写 map[string][]T
来源：http://lyy.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bcj.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mbe.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://sxu.dianchejie.cn

Py:   Counter(arr)
来源：http://xpb.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://jul.hammf.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ijv.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bpc.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pyz.sweek.top

Go:   // 手写 map[T]int
来源：http://hjq.hysaishi.cn

Ruby: arr.tally
来源：http://okf.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tij.316326.xyz

[D21] 判断是否包含某元素
来源：http://yfu.fzhhl.top

Py:   x in arr
来源：http://vba.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://jbk.zycfv.cn

JS:   arr.includes(x)
来源：http://zxo.jianghu66.top

TS:   arr.includes(x)
来源：http://ewh.zdqjudy.top

Java: list.contains(x)
来源：http://ycq.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://bjj.fzhhl.top

Ruby: arr.include?(x)
来源：http://wsr.tian-w.cn

C#:   list.Contains(x)
来源：http://mtu.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://aio.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eix.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bnp.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jcg.bjfxy.top

TS:   [...arr];
来源：http://fth.cdnleiting.top

Java: new ArrayList<>(list);
来源：http://dxl.gaohongyu789.top

Go:   copied := append([]int(nil), arr...)
来源：http://nag.tianlin.xyz

Ruby: arr.dup;  arr.clone
来源：http://uwk.aibaodan.cn

C#:   new List<int>(list);
来源：http://edx.zdbjq.cn

[D23] reduce 累积计算
来源：http://wpx.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://evl.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kkg.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfg.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hzn.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://jgw.nwbrower.top

Go:   // 手写循环
来源：http://aah.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mzt.ctjpmb.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wrx.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://qem.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qia.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kmn.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vnl.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pmb.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://grn.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uud.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qap.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iji.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://xiz.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pme.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pyy.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pqz.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://egs.mhx1999.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tdl.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jga.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xvg.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vxe.gzhubu.top

[D26] 数组转字符串
来源：http://ofx.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://vfi.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://lyz.ppjwa.cn

JS:   arr.join(", ")
来源：http://uuq.fzhhl.top

TS:   arr.join(", ")
来源：http://xal.yanxiufei.cn

Java: String.join(", ", list)
来源：http://cbm.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://nuk.jqgfzy.top

Ruby: arr.join(", ")
来源：http://vbi.mhx1999.top

C#:   string.Join(", ", list)
来源：http://fbt.havefunace.top

================================================================================
来源：http://pwk.xziqi.cn

E. 字符串处理
来源：http://nkx.gogol.net.cn

================================================================================
来源：http://ozf.zdqjudy.top

[E01] 拼接字符串
来源：http://ecs.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sag.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://occ.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://suu.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jeu.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://esn.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://esb.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tgn.shzxlz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://whk.zhoulong.xyz

[E02] 重复字符串
来源：http://hge.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://czy.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://kkp.yonumen.top

JS:   "ab".repeat(3)
来源：http://duv.pycfn.com

TS:   "ab".repeat(3)
来源：http://jqs.fengsongda.top

Java: "ab".repeat(3)
来源：http://eer.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://pmh.svipenyu.cn

Ruby: "ab" * 3
来源：http://lsf.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qnf.ydjk.org.cn

[E03] 截取子串
来源：http://etr.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vjo.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ljs.cashguo.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nog.hnqzz.top

TS:   s.slice(1, 4)
来源：http://ryz.uphjek.com

Java: s.substring(1, 4)
来源：http://ast.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wbb.ctjpmb.com

Ruby: s[1, 3];  s[1..3]
来源：http://pop.yonumen.top

C#:   s.Substring(1, 3)
来源：http://rwk.chenzaomai.com

[E04] 查找子串位置
来源：http://vax.feifeiyinyue.top

Py:   s.find("x");  s.index("x")
来源：http://nfj.meibo888.top

PHP:  strpos($s, "x");
来源：http://kek.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yhz.cashguo.top

TS:   s.indexOf("x")
来源：http://bkt.yongpay.top

Java: s.indexOf("x")
来源：http://bgm.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://ekz.zhoulong.xyz

Ruby: s.index("x")
来源：http://wmu.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://ges.zhaomingkeji.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvk.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://loh.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qre.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://szw.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://lll.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://afv.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ytp.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fri.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xxy.zycfv.cn

[E06] 替换子串
来源：http://qfu.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wqa.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://mlw.kuanghao11.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ljj.hongshengwenyu.top

TS:   s.replaceAll("a", "b")
来源：http://fds.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tzn.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wlw.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://feg.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://tau.zhixingplan.top

[E07] 按分隔符拆分
来源：http://zqx.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hdf.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jmw.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vja.tianlin.xyz

TS:   s.split(",")
来源：http://ali.shanyushiyangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://dpo.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jrn.vqdsnc.cn


<!-- 参考信息 -->