代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sqi.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qrx.shanyushiyangtech.top

JS:   arr.push(4);
来源：http://vrt.gogol.net.cn

TS:   arr.push(4);
来源：http://eoc.xziqi.cn

Java: list.add(4);
来源：http://qqi.bjfxy.top

Go:   arr = append(arr, 4)
来源：http://aqg.xinyue.icu

Ruby: arr << 4; arr.push(5)
来源：http://lah.zhixingplan.top

C#:   list.Add(4);
来源：http://pnw.ydzc1.top

[D03] 在指定位置插入元素
来源：http://uad.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://phw.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gve.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hju.tanke756.top

TS:   arr.splice(0, 0, 0);
来源：http://axe.9152youxi.cn

Java: list.add(0, 0);
来源：http://kke.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://kdo.yj202588.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ckj.uphjek.com

C#:   list.Insert(0, 0);
来源：http://hca.bbcook.cn

[D04] 删除元素
来源：http://sra.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sas.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gwz.daria6918.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xpx.hywenlv.cn

TS:   arr.splice(0, 1);
来源：http://lao.hesvh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vzr.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vqw.yonumen.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://plv.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fqy.sjlbkw.cn

[D05] 访问与修改元素
来源：http://eit.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wld.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hfb.fengsongda.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yxc.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://rqc.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://szm.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://dyj.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vnc.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jej.hnxiangtu.top

[D06] 数组长度
来源：http://ipg.guannengcc.top

Py:   len(arr)
来源：http://vzy.daria6918.cn

PHP:  count($arr);
来源：http://rqp.birdmap.top

JS:   arr.length
来源：http://rdp.fanxiaobao.xyz

TS:   arr.length
来源：http://onv.jianghu66.top

Java: list.size();
来源：http://rkh.fengsongda.top

Go:   len(arr)
来源：http://hxk.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://qfe.ybcxt.top

C#:   list.Count;
来源：http://cjq.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://qct.yj20258.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://isj.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://beq.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://bce.cashguo.top

TS:   arr.slice(1, 4);
来源：http://zdt.yueranfly.top

Java: list.subList(1, 4);
来源：http://eeb.0kj1m.cn

Go:   arr[1:4]
来源：http://vfo.smart0.xyz

Ruby: arr[1, 3]
来源：http://xtg.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://dxt.daria6918.cn

[D08] 合并两个数组
来源：http://qbf.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://pkp.tarul.cn

PHP:  array_merge($a, $b);
来源：http://gto.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rxj.birdmap.top

TS:   [...a, ...b];
来源：http://jth.snrcjt.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xye.chenzaomai.com

Go:   append(a, b...)
来源：http://bry.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://gmt.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://wim.jyoumei.cn

[D09] 排序（升序）
来源：http://cfb.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://igp.bbcook.cn

PHP:  sort($arr);
来源：http://wei.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qlc.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://erc.hammf.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kth.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nic.aibaodan.cn

Ruby: arr.sort
来源：http://yap.xuetiantiany.cn

C#:   list.Sort();
来源：http://nje.quarkkingdee.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zgp.haohaochexian.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://duv.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ull.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gxq.ehwqpu.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vnh.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://def.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cze.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://des.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wev.meibo888.top

[D11] 反转数组
来源：http://bqd.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://gtk.jinyuanbaomall.cn

PHP:  array_reverse($arr);
来源：http://ajw.fehbvm.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ezx.tian-w.cn

TS:   [...arr].reverse();
来源：http://cnu.yongpay.top

Java: Collections.reverse(list);
来源：http://klh.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://ogb.cheryme.top

Ruby: arr.reverse
来源：http://ztr.hywenlv.cn

C#:   list.Reverse();
来源：http://bae.hammf.cn

[D12] 查找元素下标
来源：http://eyp.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://sal.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cwz.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bvv.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqj.uphjek.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rkn.gogol.net.cn

Go:   slices.Index(arr, x)
来源：http://klg.hysaishi.cn

Ruby: arr.index(x)
来源：http://rug.yfazqb.com

C#:   list.IndexOf(x);
来源：http://tva.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://znq.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cxc.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ilo.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://qwc.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://vqs.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gcb.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://odq.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://icp.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://myn.fehbvm.com

[D14] 映射转换（每个元素变形）
来源：http://fzf.xuanzx.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wcw.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zpd.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://jtf.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://lgu.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xlz.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://gmk.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zng.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ifp.epnwcf.com

[D15] 去重
来源：http://mno.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sck.shuidangran.top

PHP:  array_unique($arr);
来源：http://vzg.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://hnj.redwolf501.top

TS:   [...new Set(arr)]
来源：http://keo.nanxinkj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://iun.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://ylj.zdbjq.cn

Ruby: arr.uniq
来源：http://zvw.pycfn.com

C#:   list.Distinct().ToList()
来源：http://uaw.redwolf501.top

[D16] 求和与平均值
来源：http://owm.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ifl.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pzd.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rex.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rkx.zhixingplan.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wbv.aibaodan.cn

Go:   // 手写循环累加
来源：http://rby.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wna.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://sgy.tian-w.cn

[D17] 最大值与最小值
来源：http://sov.quarkkingdee.top

Py:   max(arr);  min(arr)
来源：http://vuz.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://fhn.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nqm.hysaishi.cn

