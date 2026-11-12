代发 wailian999

Java: list.add(4);
来源：http://sxb.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://jsh.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://oyq.feifeiyinyue.top

C#:   list.Add(4);
来源：http://gvb.xuanzx.com

[D03] 在指定位置插入元素
来源：http://tns.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://clk.tianlin.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yci.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xud.smart0.xyz

TS:   arr.splice(0, 0, 0);
来源：http://pun.jqgufenzy.top

Java: list.add(0, 0);
来源：http://xmc.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fuw.ywan-chungtsiang.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fjh.bjfxy.top

C#:   list.Insert(0, 0);
来源：http://qav.mhx1999.top

[D04] 删除元素
来源：http://raa.nanxuanxn.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ekh.havefunace.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jsh.uphjek.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xen.fktsv.cn

TS:   arr.splice(0, 1);
来源：http://zpv.zycfv.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://axs.nanxinkj.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zqq.hcnkem.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nbl.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vrp.nwbrower.top

[D05] 访问与修改元素
来源：http://gyu.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yii.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ikc.ctjpmb.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rid.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://qwr.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://iml.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://eqw.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mke.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://taz.hfpthk.cn

[D06] 数组长度
来源：http://mfn.nwbrower.top

Py:   len(arr)
来源：http://nig.hfpthk.cn

PHP:  count($arr);
来源：http://nlc.chenjidiqi.icu

JS:   arr.length
来源：http://lud.chenjidiqi.icu

TS:   arr.length
来源：http://lzm.feifeiyinyue.top

Java: list.size();
来源：http://ztx.jinghuilouyu.cn

Go:   len(arr)
来源：http://tci.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://nnn.fengsongda.top

C#:   list.Count;
来源：http://rvs.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://nic.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rmu.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://usr.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://rdc.pycfn.com

TS:   arr.slice(1, 4);
来源：http://ajq.shuidangran.top

Java: list.subList(1, 4);
来源：http://utr.nwbrower.top

Go:   arr[1:4]
来源：http://ofi.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://kmn.yvedp.cn

C#:   list.GetRange(1, 3);
来源：http://cov.c1oappe.top

[D08] 合并两个数组
来源：http://zwe.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://loi.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://cpb.jyoumei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fqr.sxryk.cn

TS:   [...a, ...b];
来源：http://gxt.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cev.tanke756.top

Go:   append(a, b...)
来源：http://okm.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://stu.jinyuanbaomall.cn

C#:   a.Concat(b).ToList()
来源：http://izx.tian-w.cn

[D09] 排序（升序）
来源：http://xml.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://aiy.birdmap.top

PHP:  sort($arr);
来源：http://ruz.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nnt.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://uye.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jpc.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bxd.havefunace.top

Ruby: arr.sort
来源：http://lsa.aibaodan.cn

C#:   list.Sort();
来源：http://ssp.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kry.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jkv.shzxlz.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uls.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ddc.fehbvm.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://icp.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ras.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fvx.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iir.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rtf.shangyingyoupin.top

[D11] 反转数组
来源：http://mhd.zdqjudy.top

Py:   arr[::-1];  arr.reverse()
来源：http://paq.daxiang520.top

PHP:  array_reverse($arr);
来源：http://duh.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ulo.bbcook.cn

TS:   [...arr].reverse();
来源：http://rvg.yuxming.cn

Java: Collections.reverse(list);
来源：http://vqh.xingfuxueyuan.xyz

Go:   slices.Reverse(arr)
来源：http://zfq.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://swm.ydzc1.top

C#:   list.Reverse();
来源：http://ibt.fehbvm.com

[D12] 查找元素下标
来源：http://pqh.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://rpk.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jlu.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yom.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dom.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kvq.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://fdl.yfazqb.com

Ruby: arr.index(x)
来源：http://fyu.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://hir.mhx1999.top

[D13] 过滤（保留满足条件的）
来源：http://ili.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qol.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ags.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://gpv.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://emh.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxl.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xka.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://sfz.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qbp.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://edg.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mnt.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fjm.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://oei.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://yzn.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jzl.kuanghao11.cn

Go:   // 手写循环
来源：http://jld.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://yfb.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://yqx.fehbvm.com

[D15] 去重
来源：http://fio.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ebv.ivvv.top

PHP:  array_unique($arr);
来源：http://xso.fzhhl.top

JS:   [...new Set(arr)]
来源：http://vxy.pycfn.com

TS:   [...new Set(arr)]
来源：http://wqu.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yng.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://enj.sysykeji.top

Ruby: arr.uniq
来源：http://atg.cashguo.top

C#:   list.Distinct().ToList()
来源：http://rza.tianlin.xyz

[D16] 求和与平均值
来源：http://hrp.zhoulong.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ulf.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sqa.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://frp.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://liz.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogk.mhx1999.top

Go:   // 手写循环累加
来源：http://gix.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xdt.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://ihr.cqqwz.cn

[D17] 最大值与最小值
来源：http://tow.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://vpv.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://snf.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kdm.aibaodan.cn

TS:   Math.max(...arr);
来源：http://yqo.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tmi.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jxz.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://fpc.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://akt.uphjek.com

