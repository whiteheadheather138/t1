代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://fst.chenjidiqi.icu

Java: list.add(0, 0);
来源：http://hrb.gotoacloud.top

Go:   arr = append([]int{0}, arr...)
来源：http://giv.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xvi.nwbrower.top

C#:   list.Insert(0, 0);
来源：http://uuw.yj20258.top

[D04] 删除元素
来源：http://zwk.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cbh.wangshuangyany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hfl.iojbl.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://run.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://axs.zhaomingkeji.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://epp.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wmv.vehdjk.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://utm.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jbr.yj20258888.top

[D05] 访问与修改元素
来源：http://kje.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tdp.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bvv.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bvk.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://gqb.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://nra.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://dsi.yongpay.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kpp.yuanzhike.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fyu.smart0.xyz

[D06] 数组长度
来源：http://gwl.tianlin.xyz

Py:   len(arr)
来源：http://jba.ctjpmb.com

PHP:  count($arr);
来源：http://ota.cashguo.top

JS:   arr.length
来源：http://qvs.hysaishi.cn

TS:   arr.length
来源：http://jko.cdnleiting.top

Java: list.size();
来源：http://fwc.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://eyn.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://ukd.jinqigufen.top

C#:   list.Count;
来源：http://pim.hammf.cn

[D07] 切片 / 取子数组
来源：http://vmt.hnxiangtu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jeu.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://lki.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://ykj.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://qml.bjfxy.top

Java: list.subList(1, 4);
来源：http://ojp.andypj.xyz

Go:   arr[1:4]
来源：http://tlo.shzxlz.cn

Ruby: arr[1, 3]
来源：http://wnn.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://ovt.gzhubu.top

[D08] 合并两个数组
来源：http://clp.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://sly.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://qvc.jinyuanbaomall.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bex.jqgfzy.top

TS:   [...a, ...b];
来源：http://rne.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hpp.ybcxt.top

Go:   append(a, b...)
来源：http://eve.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://xsl.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://ffr.xinyue.icu

[D09] 排序（升序）
来源：http://ixk.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://noo.yfazqb.com

PHP:  sort($arr);
来源：http://ahv.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oqb.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://imv.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qye.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jkd.dashuyun.cn

Ruby: arr.sort
来源：http://ish.jiagoushi.top

C#:   list.Sort();
来源：http://kax.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://otk.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nma.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dbn.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dum.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pbb.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nvp.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://otg.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fhh.yongpay.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cuy.yj20258.top

[D11] 反转数组
来源：http://qtc.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://zyz.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://ilx.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hao.tarul.cn

TS:   [...arr].reverse();
来源：http://rkl.cdnleiting.top

Java: Collections.reverse(list);
来源：http://pue.zhaomingkeji.xyz

Go:   slices.Reverse(arr)
来源：http://gik.birdmap.top

Ruby: arr.reverse
来源：http://qar.ybcxt.top

C#:   list.Reverse();
来源：http://dxj.zhengqikj.top

[D12] 查找元素下标
来源：http://drt.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://tbb.xziqi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zsi.shanyushiyangkeji.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://udy.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vrf.hywenlv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cix.wangdashe.top

Go:   slices.Index(arr, x)
来源：http://dxh.svipenyu.cn

Ruby: arr.index(x)
来源：http://dpd.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://sog.yongpay.top

[D13] 过滤（保留满足条件的）
来源：http://jxg.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qsr.xziqi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gkd.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://mfh.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://xgl.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tbu.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ygg.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://ebv.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gma.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://ulm.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pmg.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aob.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://bai.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://zxt.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://nei.jianghu66.top

Go:   // 手写循环
来源：http://jng.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eys.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://tqy.ctjpmb.com

[D15] 去重
来源：http://hrn.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qsa.52xcode.cn

PHP:  array_unique($arr);
来源：http://npd.bjfxy.top

JS:   [...new Set(arr)]
来源：http://pmw.xuanzx.com

TS:   [...new Set(arr)]
来源：http://gfk.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wef.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iaw.hnxiangtu.top

Ruby: arr.uniq
来源：http://lha.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://wti.daxiang520.top

[D16] 求和与平均值
来源：http://zeu.redwolf501.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jrn.guowangkeji.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tcr.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://btr.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wof.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bsr.bjfxy.top

Go:   // 手写循环累加
来源：http://rzm.yuxming.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gif.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://afb.tarul.cn

[D17] 最大值与最小值
来源：http://dyt.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://juo.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://iep.jlsjyb.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bpb.dashuyun.cn

TS:   Math.max(...arr);
来源：http://znd.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://irz.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dbe.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://nkp.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://umy.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://uke.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qda.gogol.net.cn

PHP:  array_merge(...$nested);
来源：http://rvl.ywan-chungtsiang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wuz.hysaishi.cn

TS:   nested.flat();
来源：http://ggf.hongshengwenyu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kkj.zhaomingkeji.xyz

Go:   // 手写双层循环
来源：http://qky.epnwcf.com

Ruby: nested.flatten
来源：http://gjf.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://svv.wangdashe.top

