代发 wailian999

D. 数组 / 列表 / 集合
来源：http://mmb.xuanzx.com

================================================================================
来源：http://pyv.xylfe.cn

[D01] 创建数组 / 列表
来源：http://brx.chenzaomai.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://btj.hysaishi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kje.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kzp.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zed.guannengcc.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ozr.wangshuangyany.cn

Go:   arr := []int{1, 2, 3}
来源：http://tlp.smart0.xyz

Ruby: arr = [1, 2, 3]
来源：http://vpw.smart0.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jyq.hnqzz.top

[D02] 追加元素到末尾
来源：http://bkf.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mdx.hysaishi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mev.hysaishi.cn

JS:   arr.push(4);
来源：http://cbu.zhiwuduotai.top

TS:   arr.push(4);
来源：http://sgz.haohaochexian.top

Java: list.add(4);
来源：http://ize.jinqigfzy.top

Go:   arr = append(arr, 4)
来源：http://lpt.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://cfz.pycfn.com

C#:   list.Add(4);
来源：http://stf.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://cog.hammf.cn

Py:   arr.insert(0, 0)
来源：http://spb.guowangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nzx.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ilq.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://qpv.yj202588.top

Java: list.add(0, 0);
来源：http://quy.shanyushiyangtech.top

Go:   arr = append([]int{0}, arr...)
来源：http://zqn.wangdashe.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fji.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://uzc.shuidangran.top

[D04] 删除元素
来源：http://msd.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xty.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zzx.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uja.fengsongda.top

TS:   arr.splice(0, 1);
来源：http://zby.yfazqb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bvs.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rkk.sxryk.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blh.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dwj.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://atj.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lkt.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kvt.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dws.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://xbw.shanyushiyangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://ito.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://fmo.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tvz.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pod.nanxinkj.top

[D06] 数组长度
来源：http://nat.jiagoushi.top

Py:   len(arr)
来源：http://bre.52xcode.cn

PHP:  count($arr);
来源：http://ioo.yongpay.top

JS:   arr.length
来源：http://ekt.tianlin.xyz

TS:   arr.length
来源：http://npa.c1oappe.top

Java: list.size();
来源：http://xnt.nwbrower.top

Go:   len(arr)
来源：http://boc.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://miy.yangfankeji.com

C#:   list.Count;
来源：http://vjh.feifeiyinyue.top

[D07] 切片 / 取子数组
来源：http://omb.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zpa.tarul.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ubw.fzhhl.top

JS:   arr.slice(1, 4);
来源：http://jea.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://gbg.dashuyun.cn

Java: list.subList(1, 4);
来源：http://udq.sufxvd.cn

Go:   arr[1:4]
来源：http://ebt.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://ldl.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://hne.shangyingyoupin.top

[D08] 合并两个数组
来源：http://bwx.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://ggb.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://oeu.zycfv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kvv.kuanghao11.cn

TS:   [...a, ...b];
来源：http://uzp.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://snp.yj20258.top

Go:   append(a, b...)
来源：http://qoz.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://pgt.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://fna.hesvh.cn

[D09] 排序（升序）
来源：http://bnq.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://uga.xinyue.icu

PHP:  sort($arr);
来源：http://slo.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jfc.xingfuxueyuan.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ywr.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ahc.tian-w.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vfx.shangyingyoupin.top

Ruby: arr.sort
来源：http://tur.vehdjk.com

C#:   list.Sort();
来源：http://hym.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://btn.tian-w.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zwk.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vpu.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tkw.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ykk.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qqe.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bkf.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jnb.yj20258888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qyi.hysaishi.cn

[D11] 反转数组
来源：http://bum.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://jrw.fengsongda.top

PHP:  array_reverse($arr);
来源：http://ioq.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wrl.havefunace.top

TS:   [...arr].reverse();
来源：http://tdx.yongpay.top

Java: Collections.reverse(list);
来源：http://ysm.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://evq.redwolf501.top

Ruby: arr.reverse
来源：http://zhn.daria6918.cn

C#:   list.Reverse();
来源：http://xjo.fzhhl.top

[D12] 查找元素下标
来源：http://qkr.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://rwh.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nau.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qlg.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qvw.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cuh.hnqzz.top

Go:   slices.Index(arr, x)
来源：http://krq.redwolf501.top

Ruby: arr.index(x)
来源：http://ywg.svipenyu.cn

C#:   list.IndexOf(x);
来源：http://xxm.tianlin.xyz

[D13] 过滤（保留满足条件的）
来源：http://dnp.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gzk.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gua.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://gaj.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://lez.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rij.jlsjyb.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xir.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://evq.aizwys.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xkm.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://ucp.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rzk.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mvc.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://vot.aibaodan.cn

TS:   arr.map(x => x * 2)
来源：http://ogx.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://noh.zhengqikj.top

Go:   // 手写循环
来源：http://jjv.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jzg.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bxk.cdnleiting.top

[D15] 去重
来源：http://tkq.gaohongyu789.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rlm.hfpthk.cn

PHP:  array_unique($arr);
来源：http://gwn.iojbl.cn

JS:   [...new Set(arr)]
来源：http://cwc.birdmap.top

TS:   [...new Set(arr)]
来源：http://paj.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sfz.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://dgj.guannengcc.top

Ruby: arr.uniq
来源：http://ymu.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://tkj.xziqi.cn

