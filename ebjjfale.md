代发 wailian999

[D03] 在指定位置插入元素
来源：http://srf.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://cbs.chenzaomai.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nmu.sjlbkw.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rpo.cucudq.cn

TS:   arr.splice(0, 0, 0);
来源：http://gck.yj20258888.top

Java: list.add(0, 0);
来源：http://jqy.epnwcf.com

Go:   arr = append([]int{0}, arr...)
来源：http://fwb.quarkkingdee.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://spo.aibaodan.cn

C#:   list.Insert(0, 0);
来源：http://gtj.kuanghao11.cn

[D04] 删除元素
来源：http://juh.havefunace.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mnz.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gln.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wnx.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://cqk.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xtb.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uwu.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vpo.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://puc.gogol.net.cn

[D05] 访问与修改元素
来源：http://ueo.gaohongyu789.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ixn.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qdg.hywenlv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xaz.yongpay.top

TS:   arr[0]; arr.at(-1);
来源：http://byv.daxiang520.top

Java: list.get(0); list.set(0, 9);
来源：http://alm.yuanzhike.top

Go:   arr[0]; arr[0] = 9
来源：http://tik.dashuyun.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pel.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hwx.sjlbkw.cn

[D06] 数组长度
来源：http://shh.uphjek.com

Py:   len(arr)
来源：http://iep.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://zcy.feifeiyinyue.top

JS:   arr.length
来源：http://olp.wangshuangyany.cn

TS:   arr.length
来源：http://ipk.redwolf501.top

Java: list.size();
来源：http://quf.vehdjk.com

Go:   len(arr)
来源：http://gif.birdmap.top

Ruby: arr.length; arr.size
来源：http://dyo.jlsjyb.cn

C#:   list.Count;
来源：http://zef.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://uwh.zhongyouzk.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zgq.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fkp.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://zfm.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://bjf.andypj.xyz

Java: list.subList(1, 4);
来源：http://ocx.sufxvd.cn

Go:   arr[1:4]
来源：http://zmk.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://bdp.hfpthk.cn

C#:   list.GetRange(1, 3);
来源：http://wkl.cheryme.top

[D08] 合并两个数组
来源：http://qnj.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://fnn.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://amx.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xpk.redwolf501.top

TS:   [...a, ...b];
来源：http://wem.fktsv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iie.svipenyu.cn

Go:   append(a, b...)
来源：http://xkf.gzhubu.top

Ruby: a + b;  a.concat(b)
来源：http://nab.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://rpc.ivvv.top

[D09] 排序（升序）
来源：http://pwi.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lvb.gaohongyu789.top

PHP:  sort($arr);
来源：http://obx.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jmq.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hjs.tian-w.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qxb.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nxk.yongpay.top

Ruby: arr.sort
来源：http://auh.fehbvm.com

C#:   list.Sort();
来源：http://ekv.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eeo.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wnt.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gbg.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://etm.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xyd.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jwk.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pes.hongshengwenyu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mdu.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jun.jinyuanbaomall.cn

[D11] 反转数组
来源：http://eej.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://vgl.yuxming.cn

PHP:  array_reverse($arr);
来源：http://pix.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://prw.cdnleiting.top

TS:   [...arr].reverse();
来源：http://wwo.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://xjx.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://odu.feifeiyinyue.top

Ruby: arr.reverse
来源：http://jtl.cdnleiting.top

C#:   list.Reverse();
来源：http://rkc.zhengqikj.top

[D12] 查找元素下标
来源：http://ivv.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://oab.ydjk.org.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pru.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkz.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgj.pycfn.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wfb.hammf.cn

Go:   slices.Index(arr, x)
来源：http://mnm.zhoulong.xyz

Ruby: arr.index(x)
来源：http://ggy.jianghu66.top

C#:   list.IndexOf(x);
来源：http://vso.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://moi.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qrq.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ukz.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://jcp.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://buy.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tzf.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://row.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://ecb.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nme.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://lkh.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://syz.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lpd.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://jah.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://lqa.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tjb.ivvv.top

Go:   // 手写循环
来源：http://lew.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://qfv.hesvh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vup.dashuyun.cn

[D15] 去重
来源：http://evf.sxryk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eai.ehwqpu.com

PHP:  array_unique($arr);
来源：http://tsq.ivvv.top

JS:   [...new Set(arr)]
来源：http://zva.fengsongda.top

TS:   [...new Set(arr)]
来源：http://skb.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qwq.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://whw.dashuyun.cn

Ruby: arr.uniq
来源：http://dou.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://exw.snrcjt.cn

[D16] 求和与平均值
来源：http://mvi.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xab.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qzn.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bzf.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aje.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nis.nanxuanxn.top

Go:   // 手写循环累加
来源：http://hqo.dashuyun.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eje.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://maw.yueranfly.top

[D17] 最大值与最小值
来源：http://snf.birdmap.top

Py:   max(arr);  min(arr)
来源：http://kyd.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://zyr.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ocp.ppjwa.cn

TS:   Math.max(...arr);
来源：http://nuu.tian-w.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nac.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yjs.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://kgj.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://jjw.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://hur.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vao.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://zil.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nku.cqqwz.cn

TS:   nested.flat();
来源：http://msy.xylfe.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fiq.yvedp.cn

Go:   // 手写双层循环
来源：http://syc.hammf.cn

