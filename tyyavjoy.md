代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://puc.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://avv.hnqzz.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://bxq.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qsz.chenjidiqi.icu

Go:   arr := []int{1, 2, 3}
来源：http://wcd.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://bxt.yongpay.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://usf.yvedp.cn

[D02] 追加元素到末尾
来源：http://yny.ehwqpu.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wrb.fanxiaobao.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yds.cheryme.top

JS:   arr.push(4);
来源：http://gik.aizwys.cn

TS:   arr.push(4);
来源：http://yaz.tarul.cn

Java: list.add(4);
来源：http://vhm.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://aib.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://wym.gotoacloud.top

C#:   list.Add(4);
来源：http://pfv.jqgufenzy.top

[D03] 在指定位置插入元素
来源：http://mwj.ivvv.top

Py:   arr.insert(0, 0)
来源：http://usr.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pia.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fio.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://aah.cucudq.cn

Java: list.add(0, 0);
来源：http://gou.shangyingyoupin.top

Go:   arr = append([]int{0}, arr...)
来源：http://fcn.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ogt.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://ibg.quarkkingdee.top

[D04] 删除元素
来源：http://ibe.epnwcf.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bed.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uxn.xinyue.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cao.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://pkj.uphjek.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pui.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rou.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tmj.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sjr.haohaochexian.top

[D05] 访问与修改元素
来源：http://ubc.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vos.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jhy.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://psu.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://cdy.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://mza.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://bhe.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uwg.xuetiantiany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dzw.wangshuangyany.cn

[D06] 数组长度
来源：http://ppd.hywenlv.cn

Py:   len(arr)
来源：http://nbh.bbcook.cn

PHP:  count($arr);
来源：http://rvq.ydzc1.top

JS:   arr.length
来源：http://qni.ywan-chungtsiang.top

TS:   arr.length
来源：http://xuy.xingfuxueyuan.xyz

Java: list.size();
来源：http://iqk.bjfxy.top

Go:   len(arr)
来源：http://jxh.bbcook.cn

Ruby: arr.length; arr.size
来源：http://wox.pycfn.com

C#:   list.Count;
来源：http://lmh.birdmap.top

[D07] 切片 / 取子数组
来源：http://qaw.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vcm.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oqm.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://zdh.cucudq.cn

TS:   arr.slice(1, 4);
来源：http://lqe.zdqjudy.top

Java: list.subList(1, 4);
来源：http://iac.hesvh.cn

Go:   arr[1:4]
来源：http://qjt.cqqwz.cn

Ruby: arr[1, 3]
来源：http://dsd.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://gsc.jqgfzy.top

[D08] 合并两个数组
来源：http://irs.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://yqk.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://hyx.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nfa.gogol.net.cn

TS:   [...a, ...b];
来源：http://zeg.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ljo.daria6918.cn

Go:   append(a, b...)
来源：http://osm.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://ktg.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://cxd.yj20258888.top

[D09] 排序（升序）
来源：http://pqq.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://qyl.fehbvm.com

PHP:  sort($arr);
来源：http://uuh.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://han.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://gca.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ghu.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://idf.pycfn.com

Ruby: arr.sort
来源：http://bdz.shzxlz.cn

C#:   list.Sort();
来源：http://cll.ivvv.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mfu.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pdo.xylfe.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ljk.jinyuanbaomall.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ecs.mhx1999.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nrc.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gub.yvedp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ldg.52xcode.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bgj.tanke756.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kon.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://idg.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://voj.xziqi.cn

PHP:  array_reverse($arr);
来源：http://qvu.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iqe.ehwqpu.com

TS:   [...arr].reverse();
来源：http://qvx.sweek.top

Java: Collections.reverse(list);
来源：http://ccv.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://kci.c1oappe.top

Ruby: arr.reverse
来源：http://isg.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://bpp.0kj1m.cn

[D12] 查找元素下标
来源：http://kpe.smart0.xyz

Py:   arr.index(x);  x in arr
来源：http://fla.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://goq.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gej.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uhf.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://prv.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://xgc.tian-w.cn

Ruby: arr.index(x)
来源：http://ttp.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://toc.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://pwg.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tmj.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rqn.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://ljo.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://aio.zhaomingkeji.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gxk.hongshengwenyu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zfl.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xpt.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://vfd.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://xup.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wnn.gaohongyu789.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ipv.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://ldz.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://wyz.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vmi.yvedp.cn

Go:   // 手写循环
来源：http://olb.xinyue.icu

Ruby: arr.map { |x| x * 2 }
来源：http://ind.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ffw.aibaodan.cn

[D15] 去重
来源：http://fyr.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rny.hysaishi.cn

PHP:  array_unique($arr);
来源：http://bib.xylfe.cn

JS:   [...new Set(arr)]
来源：http://ryh.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://dik.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vhg.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zyp.yvedp.cn

Ruby: arr.uniq
来源：http://fpr.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://hyx.zhixingplan.top

[D16] 求和与平均值
来源：http://uug.tanke756.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nnq.bbcook.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ejq.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kzs.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://obw.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zav.xinyue.icu