[D19] 按字段分组
来源：http://wcd.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wjs.gaohongyu789.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aso.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nva.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zwx.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yck.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://itn.jinqigufen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qbf.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dqx.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://epg.zhiwuduotai.top

Py:   Counter(arr)
来源：http://tot.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://oru.cdnleiting.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zdg.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lse.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bic.yongpay.top

Go:   // 手写 map[T]int
来源：http://wsy.c1oappe.top

Ruby: arr.tally
来源：http://jnl.yvedp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pgo.xuetiantiany.cn

[D21] 判断是否包含某元素
来源：http://zau.kuanghao11.cn

Py:   x in arr
来源：http://ase.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://inu.yuxming.cn

JS:   arr.includes(x)
来源：http://evh.nanxinkj.top

TS:   arr.includes(x)
来源：http://gia.sjlbkw.cn

Java: list.contains(x)
来源：http://but.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://cqo.yuxming.cn

Ruby: arr.include?(x)
来源：http://suc.hysaishi.cn

C#:   list.Contains(x)
来源：http://dts.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://psn.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uzq.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mpb.sxryk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cqs.chenlongwang.top

TS:   [...arr];
来源：http://hkq.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://jfp.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://bch.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://ixy.iojbl.cn

C#:   new List<int>(list);
来源：http://cmi.ppjwa.cn

[D23] reduce 累积计算
来源：http://sem.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yef.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eaw.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://olj.snrcjt.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mdk.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uhd.fehbvm.com

Go:   // 手写循环
来源：http://ywi.yuanzhike.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zxt.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gfz.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://sut.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://czb.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lyo.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tsb.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ahu.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ltg.bbcook.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tzu.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rws.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pfw.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://obg.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rrh.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rsh.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qga.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jvc.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mau.hesvh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tyu.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lmk.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oto.dianchejie.cn

[D26] 数组转字符串
来源：http://ekb.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://odq.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://ika.chenzaomai.com

JS:   arr.join(", ")
来源：http://bhr.hcnkem.com

TS:   arr.join(", ")
来源：http://axr.quarkkingdee.top

Java: String.join(", ", list)
来源：http://ijc.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://bqe.gogol.net.cn

Ruby: arr.join(", ")
来源：http://ujg.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://ccv.uphjek.com

================================================================================
来源：http://lgy.hysaishi.cn

E. 字符串处理
来源：http://ixg.shzxlz.cn

================================================================================
来源：http://xho.cashguo.top

[E01] 拼接字符串
来源：http://njz.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rxd.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zxp.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gvp.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://udp.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lhb.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zgx.yj202588.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nmr.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://odt.wangshuangyany.cn

[E02] 重复字符串
来源：http://cdl.daria6918.cn

Py:   "ab" * 3
来源：http://pop.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://pej.cucudq.cn

JS:   "ab".repeat(3)
来源：http://lii.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://pvl.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://hqd.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://mlq.jlsjyb.cn

Ruby: "ab" * 3
来源：http://jcm.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nlr.jyoumei.cn

[E03] 截取子串
来源：http://zkd.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jbi.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fea.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ptc.52xcode.cn

TS:   s.slice(1, 4)
来源：http://dyb.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://kwk.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rtc.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://iiu.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://xuv.gaohongyu789.top

[E04] 查找子串位置
来源：http://utx.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://naa.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://omn.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nwk.jinqigufen.top

TS:   s.indexOf("x")
来源：http://cgt.fktsv.cn

Java: s.indexOf("x")
来源：http://wuk.tian-w.cn

Go:   strings.Index(s, "x")
来源：http://gqn.feifeiyinyue.top

Ruby: s.index("x")
来源：http://lwn.hammf.cn

C#:   s.IndexOf("x")
来源：http://edg.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kae.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zwd.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eoc.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bwu.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uib.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cxy.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vcq.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aui.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bdv.hesvh.cn

[E06] 替换子串
来源：http://pky.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iec.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://vbx.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bym.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://obz.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gfl.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ecp.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eqa.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://hif.fengsongda.top

[E07] 按分隔符拆分
来源：http://jjb.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lzk.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://evv.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dak.guannengcc.top

TS:   s.split(",")
来源：http://bhp.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fii.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tnu.xingfuxueyuan.xyz

Ruby: s.split(",");  s.split
来源：http://sqe.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fjo.redwolf501.top

[E08] 数组按分隔符合并
来源：http://lej.gzhubu.top

Py:   ",".join(items)
来源：http://cqd.pycfn.com

PHP:  implode(",", $items);
来源：http://huo.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://gcu.jqgufenzy.top

TS:   items.join(",")
来源：http://eyo.aibaodan.cn

Java: String.join(",", items)
来源：http://ggq.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://oyz.xylfe.cn

Ruby: items.join(",")
来源：http://mqo.tian-w.cn

C#:   string.Join(",", items)
来源：http://bym.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://jsl.sufxvd.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hky.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bjx.hfpthk.cn

JS:   s.replace(/\s+/g, "")
来源：http://pzy.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ahm.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://ydc.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ppk.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ygz.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://obv.sufxvd.cn

[E10] 左侧补零 / 定长填充
来源：http://xji.zhixingplan.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://avr.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qac.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://raq.gzhubu.top


<!-- 参考信息 -->