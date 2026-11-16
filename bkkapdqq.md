代发 wailian999

Java: list.add(4);
来源：http://qru.yj20258.top

Go:   arr = append(arr, 4)
来源：http://ofx.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://qae.yj202588.top

C#:   list.Add(4);
来源：http://zoz.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://rrs.ppjwa.cn

Py:   arr.insert(0, 0)
来源：http://fmv.quarkkingdee.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zre.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qmf.pengpengdd.cyou

TS:   arr.splice(0, 0, 0);
来源：http://nbz.tian-w.cn

Java: list.add(0, 0);
来源：http://dwe.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://nsc.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vhl.jiagoushi.top

C#:   list.Insert(0, 0);
来源：http://xmm.aibaodan.cn

[D04] 删除元素
来源：http://pmi.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lfj.ydzc1.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zwk.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kuj.316326.xyz

TS:   arr.splice(0, 1);
来源：http://jaq.jqgfzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ycw.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rdk.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jpz.fehbvm.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cph.zdqjudy.top

[D05] 访问与修改元素
来源：http://inq.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lht.ywan-chungtsiang.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gem.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cwv.pycfn.com

TS:   arr[0]; arr.at(-1);
来源：http://pae.ppjwa.cn

Java: list.get(0); list.set(0, 9);
来源：http://veg.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://cnc.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xvm.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mwz.sufxvd.cn

[D06] 数组长度
来源：http://pca.gogol.net.cn

Py:   len(arr)
来源：http://vzo.xylfe.cn

PHP:  count($arr);
来源：http://zmt.dashuyun.cn

JS:   arr.length
来源：http://nrm.feifeiyinyue.top

TS:   arr.length
来源：http://gsk.smart0.xyz

Java: list.size();
来源：http://tjx.ywan-chungtsiang.top

Go:   len(arr)
来源：http://ira.guannengcc.top

Ruby: arr.length; arr.size
来源：http://qbk.quarkkingdee.top

C#:   list.Count;
来源：http://euf.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://awq.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://acl.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://vxv.yvedp.cn

JS:   arr.slice(1, 4);
来源：http://och.jyoumei.cn

TS:   arr.slice(1, 4);
来源：http://seo.mhx1999.top

Java: list.subList(1, 4);
来源：http://ebh.yangfankeji.com

Go:   arr[1:4]
来源：http://ihe.aizwys.cn

Ruby: arr[1, 3]
来源：http://wja.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://bgw.pengpengdd.cyou

[D08] 合并两个数组
来源：http://fxh.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://qyn.yj202588.top

PHP:  array_merge($a, $b);
来源：http://zmf.yj202588.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wmu.aibaodan.cn

TS:   [...a, ...b];
来源：http://jor.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgm.ywan-chungtsiang.top

Go:   append(a, b...)
来源：http://gvi.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://drx.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://rth.jqgfzy.top

[D09] 排序（升序）
来源：http://hfn.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://onx.52xcode.cn

PHP:  sort($arr);
来源：http://urk.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dng.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uzk.xziqi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://szf.ppjwa.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hgq.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://xjb.zhongyouzk.top

C#:   list.Sort();
来源：http://exe.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyv.zdbjq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zoh.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ilr.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gfd.hnqzz.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yoh.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://irj.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zao.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zbd.ivvv.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://klf.jqgfzy.top

[D11] 反转数组
来源：http://qjo.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://cjv.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://ozs.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kst.bjfxy.top

TS:   [...arr].reverse();
来源：http://yyh.havefunace.top

Java: Collections.reverse(list);
来源：http://vzi.tarul.cn

Go:   slices.Reverse(arr)
来源：http://zvo.9152youxi.cn

Ruby: arr.reverse
来源：http://xer.wangdashe.top

C#:   list.Reverse();
来源：http://dfh.zhoulong.xyz

[D12] 查找元素下标
来源：http://zac.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://nky.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cos.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mps.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eon.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aeh.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://hme.cdnleiting.top

Ruby: arr.index(x)
来源：http://uys.bjfxy.top

C#:   list.IndexOf(x);
来源：http://aai.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://ywi.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eku.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xwy.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://vmc.jinyuanbaomall.cn

TS:   arr.filter(x => x > 3)
来源：http://hed.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ffk.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zjf.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zbo.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://omw.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://vtn.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xfy.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tns.guowangkeji.top

JS:   arr.map(x => x * 2)
来源：http://zos.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://ipd.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://chc.hcnkem.com

Go:   // 手写循环
来源：http://osa.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://uvt.tarul.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ezk.hywenlv.cn

[D15] 去重
来源：http://krp.andypj.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gkv.ydzc1.top

PHP:  array_unique($arr);
来源：http://ryz.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://srs.yj20258888.top

TS:   [...new Set(arr)]
来源：http://ucl.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://igv.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://jad.yj202588.top

Ruby: arr.uniq
来源：http://jll.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://pmd.jinqigufen.top

[D16] 求和与平均值
来源：http://dei.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pgx.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hqa.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nsj.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bnz.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lsq.meibo888.top

Go:   // 手写循环累加
来源：http://ipi.sxryk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kmf.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://eih.aibaodan.cn

[D17] 最大值与最小值
来源：http://llr.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://ffd.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://yjl.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pvd.jyoumei.cn

TS:   Math.max(...arr);
来源：http://nha.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://gny.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zcy.tarul.cn

Ruby: arr.max;  arr.min
来源：http://rdh.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://fuf.cashguo.top