Go:   // 手写循环累加
来源：http://aai.haohaochexian.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bir.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://nkh.shuidangran.top

[D17] 最大值与最小值
来源：http://txw.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://trw.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://bwk.jiagoushi.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ztw.jianghu66.top

TS:   Math.max(...arr);
来源：http://dxs.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bhq.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://orf.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://bua.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://skp.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://fgz.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tij.cashguo.top

PHP:  array_merge(...$nested);
来源：http://mpr.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ccg.jianghu66.top

TS:   nested.flat();
来源：http://xgr.jinqigfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dzg.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://lks.fehbvm.com

Ruby: nested.flatten
来源：http://eio.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ivz.ppjwa.cn

[D19] 按字段分组
来源：http://oqi.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bgd.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://thw.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qno.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://suy.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ndc.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://lan.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lsl.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dih.316326.xyz

[D20] 统计每个元素出现次数
来源：http://ujr.ydjk.org.cn

Py:   Counter(arr)
来源：http://dqx.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://tuf.uphjek.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tou.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://auo.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nya.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://mdd.xylfe.cn

Ruby: arr.tally
来源：http://lwq.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sga.nwbrower.top

[D21] 判断是否包含某元素
来源：http://hzt.jinghuilouyu.cn

Py:   x in arr
来源：http://nzi.jqgfzy.top

PHP:  in_array($x, $arr, true);
来源：http://wgx.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://gcp.yj20258.top

TS:   arr.includes(x)
来源：http://ywx.zhongyouzk.top

Java: list.contains(x)
来源：http://qjx.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://ifd.guannengcc.top

Ruby: arr.include?(x)
来源：http://ucq.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://uoj.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://fjv.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iro.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ent.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ejw.aizwys.cn

TS:   [...arr];
来源：http://ptx.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://yro.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xvy.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://ykv.epnwcf.com

C#:   new List<int>(list);
来源：http://pgs.xziqi.cn

[D23] reduce 累积计算
来源：http://ffz.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://caa.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bmo.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdc.zhoulong.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abo.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://qph.gogol.net.cn

Go:   // 手写循环
来源：http://swt.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lum.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://soq.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://skq.ywan-chungtsiang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://odk.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://utb.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://krj.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jel.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rll.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qgz.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ciq.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ano.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://fig.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eou.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pgl.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ijg.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qbf.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://smu.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qqo.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vys.tian-w.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hwv.guowangkeji.top

[D26] 数组转字符串
来源：http://ugs.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://ypq.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://pzb.shuidangran.top

JS:   arr.join(", ")
来源：http://arb.andypj.xyz

TS:   arr.join(", ")
来源：http://xhn.sufxvd.cn

Java: String.join(", ", list)
来源：http://ntd.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://qmu.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://hno.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://ugs.vehdjk.com

================================================================================
来源：http://xzy.smart0.xyz

E. 字符串处理
来源：http://ybc.feifeiyinyue.top

================================================================================
来源：http://ggn.dianchejie.cn

[E01] 拼接字符串
来源：http://uho.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwu.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zaa.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nqd.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hys.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jwl.xinyue.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://owh.shzxlz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zya.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wfs.yuxming.cn

[E02] 重复字符串
来源：http://yzm.ybcxt.top

Py:   "ab" * 3
来源：http://jpr.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://dxo.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://dmg.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://wce.aizwys.cn

Java: "ab".repeat(3)
来源：http://jyt.zhoulong.xyz

Go:   strings.Repeat("ab", 3)
来源：http://jqm.svipenyu.cn

Ruby: "ab" * 3
来源：http://efp.pycfn.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yyf.kuanghao11.cn

[E03] 截取子串
来源：http://mda.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ity.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fgn.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aso.yongpay.top

TS:   s.slice(1, 4)
来源：http://awj.dashuyun.cn

Java: s.substring(1, 4)
来源：http://aeu.shzxlz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uyd.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://rrx.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://jkz.zdqjudy.top

[E04] 查找子串位置
来源：http://isn.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://ebh.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://prk.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nvn.redwolf501.top

TS:   s.indexOf("x")
来源：http://zgd.gotoacloud.top

Java: s.indexOf("x")
来源：http://zrl.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://ckd.jiagoushi.top

Ruby: s.index("x")
来源：http://wmi.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://lly.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ojc.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://azt.yfazqb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yqv.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ehc.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hhg.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ral.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jfv.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://urq.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jhu.9152youxi.cn

[E06] 替换子串
来源：http://prk.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jaf.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://ita.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cof.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://ifp.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xcf.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lyj.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hov.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://zzj.chenlongwang.top

[E07] 按分隔符拆分
来源：http://fas.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qer.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vrp.bjfxy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nws.jinghuilouyu.cn

TS:   s.split(",")
来源：http://mrj.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fex.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mhu.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://eul.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pyd.yj202588.top

[E08] 数组按分隔符合并
来源：http://xvh.birdmap.top

Py:   ",".join(items)
来源：http://qdf.iojbl.cn


<!-- 参考信息 -->