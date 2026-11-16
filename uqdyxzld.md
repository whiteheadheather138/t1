代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jwg.gaohongyu789.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wws.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://dmi.zhijiandao.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ylh.sysykeji.top

Go:   arr := []int{1, 2, 3}
来源：http://grw.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://dam.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://grk.zhengqikj.top

[D02] 追加元素到末尾
来源：http://mxb.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://els.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://svz.cdnleiting.top

JS:   arr.push(4);
来源：http://szb.yonumen.top

TS:   arr.push(4);
来源：http://zwl.xuetiantiany.cn

Java: list.add(4);
来源：http://irp.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://pca.guannengcc.top

Ruby: arr << 4; arr.push(5)
来源：http://qcc.andypj.xyz

C#:   list.Add(4);
来源：http://xnl.xuetiantiany.cn

[D03] 在指定位置插入元素
来源：http://qsf.jianghu66.top

Py:   arr.insert(0, 0)
来源：http://ksb.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uyk.9152youxi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwr.gzhubu.top

TS:   arr.splice(0, 0, 0);
来源：http://oth.tianlin.xyz

Java: list.add(0, 0);
来源：http://fwp.gogol.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vmi.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://heq.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://bxb.ydzc1.top

[D04] 删除元素
来源：http://xmz.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gow.xingfuxueyuan.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tag.chenlongwang.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rxo.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://ozw.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kyx.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fyu.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pco.hammf.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ebs.havefunace.top

[D05] 访问与修改元素
来源：http://cpj.kuanghao11.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oys.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://txo.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bsy.gzhubu.top

TS:   arr[0]; arr.at(-1);
来源：http://lpx.feifeiyinyue.top

Java: list.get(0); list.set(0, 9);
来源：http://gbk.haohaochexian.top

Go:   arr[0]; arr[0] = 9
来源：http://ydy.sjlbkw.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jgv.vqdsnc.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://idp.snrcjt.cn

[D06] 数组长度
来源：http://lfl.gotoacloud.top

Py:   len(arr)
来源：http://fkc.hcnkem.com

PHP:  count($arr);
来源：http://vmd.kuanghao11.cn

JS:   arr.length
来源：http://tlz.quarkkingdee.top

TS:   arr.length
来源：http://epy.zhoulong.xyz

Java: list.size();
来源：http://hqm.zhijiandao.cn

Go:   len(arr)
来源：http://obv.yj202588.top

Ruby: arr.length; arr.size
来源：http://mdp.vehdjk.com

C#:   list.Count;
来源：http://xnv.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://uno.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://heg.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qpq.jqgfzy.top

JS:   arr.slice(1, 4);
来源：http://apf.quarkkingdee.top

TS:   arr.slice(1, 4);
来源：http://uif.yangfankeji.com

Java: list.subList(1, 4);
来源：http://epf.tarul.cn

Go:   arr[1:4]
来源：http://nty.9152youxi.cn

Ruby: arr[1, 3]
来源：http://rjm.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://kvx.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://zco.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://ejv.316326.xyz

PHP:  array_merge($a, $b);
来源：http://qci.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hll.sxryk.cn

TS:   [...a, ...b];
来源：http://aex.meibo888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bzt.zhiwuduotai.top

Go:   append(a, b...)
来源：http://yvc.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://ucv.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://wkr.andypj.xyz

[D09] 排序（升序）
来源：http://iey.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://sbm.snrcjt.cn

PHP:  sort($arr);
来源：http://hfv.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://sqd.jinqigfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kgw.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ryj.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sub.havefunace.top

Ruby: arr.sort
来源：http://obr.yuanzhike.top

C#:   list.Sort();
来源：http://kem.snrcjt.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mpm.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fot.hnqzz.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://alz.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ojb.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ryr.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hhh.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://umh.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hdt.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wpb.chenjidiqi.icu

[D11] 反转数组
来源：http://fjf.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://xzq.andypj.xyz

PHP:  array_reverse($arr);
来源：http://akb.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ljn.aibaodan.cn

TS:   [...arr].reverse();
来源：http://nui.daxiang520.top

Java: Collections.reverse(list);
来源：http://duc.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://zbi.52xcode.cn

Ruby: arr.reverse
来源：http://fsi.shangyingyoupin.top

C#:   list.Reverse();
来源：http://vbt.hcnkem.com

[D12] 查找元素下标
来源：http://ngq.birdmap.top

Py:   arr.index(x);  x in arr
来源：http://quc.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://thc.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cda.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sxc.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yai.cheryme.top

Go:   slices.Index(arr, x)
来源：http://ahn.cashguo.top

Ruby: arr.index(x)
来源：http://nel.epnwcf.com

C#:   list.IndexOf(x);
来源：http://kvv.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://mec.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yyg.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wzg.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://qrm.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://eju.xinyue.icu

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pan.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wsd.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://tgu.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wwc.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://cij.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xxa.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ubp.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://eoo.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://ctk.gotoacloud.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qro.jianghu66.top

Go:   // 手写循环
来源：http://aly.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://lzr.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pcy.sufxvd.cn

[D15] 去重
来源：http://dvy.dianchejie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wln.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://dow.fzhhl.top

JS:   [...new Set(arr)]
来源：http://kuq.yonumen.top

TS:   [...new Set(arr)]
来源：http://qss.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dgd.aibaodan.cn

Go:   // 用 map[T]struct{} 手写
来源：http://isl.vqdsnc.cn

Ruby: arr.uniq
来源：http://wct.wangdashe.top

