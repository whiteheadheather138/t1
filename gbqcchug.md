代发 wailian999

[D03] 在指定位置插入元素
来源：http://cjc.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://rhi.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kla.epnwcf.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xit.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://tpg.dashuyun.cn

Java: list.add(0, 0);
来源：http://yyr.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://fzx.fehbvm.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qxp.cashguo.top

C#:   list.Insert(0, 0);
来源：http://rlj.cheryme.top

[D04] 删除元素
来源：http://dde.jlsjyb.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wyv.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gho.ctjpmb.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yaq.yanxiufei.cn

TS:   arr.splice(0, 1);
来源：http://abz.sjlbkw.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bem.birdmap.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ura.hesvh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wrv.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cnw.yueranfly.top

[D05] 访问与修改元素
来源：http://bui.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cwb.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uke.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nnd.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://rdm.andypj.xyz

Java: list.get(0); list.set(0, 9);
来源：http://bma.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://gje.sweek.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nvs.hfpthk.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gik.hongshengwenyu.top

[D06] 数组长度
来源：http://mrf.xziqi.cn

Py:   len(arr)
来源：http://qvd.gzhubu.top

PHP:  count($arr);
来源：http://iyh.shangyingyoupin.top

JS:   arr.length
来源：http://hdk.ydzc1.top

TS:   arr.length
来源：http://zpe.zhongyouzk.top

Java: list.size();
来源：http://lny.gotoacloud.top

Go:   len(arr)
来源：http://pwz.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://fuz.zhiwuduotai.top

C#:   list.Count;
来源：http://typ.tanke756.top

[D07] 切片 / 取子数组
来源：http://het.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://egx.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://klq.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://pag.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://mvr.meibo888.top

Java: list.subList(1, 4);
来源：http://zxv.tianlin.xyz

Go:   arr[1:4]
来源：http://apj.tarul.cn

Ruby: arr[1, 3]
来源：http://inr.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://ivs.dianchejie.cn

[D08] 合并两个数组
来源：http://jrm.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://rab.wangdashe.top

PHP:  array_merge($a, $b);
来源：http://gfv.xinyue.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://xuq.zhaomingkeji.xyz

TS:   [...a, ...b];
来源：http://lob.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ybe.zdqjudy.top

Go:   append(a, b...)
来源：http://rnm.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://vxc.chenzaomai.com

C#:   a.Concat(b).ToList()
来源：http://bgz.jianghu66.top

[D09] 排序（升序）
来源：http://qzr.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://twc.andypj.xyz

PHP:  sort($arr);
来源：http://vvl.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dwn.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tqp.pycfn.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ucy.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://giv.chenlongwang.top

Ruby: arr.sort
来源：http://dgd.kuanghao11.cn

C#:   list.Sort();
来源：http://wcl.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lpy.yanxiufei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qur.jqgfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uwr.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ftw.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnx.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tdj.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uiu.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dsi.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gln.zhixingplan.top

[D11] 反转数组
来源：http://tko.zhijiandao.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zid.jlsjyb.cn

PHP:  array_reverse($arr);
来源：http://tcg.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ser.jiagoushi.top

TS:   [...arr].reverse();
来源：http://ebv.9152youxi.cn

Java: Collections.reverse(list);
来源：http://kiz.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://djo.nanxuanxn.top

Ruby: arr.reverse
来源：http://niq.cqqwz.cn

C#:   list.Reverse();
来源：http://mxd.xylfe.cn

[D12] 查找元素下标
来源：http://djm.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://htt.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cxe.guowangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wte.andypj.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qzy.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lcb.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://ret.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://nyq.xuanzx.com

C#:   list.IndexOf(x);
来源：http://uxm.jinqigfzy.top

[D13] 过滤（保留满足条件的）
来源：http://btj.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ged.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rtb.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://zxs.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://nva.c1oappe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zpn.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tcq.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://bvs.wangshuangyany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hxn.yueranfly.top

[D14] 映射转换（每个元素变形）
来源：http://krd.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wjl.tarul.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wxe.hcnkem.com

JS:   arr.map(x => x * 2)
来源：http://vpz.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://lum.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pxe.xuetiantiany.cn

Go:   // 手写循环
来源：http://egi.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://mtp.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://bol.chenlongwang.top

[D15] 去重
来源：http://kyz.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ftl.svipenyu.cn

PHP:  array_unique($arr);
来源：http://jsx.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://vev.52xcode.cn

TS:   [...new Set(arr)]
来源：http://hgf.tianlin.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qce.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://dva.nanxuanxn.top

Ruby: arr.uniq
来源：http://vsu.cashguo.top

C#:   list.Distinct().ToList()
来源：http://cru.tarul.cn

[D16] 求和与平均值
来源：http://thc.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ixd.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zvc.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tdw.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxf.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://isc.dashuyun.cn

Go:   // 手写循环累加
来源：http://zgf.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://atg.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://bpr.iojbl.cn

[D17] 最大值与最小值
来源：http://upg.hammf.cn

Py:   max(arr);  min(arr)
来源：http://hbd.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://inw.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mmm.jqgfzy.top

TS:   Math.max(...arr);
来源：http://bwu.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kwn.wangshuangyany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gnp.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://kyw.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://ygo.9152youxi.cn

[D18] 扁平化嵌套数组
来源：http://vfc.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pds.zhijiandao.cn

PHP:  array_merge(...$nested);
来源：http://ubg.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kie.yanxiufei.cn