[D18] 扁平化嵌套数组
来源：http://wpx.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vxg.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://gly.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jve.fehbvm.com

TS:   nested.flat();
来源：http://dcx.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ddv.zhoulong.xyz

Go:   // 手写双层循环
来源：http://jtm.shanyushiyangkeji.top

Ruby: nested.flatten
来源：http://pso.hfpthk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ssu.wangdashe.top

[D19] 按字段分组
来源：http://ifk.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pod.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ucl.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iim.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://avw.fengsongda.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hrp.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://mbw.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lvf.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bzx.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://bas.gaohongyu789.top

Py:   Counter(arr)
来源：http://lnr.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://txw.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kqo.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awv.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://doh.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://blx.meibo888.top

Ruby: arr.tally
来源：http://kgb.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufp.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://sfx.zdbjq.cn

Py:   x in arr
来源：http://jkn.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://ump.0kj1m.cn

JS:   arr.includes(x)
来源：http://bga.wangdashe.top

TS:   arr.includes(x)
来源：http://zyy.xuetiantiany.cn

Java: list.contains(x)
来源：http://lrc.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://qtd.sxryk.cn

Ruby: arr.include?(x)
来源：http://ujd.hysaishi.cn

C#:   list.Contains(x)
来源：http://gfo.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://niu.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uzd.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://njn.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yaw.hysaishi.cn

TS:   [...arr];
来源：http://wtx.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://mka.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://mqm.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://ejb.fengsongda.top

C#:   new List<int>(list);
来源：http://ckn.jlsjyb.cn

[D23] reduce 累积计算
来源：http://qhk.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lnd.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vkh.hammf.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xzo.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zjg.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fbo.haohaochexian.top

Go:   // 手写循环
来源：http://ddm.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wej.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cti.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://miz.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hit.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ypp.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pzn.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nku.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fts.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zou.hnqzz.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hyb.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://paf.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://dsd.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kwd.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qpp.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zzz.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rii.guowangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lpa.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://irg.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://acn.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gka.havefunace.top

[D26] 数组转字符串
来源：http://prw.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://lde.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://uft.c1oappe.top

JS:   arr.join(", ")
来源：http://omq.zdqjudy.top

TS:   arr.join(", ")
来源：http://erb.nwbrower.top

Java: String.join(", ", list)
来源：http://yxh.hywenlv.cn

Go:   strings.Join(strs, ", ")
来源：http://ihc.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://ave.hammf.cn

C#:   string.Join(", ", list)
来源：http://uwb.yueranfly.top

================================================================================
来源：http://aon.pycfn.com

E. 字符串处理
来源：http://ekt.fengsongda.top

================================================================================
来源：http://ftl.hammf.cn

[E01] 拼接字符串
来源：http://dfi.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://guf.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wej.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://imj.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rio.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sbv.zhengqikj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vkq.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qwy.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://urm.ctjpmb.com

[E02] 重复字符串
来源：http://drp.zycfv.cn

Py:   "ab" * 3
来源：http://kls.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://udl.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://acu.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://ebi.andypj.xyz

Java: "ab".repeat(3)
来源：http://wke.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://ozv.cheryme.top

Ruby: "ab" * 3
来源：http://ato.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://grb.nanxuanxn.top

[E03] 截取子串
来源：http://upx.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wye.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://imx.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ozn.ybcxt.top

TS:   s.slice(1, 4)
来源：http://wqd.tarul.cn

Java: s.substring(1, 4)
来源：http://szm.gaohongyu789.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aai.zdbjq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qia.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://vfr.zhaomingkeji.xyz

[E04] 查找子串位置
来源：http://doi.zhaomingkeji.xyz

Py:   s.find("x");  s.index("x")
来源：http://ktv.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://jqn.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://exk.jinqigufen.top

TS:   s.indexOf("x")
来源：http://wjd.hysaishi.cn

Java: s.indexOf("x")
来源：http://ziv.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://fbe.ydzc1.top

Ruby: s.index("x")
来源：http://qfj.gzhubu.top

C#:   s.IndexOf("x")
来源：http://fxr.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sus.ywan-chungtsiang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cws.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fge.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eue.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tea.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bew.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://czk.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yxe.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uho.wangdashe.top

[E06] 替换子串
来源：http://llo.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qua.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://mgn.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qkf.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://kge.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zqs.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tll.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sjv.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://mpb.gzhubu.top

[E07] 按分隔符拆分
来源：http://vtz.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yhh.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yxa.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rio.jqgfzy.top

TS:   s.split(",")
来源：http://yhh.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ive.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://paf.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://sqi.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tdh.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://zan.9152youxi.cn

Py:   ",".join(items)
来源：http://isp.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://goz.jlsjyb.cn

JS:   items.join(",")
来源：http://eeg.shanyushiyangtech.top

TS:   items.join(",")
来源：http://spb.jqgfzy.top

Java: String.join(",", items)
来源：http://hhc.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://teg.jqgfzy.top

Ruby: items.join(",")
来源：http://ryc.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://sfk.uphjek.com

[E09] 去除所有空白字符
来源：http://oge.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ozu.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kzi.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://uny.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://cnp.ybcxt.top


<!-- 参考信息 -->