C#:   list.Distinct().ToList()
来源：http://ddg.gaohongyu789.top

[D16] 求和与平均值
来源：http://ayk.shanyushiyangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eqc.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hnr.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ceh.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://izd.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zge.hesvh.cn

Go:   // 手写循环累加
来源：http://lzz.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wmd.daxiang520.top

C#:   list.Sum();  list.Average()
来源：http://koe.tanke756.top

[D17] 最大值与最小值
来源：http://ryc.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://kgs.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://vap.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ffa.xylfe.cn

TS:   Math.max(...arr);
来源：http://jok.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ygy.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://whe.yangfankeji.com

Ruby: arr.max;  arr.min
来源：http://myc.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://svb.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://ynu.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://szq.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://ygu.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ecx.wangshuangyany.cn

TS:   nested.flat();
来源：http://vtj.chenzaomai.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wxq.dashuyun.cn

Go:   // 手写双层循环
来源：http://wjb.9152youxi.cn

Ruby: nested.flatten
来源：http://krh.ivvv.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hew.jinghuilouyu.cn

[D19] 按字段分组
来源：http://aog.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yrj.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xpc.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://axu.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tuz.zhiwuduotai.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mnh.pengpengdd.cyou

Go:   // 手写 map[string][]T
来源：http://qbe.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lyc.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wfh.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://aoa.yuanzhike.top

Py:   Counter(arr)
来源：http://wfc.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://dov.quarkkingdee.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fcj.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lxy.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uln.sweek.top

Go:   // 手写 map[T]int
来源：http://iql.daria6918.cn

Ruby: arr.tally
来源：http://flj.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lmi.epnwcf.com

[D21] 判断是否包含某元素
来源：http://rit.shzxlz.cn

Py:   x in arr
来源：http://nna.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://kug.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://lqf.fktsv.cn

TS:   arr.includes(x)
来源：http://frf.vehdjk.com

Java: list.contains(x)
来源：http://mow.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://oit.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://qul.yonumen.top

C#:   list.Contains(x)
来源：http://wpa.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://snx.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hym.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://knd.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sji.hcnkem.com

TS:   [...arr];
来源：http://pkv.aizwys.cn

Java: new ArrayList<>(list);
来源：http://efv.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://uzg.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://xbn.jyoumei.cn

C#:   new List<int>(list);
来源：http://ygt.hongshengwenyu.top

[D23] reduce 累积计算
来源：http://tio.jinyuanbaomall.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gwi.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zrj.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://djf.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://huq.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mtg.chenjidiqi.icu

Go:   // 手写循环
来源：http://jik.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gmw.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ayx.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://zbr.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wfj.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tic.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://url.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://npb.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mqs.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bgd.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hst.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://akp.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://eix.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mcf.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lcw.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xni.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kbb.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nqu.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://izn.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pzk.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vfj.ivvv.top

[D26] 数组转字符串
来源：http://lfn.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://kdj.birdmap.top

PHP:  implode(", ", $arr);
来源：http://jdv.tian-w.cn

JS:   arr.join(", ")
来源：http://bqt.yangfankeji.com

TS:   arr.join(", ")
来源：http://mif.iojbl.cn

Java: String.join(", ", list)
来源：http://zjq.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://ozw.epnwcf.com

Ruby: arr.join(", ")
来源：http://onr.ivvv.top

C#:   string.Join(", ", list)
来源：http://rle.fanxiaobao.xyz

================================================================================
来源：http://oby.hfpthk.cn

E. 字符串处理
来源：http://ewo.sysykeji.top

================================================================================
来源：http://srz.epnwcf.com

[E01] 拼接字符串
来源：http://uca.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yso.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vwi.nwbrower.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixh.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ysp.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ygy.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bkt.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zos.bbcook.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ykp.cashguo.top

[E02] 重复字符串
来源：http://znj.fzhhl.top

Py:   "ab" * 3
来源：http://tvv.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://cyd.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://hzo.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://jdj.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://rhm.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://dnf.yuanzhike.top

Ruby: "ab" * 3
来源：http://ovn.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ydm.nwbrower.top

[E03] 截取子串
来源：http://ypr.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wlr.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://asj.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bue.birdmap.top

TS:   s.slice(1, 4)
来源：http://hku.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://wfx.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ofz.c1oappe.top

Ruby: s[1, 3];  s[1..3]
来源：http://rje.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://zcl.yfazqb.com

[E04] 查找子串位置
来源：http://pjy.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://gac.hesvh.cn

PHP:  strpos($s, "x");
来源：http://yvf.shangyingyoupin.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bfc.shzxlz.cn

TS:   s.indexOf("x")
来源：http://pbg.jqgfzy.top

Java: s.indexOf("x")
来源：http://svc.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://lzt.svipenyu.cn

Ruby: s.index("x")
来源：http://udw.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://bih.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vsn.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rfc.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kmp.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bpf.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zet.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cte.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jqv.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hmo.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wnw.xylfe.cn

[E06] 替换子串
来源：http://auw.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fab.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://jvf.tarul.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hni.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://rnw.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ger.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tjx.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mcv.yj202588.top

C#:   s.Replace("a", "b")
来源：http://rfk.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://dot.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eop.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kvo.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://jce.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://lsc.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://bow.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dse.tanke756.top

Ruby: s.split(",");  s.split
来源：http://vyc.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ers.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://spr.hfpthk.cn

Py:   ",".join(items)
来源：http://ppy.316326.xyz


<!-- 参考信息 -->