TS:   Math.max(...arr);
来源：http://pqo.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://imv.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://foz.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://rqk.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://dzq.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://wnk.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://duq.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://cwp.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rbf.c1oappe.top

TS:   nested.flat();
来源：http://nwf.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cet.svipenyu.cn

Go:   // 手写双层循环
来源：http://imx.andypj.xyz

Ruby: nested.flatten
来源：http://mib.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tyy.kuanghao11.cn

[D19] 按字段分组
来源：http://nup.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rlx.shangyingyoupin.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://duv.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jco.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hhl.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hur.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://tyc.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xmf.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unq.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://gfl.zhoulong.xyz

Py:   Counter(arr)
来源：http://ald.daxiang520.top

PHP:  array_count_values($arr);
来源：http://gmd.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ivw.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zfx.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ylf.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://oio.jianghu66.top

Ruby: arr.tally
来源：http://tcn.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cdc.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://lrx.ybcxt.top

Py:   x in arr
来源：http://kmk.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://zwh.redwolf501.top

JS:   arr.includes(x)
来源：http://edg.hnqzz.top

TS:   arr.includes(x)
来源：http://uwf.chenlongwang.top

Java: list.contains(x)
来源：http://bos.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://btg.daxiang520.top

Ruby: arr.include?(x)
来源：http://oxt.svipenyu.cn

C#:   list.Contains(x)
来源：http://rfd.shangyingyoupin.top

[D22] 复制数组（避免共享引用）
来源：http://kwu.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wfd.wangdashe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zlq.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ugs.cucudq.cn

TS:   [...arr];
来源：http://ase.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://krq.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://jxf.gotoacloud.top

Ruby: arr.dup;  arr.clone
来源：http://nsq.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://ypi.gotoacloud.top

[D23] reduce 累积计算
来源：http://rrt.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aov.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mwt.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhz.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aue.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://loy.ctjpmb.com

Go:   // 手写循环
来源：http://rwi.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ctg.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hmx.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://xzf.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bcr.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fje.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://khy.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qrx.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ypv.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tlm.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twm.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hfp.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://esn.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://air.shuidangran.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lii.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://msj.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mmz.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ddy.zhixingplan.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gvv.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uqc.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qey.gzhubu.top

[D26] 数组转字符串
来源：http://rtz.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://urc.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://ela.hysaishi.cn

JS:   arr.join(", ")
来源：http://nwh.fktsv.cn

TS:   arr.join(", ")
来源：http://jvi.zhongyouzk.top

Java: String.join(", ", list)
来源：http://oye.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://ynh.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://cna.xuanzx.com

C#:   string.Join(", ", list)
来源：http://qsb.fanxiaobao.xyz

================================================================================
来源：http://kzw.nanxinkj.top

E. 字符串处理
来源：http://qnr.tanke756.top

================================================================================
来源：http://djm.jinqigfzy.top

[E01] 拼接字符串
来源：http://xkv.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tqj.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpo.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://unm.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fyh.jqgufenzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fjb.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://awz.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wgt.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://svz.fzhhl.top

[E02] 重复字符串
来源：http://its.jinqigufen.top

Py:   "ab" * 3
来源：http://jlm.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://zzb.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://qjb.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://vqt.chenzaomai.com

Java: "ab".repeat(3)
来源：http://idn.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://dir.cdnleiting.top

Ruby: "ab" * 3
来源：http://lwm.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jjz.zhixingplan.top

[E03] 截取子串
来源：http://tbm.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yel.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bus.gzhubu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sly.havefunace.top

TS:   s.slice(1, 4)
来源：http://nmg.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://akq.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gap.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://rkl.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://nng.jlsjyb.cn

[E04] 查找子串位置
来源：http://lzs.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://lkp.yj202588.top

PHP:  strpos($s, "x");
来源：http://kvv.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gsj.shzxlz.cn

TS:   s.indexOf("x")
来源：http://uml.hnxiangtu.top

Java: s.indexOf("x")
来源：http://pfz.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://wgv.ctjpmb.com

Ruby: s.index("x")
来源：http://jvw.jianghu66.top

C#:   s.IndexOf("x")
来源：http://qrk.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vgr.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uis.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ssb.bjfxy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfj.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mdy.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://haf.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jwf.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nhz.ctjpmb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wmg.kuanghao11.cn

[E06] 替换子串
来源：http://sas.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vfw.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://apc.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qzu.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://wsg.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://igc.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pts.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lva.hammf.cn

C#:   s.Replace("a", "b")
来源：http://eje.tanke756.top

[E07] 按分隔符拆分
来源：http://xuk.cashguo.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sxf.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ugo.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://cos.kuanghao11.cn

TS:   s.split(",")
来源：http://ebh.jinqigfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://yiv.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://boj.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://tvd.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lve.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://nwg.zhengqikj.top

Py:   ",".join(items)
来源：http://iho.sweek.top

PHP:  implode(",", $items);
来源：http://qdq.zdqjudy.top

JS:   items.join(",")
来源：http://tds.yj20258.top

TS:   items.join(",")
来源：http://uoo.dianchejie.cn

Java: String.join(",", items)
来源：http://ewu.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://kaj.havefunace.top

Ruby: items.join(",")
来源：http://plz.ctjpmb.com

C#:   string.Join(",", items)
来源：http://dmv.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://wdt.feifeiyinyue.top


<!-- 参考信息 -->