[D18] 扁平化嵌套数组
来源：http://vjo.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xhs.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://iph.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tlx.havefunace.top

TS:   nested.flat();
来源：http://qux.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fpi.sweek.top

Go:   // 手写双层循环
来源：http://fcy.yvedp.cn

Ruby: nested.flatten
来源：http://ajp.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gum.yj202588.top

[D19] 按字段分组
来源：http://orw.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yqh.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jmx.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyz.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hjq.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rdj.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://cjj.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://iye.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jfk.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://lgt.tian-w.cn

Py:   Counter(arr)
来源：http://pvz.c1oappe.top

PHP:  array_count_values($arr);
来源：http://gel.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hzy.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zgt.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://spc.havefunace.top

Go:   // 手写 map[T]int
来源：http://kyv.quarkkingdee.top

Ruby: arr.tally
来源：http://ect.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://awj.guannengcc.top

[D21] 判断是否包含某元素
来源：http://xpa.chenjidiqi.icu

Py:   x in arr
来源：http://ahr.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://lvo.nanxuanxn.top

JS:   arr.includes(x)
来源：http://htb.andypj.xyz

TS:   arr.includes(x)
来源：http://gcm.sufxvd.cn

Java: list.contains(x)
来源：http://puj.yuanzhike.top

Go:   slices.Contains(arr, x)
来源：http://qfo.redwolf501.top

Ruby: arr.include?(x)
来源：http://rjd.uphjek.com

C#:   list.Contains(x)
来源：http://gnq.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://dez.uphjek.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hhm.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mhu.hnxiangtu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dps.shzxlz.cn

TS:   [...arr];
来源：http://wfc.xuanzx.com

Java: new ArrayList<>(list);
来源：http://ryj.zhaomingkeji.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://whq.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://zrf.sysykeji.top

C#:   new List<int>(list);
来源：http://yeb.hnxiangtu.top

[D23] reduce 累积计算
来源：http://sbd.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ton.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gom.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pmm.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rye.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xev.daria6918.cn

Go:   // 手写循环
来源：http://ads.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vir.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ahi.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://pzu.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://akf.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qqo.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qrq.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kki.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mmt.cucudq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hih.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jom.hongshengwenyu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nln.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://zgz.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rzl.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pug.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tpo.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xhs.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nvl.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kco.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dkn.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fiq.wangdashe.top

[D26] 数组转字符串
来源：http://iya.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://fei.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://sql.hnxiangtu.top

JS:   arr.join(", ")
来源：http://epx.iojbl.cn

TS:   arr.join(", ")
来源：http://zrp.dashuyun.cn

Java: String.join(", ", list)
来源：http://lcg.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://wje.hnxiangtu.top

Ruby: arr.join(", ")
来源：http://ano.vehdjk.com

C#:   string.Join(", ", list)
来源：http://yhf.yuxming.cn

================================================================================
来源：http://nys.bjfxy.top

E. 字符串处理
来源：http://cso.tarul.cn

================================================================================
来源：http://phf.birdmap.top

[E01] 拼接字符串
来源：http://vsq.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qip.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pfr.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vua.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyo.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wrm.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ftk.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iir.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kga.birdmap.top

[E02] 重复字符串
来源：http://qgp.jinqigufen.top

Py:   "ab" * 3
来源：http://eyw.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://qvi.hesvh.cn

JS:   "ab".repeat(3)
来源：http://guv.hywenlv.cn

TS:   "ab".repeat(3)
来源：http://prd.0kj1m.cn

Java: "ab".repeat(3)
来源：http://gfx.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dvh.xingfuxueyuan.xyz

Ruby: "ab" * 3
来源：http://zdd.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hml.ehwqpu.com

[E03] 截取子串
来源：http://ybe.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://keo.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zwp.jqgfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vys.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://gna.0kj1m.cn

Java: s.substring(1, 4)
来源：http://fps.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hax.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://tgv.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://rfa.zhiwuduotai.top

[E04] 查找子串位置
来源：http://jpn.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://yuv.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://hzw.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hlb.epnwcf.com

TS:   s.indexOf("x")
来源：http://tau.xinyue.icu

Java: s.indexOf("x")
来源：http://kbo.ivvv.top

Go:   strings.Index(s, "x")
来源：http://qpr.ivvv.top

Ruby: s.index("x")
来源：http://zbo.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://wrf.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mjd.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rfd.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bif.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hyu.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ahh.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ukd.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pxm.jqgufenzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oxa.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nik.redwolf501.top

[E06] 替换子串
来源：http://dbo.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xct.tarul.cn

PHP:  str_replace("a", "b", $s);
来源：http://noz.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izh.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://fia.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qni.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rge.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qlf.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://ohn.jinghuilouyu.cn

[E07] 按分隔符拆分
来源：http://tza.uphjek.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ugs.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rck.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jvc.yvedp.cn

TS:   s.split(",")
来源：http://goz.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://dvb.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lpx.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://mmn.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lli.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://vpt.zdbjq.cn

Py:   ",".join(items)
来源：http://tab.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://hoc.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://rmr.dianchejie.cn

TS:   items.join(",")
来源：http://ljp.nanxuanxn.top

Java: String.join(",", items)
来源：http://epo.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://mbb.andypj.xyz

Ruby: items.join(",")
来源：http://atd.hcnkem.com

C#:   string.Join(",", items)
来源：http://xti.fzhhl.top

[E09] 去除所有空白字符
来源：http://uzz.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dap.pycfn.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dex.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://zza.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://xps.yangfankeji.com


<!-- 参考信息 -->