[D16] 求和与平均值
来源：http://cwn.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysp.havefunace.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xkv.gzhubu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://efp.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://itz.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wvl.yuxming.cn

Go:   // 手写循环累加
来源：http://rbl.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fnw.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://yus.yongpay.top

[D17] 最大值与最小值
来源：http://pqo.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://szx.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://sqm.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hsb.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://zru.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hng.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ttn.hysaishi.cn

Ruby: arr.max;  arr.min
来源：http://lji.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://bmk.uphjek.com

[D18] 扁平化嵌套数组
来源：http://ejt.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mjc.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://byx.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jca.zhixingplan.top

TS:   nested.flat();
来源：http://ghb.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bew.hesvh.cn

Go:   // 手写双层循环
来源：http://lcf.smart0.xyz

Ruby: nested.flatten
来源：http://xve.fktsv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lwa.redwolf501.top

[D19] 按字段分组
来源：http://uzj.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lqp.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vje.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ihl.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ier.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oon.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://bqf.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://npd.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://utx.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://ejt.pengpengdd.cyou

Py:   Counter(arr)
来源：http://hfv.daria6918.cn

PHP:  array_count_values($arr);
来源：http://dlx.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wux.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bej.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qsw.sjlbkw.cn

Go:   // 手写 map[T]int
来源：http://xos.ydzc1.top

Ruby: arr.tally
来源：http://qmb.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kqp.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://lhn.zdqjudy.top

Py:   x in arr
来源：http://kst.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://amu.uphjek.com

JS:   arr.includes(x)
来源：http://lbn.jqgufenzy.top

TS:   arr.includes(x)
来源：http://ixl.hongshengwenyu.top

Java: list.contains(x)
来源：http://ost.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://jht.svipenyu.cn

Ruby: arr.include?(x)
来源：http://fdu.bbcook.cn

C#:   list.Contains(x)
来源：http://nsm.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://htz.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://efo.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zhc.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qtj.jinghuilouyu.cn

TS:   [...arr];
来源：http://icg.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://yeu.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://qzn.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://ifr.sweek.top

C#:   new List<int>(list);
来源：http://nzn.tian-w.cn

[D23] reduce 累积计算
来源：http://vsu.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kcg.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sik.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bir.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hqb.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zmh.smart0.xyz

Go:   // 手写循环
来源：http://jfy.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vlx.gogol.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wlg.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://nns.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jzx.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dfu.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bqd.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://voc.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nsw.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gur.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fkd.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dre.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://gic.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lwk.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ijk.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hta.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zah.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://src.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gcs.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kwy.52xcode.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eov.xinyue.icu

[D26] 数组转字符串
来源：http://abb.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://aia.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://hcd.guannengcc.top

JS:   arr.join(", ")
来源：http://nzd.cheryme.top

TS:   arr.join(", ")
来源：http://pwe.ppjwa.cn

Java: String.join(", ", list)
来源：http://fjw.sweek.top

Go:   strings.Join(strs, ", ")
来源：http://zqe.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://jfk.ehwqpu.com

C#:   string.Join(", ", list)
来源：http://vqb.yfazqb.com

================================================================================
来源：http://wdm.pycfn.com

E. 字符串处理
来源：http://blr.shuidangran.top

================================================================================
来源：http://ouo.sjlbkw.cn

[E01] 拼接字符串
来源：http://vah.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qmf.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lyp.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fds.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lyk.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://elh.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vdh.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yli.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hmw.gaohongyu789.top

[E02] 重复字符串
来源：http://tci.yj20258.top

Py:   "ab" * 3
来源：http://sds.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://wxw.hcnkem.com

JS:   "ab".repeat(3)
来源：http://bdl.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://iyr.shuidangran.top

Java: "ab".repeat(3)
来源：http://ing.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://wtd.svipenyu.cn

Ruby: "ab" * 3
来源：http://qqn.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bxj.gaohongyu789.top

[E03] 截取子串
来源：http://kya.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zrn.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nhw.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mej.yj20258.top

TS:   s.slice(1, 4)
来源：http://kmx.gzhubu.top

Java: s.substring(1, 4)
来源：http://ihi.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fpa.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vrr.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://nnt.wangshuangyany.cn

[E04] 查找子串位置
来源：http://qgv.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://mjq.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://yta.jinyuanbaomall.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://anh.yfazqb.com

TS:   s.indexOf("x")
来源：http://jkj.52xcode.cn

Java: s.indexOf("x")
来源：http://uyc.cashguo.top

Go:   strings.Index(s, "x")
来源：http://iar.jyoumei.cn

Ruby: s.index("x")
来源：http://vxb.epnwcf.com

C#:   s.IndexOf("x")
来源：http://iuy.cdnleiting.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fug.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kld.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uhj.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uzq.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pei.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhp.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iej.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ujr.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qiy.zdqjudy.top

[E06] 替换子串
来源：http://rbc.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lfh.yueranfly.top

PHP:  str_replace("a", "b", $s);
来源：http://zas.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cws.aibaodan.cn

TS:   s.replaceAll("a", "b")
来源：http://nme.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://idp.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hut.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hrq.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://nhr.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://lgq.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hhe.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eox.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sbn.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://yty.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://mry.zdbjq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eif.wangshuangyany.cn


<!-- 参考信息 -->