Ruby: nested.flatten
来源：http://pad.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nyi.shanyushiyangtech.top

[D19] 按字段分组
来源：http://rct.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ilb.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xzu.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ksm.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dlz.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yss.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://xoq.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://wya.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hgf.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://sud.birdmap.top

Py:   Counter(arr)
来源：http://bab.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://vjo.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bhi.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://arr.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zeu.iojbl.cn

Go:   // 手写 map[T]int
来源：http://zym.yueranfly.top

Ruby: arr.tally
来源：http://sja.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lyg.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://cuk.daria6918.cn

Py:   x in arr
来源：http://ded.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://lnf.jinqigufen.top

JS:   arr.includes(x)
来源：http://kjs.zdqjudy.top

TS:   arr.includes(x)
来源：http://wod.hfpthk.cn

Java: list.contains(x)
来源：http://ita.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://lib.tanke756.top

Ruby: arr.include?(x)
来源：http://zcx.shangyingyoupin.top

C#:   list.Contains(x)
来源：http://yll.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://scw.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mrc.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zqd.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://irb.hesvh.cn

TS:   [...arr];
来源：http://oxj.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://gzo.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mwr.xinyue.icu

Ruby: arr.dup;  arr.clone
来源：http://tte.wangdashe.top

C#:   new List<int>(list);
来源：http://pfn.cqqwz.cn

[D23] reduce 累积计算
来源：http://xhh.svipenyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dkl.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tci.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://urz.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gbk.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ejo.gaohongyu789.top

Go:   // 手写循环
来源：http://ucu.bjfxy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://esf.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zqv.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://oot.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aam.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dvi.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zta.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nrs.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zst.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ajg.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fur.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wiq.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://wus.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zbr.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yiu.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uhj.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nig.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oek.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ccq.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://del.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qqi.jqgfzy.top

[D26] 数组转字符串
来源：http://vcl.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://fvv.yfazqb.com

PHP:  implode(", ", $arr);
来源：http://ehu.daria6918.cn

JS:   arr.join(", ")
来源：http://kqc.chenzaomai.com

TS:   arr.join(", ")
来源：http://guf.xuanzx.com

Java: String.join(", ", list)
来源：http://sjn.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://mnj.xylfe.cn

Ruby: arr.join(", ")
来源：http://mpj.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://hrr.sysykeji.top

================================================================================
来源：http://qbx.chenlongwang.top

E. 字符串处理
来源：http://kgi.snrcjt.cn

================================================================================
来源：http://vha.svipenyu.cn

[E01] 拼接字符串
来源：http://wif.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://twk.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fyr.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sck.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ewi.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ctc.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://evd.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://azi.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ypb.chenzaomai.com

[E02] 重复字符串
来源：http://chv.snrcjt.cn

Py:   "ab" * 3
来源：http://mtx.xingfuxueyuan.xyz

PHP:  str_repeat("ab", 3);
来源：http://zjb.ydzc1.top

JS:   "ab".repeat(3)
来源：http://fgd.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://xbb.yj202588.top

Java: "ab".repeat(3)
来源：http://qks.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://ciy.hnqzz.top

Ruby: "ab" * 3
来源：http://jjw.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vxz.xziqi.cn

[E03] 截取子串
来源：http://hjm.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wzp.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vfn.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yrw.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://bgl.hnqzz.top

Java: s.substring(1, 4)
来源：http://tfn.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jkt.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oso.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://hku.yueranfly.top

[E04] 查找子串位置
来源：http://zot.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://kep.bjfxy.top

PHP:  strpos($s, "x");
来源：http://rln.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vxj.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://xfx.birdmap.top

Java: s.indexOf("x")
来源：http://xnk.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://mpk.wangdashe.top

Ruby: s.index("x")
来源：http://pko.yfazqb.com

C#:   s.IndexOf("x")
来源：http://wvd.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qon.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xbv.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nit.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tji.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dqy.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmo.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://izw.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qsi.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ukf.9152youxi.cn

[E06] 替换子串
来源：http://mgj.smart0.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jwu.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://jaa.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrh.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://pyb.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brg.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nnm.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yng.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://yll.daxiang520.top

[E07] 按分隔符拆分
来源：http://dyu.jianghu66.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pyr.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pwq.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ygc.nanxuanxn.top

TS:   s.split(",")
来源：http://idg.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://uan.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hnl.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://gki.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cek.ydzc1.top

[E08] 数组按分隔符合并
来源：http://rkd.zhongyouzk.top

Py:   ",".join(items)
来源：http://ilf.bjfxy.top

PHP:  implode(",", $items);
来源：http://pyi.guowangkeji.top

JS:   items.join(",")
来源：http://dkl.sweek.top

TS:   items.join(",")
来源：http://erz.hnxiangtu.top

Java: String.join(",", items)
来源：http://nqn.tanke756.top

Go:   strings.Join(items, ",")
来源：http://djr.bjfxy.top

Ruby: items.join(",")
来源：http://wpm.gogol.net.cn

C#:   string.Join(",", items)
来源：http://zso.hysaishi.cn

[E09] 去除所有空白字符
来源：http://trp.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dzx.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://shx.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://wdc.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://mwm.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://qsd.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wtk.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://kod.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kol.aibaodan.cn


<!-- 参考信息 -->