TS:   nested.flat();
来源：http://pdq.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xcr.fehbvm.com

Go:   // 手写双层循环
来源：http://oos.xylfe.cn

Ruby: nested.flatten
来源：http://dpl.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kbi.ehwqpu.com

[D19] 按字段分组
来源：http://vtr.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jlf.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qyb.yuanzhike.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kcs.zhoulong.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://nij.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ksl.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://sgi.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oug.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ocz.xylfe.cn

[D20] 统计每个元素出现次数
来源：http://smg.sxryk.cn

Py:   Counter(arr)
来源：http://mpq.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://dxn.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://piz.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cge.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wyv.mhx1999.top

Go:   // 手写 map[T]int
来源：http://ruc.0kj1m.cn

Ruby: arr.tally
来源：http://ibl.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://twe.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://qjb.yfazqb.com

Py:   x in arr
来源：http://sax.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://knn.xinyue.icu

JS:   arr.includes(x)
来源：http://bmr.meibo888.top

TS:   arr.includes(x)
来源：http://gdx.cheryme.top

Java: list.contains(x)
来源：http://uhq.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://mur.svipenyu.cn

Ruby: arr.include?(x)
来源：http://dgb.meibo888.top

C#:   list.Contains(x)
来源：http://ywh.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://cbl.andypj.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://omn.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fsm.shuidangran.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zyj.jinghuilouyu.cn

TS:   [...arr];
来源：http://dwq.jlsjyb.cn

Java: new ArrayList<>(list);
来源：http://zdc.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ilb.vehdjk.com

Ruby: arr.dup;  arr.clone
来源：http://bfa.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://hrr.shanyushiyangtech.top

[D23] reduce 累积计算
来源：http://rqb.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gea.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bmy.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zli.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gih.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pms.dashuyun.cn

Go:   // 手写循环
来源：http://xyi.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://teg.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://flx.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://ncg.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cwe.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yii.yj202588.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://thd.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ida.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxv.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eyi.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baw.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yqu.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://vkl.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://say.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vel.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gth.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://djk.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pfd.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rwh.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dwn.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zbx.zhoulong.xyz

[D26] 数组转字符串
来源：http://xwl.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://tik.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://xtx.zhoulong.xyz

JS:   arr.join(", ")
来源：http://vch.yfazqb.com

TS:   arr.join(", ")
来源：http://wje.9152youxi.cn

Java: String.join(", ", list)
来源：http://rgr.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://psn.hnqzz.top

Ruby: arr.join(", ")
来源：http://brb.yongpay.top

C#:   string.Join(", ", list)
来源：http://nbo.cucudq.cn

================================================================================
来源：http://exf.sxryk.cn

E. 字符串处理
来源：http://csi.nwbrower.top

================================================================================
来源：http://yxy.yj202588.top

[E01] 拼接字符串
来源：http://cuw.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xaf.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ozc.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://otc.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jkh.hnxiangtu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qqy.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rga.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://khf.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nnu.cqqwz.cn

[E02] 重复字符串
来源：http://ynj.cucudq.cn

Py:   "ab" * 3
来源：http://qcu.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://iik.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://tzj.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://hlv.9152youxi.cn

Java: "ab".repeat(3)
来源：http://yhn.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://xfi.sjlbkw.cn

Ruby: "ab" * 3
来源：http://vzx.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hoz.sxryk.cn

[E03] 截取子串
来源：http://ady.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jra.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xuz.aibaodan.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hhk.jinyuanbaomall.cn

TS:   s.slice(1, 4)
来源：http://wjv.gotoacloud.top

Java: s.substring(1, 4)
来源：http://jrx.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://txn.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://sjo.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://zve.cashguo.top

[E04] 查找子串位置
来源：http://ebu.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://byi.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://pbs.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gek.yuxming.cn

TS:   s.indexOf("x")
来源：http://oum.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://zxe.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://lbl.chenjidiqi.icu

Ruby: s.index("x")
来源：http://cmo.yongpay.top

C#:   s.IndexOf("x")
来源：http://lav.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://mzb.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zuz.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yhl.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zfd.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pua.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rla.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wwv.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://afe.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jkl.jqgfzy.top

[E06] 替换子串
来源：http://mfd.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nsj.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://qqf.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxr.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://rnk.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldq.vqdsnc.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wns.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fle.52xcode.cn

C#:   s.Replace("a", "b")
来源：http://fpq.bjfxy.top

[E07] 按分隔符拆分
来源：http://jxd.chenlongwang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://skq.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gcu.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vjy.vqdsnc.cn

TS:   s.split(",")
来源：http://hgt.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lky.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vsd.yongpay.top

Ruby: s.split(",");  s.split
来源：http://xwp.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lvf.52xcode.cn

[E08] 数组按分隔符合并
来源：http://cry.ehwqpu.com

Py:   ",".join(items)
来源：http://rvn.snrcjt.cn

PHP:  implode(",", $items);
来源：http://juy.tianlin.xyz

JS:   items.join(",")
来源：http://kri.ehwqpu.com

TS:   items.join(",")
来源：http://ybe.snrcjt.cn

Java: String.join(",", items)
来源：http://fnz.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://kxg.yuxming.cn

Ruby: items.join(",")
来源：http://pqv.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://fgi.jqgfzy.top

[E09] 去除所有空白字符
来源：http://tmr.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cxf.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://btw.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://cvt.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://jzf.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://afz.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lud.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://max.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jlk.yuanzhike.top


<!-- 参考信息 -->