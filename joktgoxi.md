代发 wailian999

Java: list.add(4);
来源：http://yos.gogol.net.cn

Go:   arr = append(arr, 4)
来源：http://iqc.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://wxf.sxryk.cn

C#:   list.Add(4);
来源：http://mab.epnwcf.com

[D03] 在指定位置插入元素
来源：http://wqs.yj20258888.top

Py:   arr.insert(0, 0)
来源：http://ckw.sysykeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sjy.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rfe.zhoulong.xyz

TS:   arr.splice(0, 0, 0);
来源：http://hic.zycfv.cn

Java: list.add(0, 0);
来源：http://ber.hongshengwenyu.top

Go:   arr = append([]int{0}, arr...)
来源：http://eka.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hiw.cqqwz.cn

C#:   list.Insert(0, 0);
来源：http://txl.sjlbkw.cn

[D04] 删除元素
来源：http://uul.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lpr.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jkp.quarkkingdee.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cad.ivvv.top

TS:   arr.splice(0, 1);
来源：http://olw.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hwa.ybcxt.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ffa.bjfxy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mza.bbcook.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lan.daria6918.cn

[D05] 访问与修改元素
来源：http://duh.jinqigfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ygb.birdmap.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hyc.zycfv.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ooh.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://jrk.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://vqx.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://dmt.hysaishi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gna.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bly.yfazqb.com

[D06] 数组长度
来源：http://gzk.cashguo.top

Py:   len(arr)
来源：http://fdc.sjlbkw.cn

PHP:  count($arr);
来源：http://zsy.redwolf501.top

JS:   arr.length
来源：http://zvb.shangyingyoupin.top

TS:   arr.length
来源：http://kpz.dashuyun.cn

Java: list.size();
来源：http://rvx.sweek.top

Go:   len(arr)
来源：http://rda.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://weo.nanxuanxn.top

C#:   list.Count;
来源：http://lzl.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://tav.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://atl.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://lcl.jyoumei.cn

JS:   arr.slice(1, 4);
来源：http://clw.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://ool.chenzaomai.com

Java: list.subList(1, 4);
来源：http://rwy.jyoumei.cn

Go:   arr[1:4]
来源：http://zbr.fengsongda.top

Ruby: arr[1, 3]
来源：http://ltu.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://zoz.ybcxt.top

[D08] 合并两个数组
来源：http://ptx.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://btl.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://zns.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://elr.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://qmm.bbcook.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nlf.andypj.xyz

Go:   append(a, b...)
来源：http://kcq.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://kqx.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://bjg.xuetiantiany.cn

[D09] 排序（升序）
来源：http://uaf.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ypy.hammf.cn

PHP:  sort($arr);
来源：http://bfn.dashuyun.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dtz.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aee.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gsm.cucudq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ztk.svipenyu.cn

Ruby: arr.sort
来源：http://wkh.tian-w.cn

C#:   list.Sort();
来源：http://iwq.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pfq.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://anf.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mqx.ydzc1.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xkr.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xdg.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cij.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://inn.jinqigfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kuv.xuetiantiany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ivm.52xcode.cn

[D11] 反转数组
来源：http://phu.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://cwc.hcnkem.com

PHP:  array_reverse($arr);
来源：http://kye.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hgm.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://wxd.xziqi.cn

Java: Collections.reverse(list);
来源：http://fce.yongpay.top

Go:   slices.Reverse(arr)
来源：http://gqr.jinqigufen.top

Ruby: arr.reverse
来源：http://coi.jlsjyb.cn

C#:   list.Reverse();
来源：http://czr.ivvv.top

[D12] 查找元素下标
来源：http://bix.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://vej.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jom.nanxuanxn.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vxu.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hom.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://juh.sweek.top

Go:   slices.Index(arr, x)
来源：http://tgz.nwbrower.top

Ruby: arr.index(x)
来源：http://foe.cucudq.cn

C#:   list.IndexOf(x);
来源：http://tdk.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://ffq.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cuz.ywan-chungtsiang.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://atx.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://dfw.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://stf.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nnm.fktsv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dpi.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://zdp.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://vem.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://jzb.ctjpmb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dzz.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ukx.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://gsf.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://swb.xylfe.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qbj.wangdashe.top

Go:   // 手写循环
来源：http://nqo.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://acv.hnxiangtu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wtw.0kj1m.cn

[D15] 去重
来源：http://wrd.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xer.yj20258888.top

PHP:  array_unique($arr);
来源：http://gbi.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://cwg.yj20258.top

TS:   [...new Set(arr)]
来源：http://lyo.ydjk.org.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://itj.birdmap.top

Go:   // 用 map[T]struct{} 手写
来源：http://jdg.hammf.cn

Ruby: arr.uniq
来源：http://yeu.yj20258888.top

C#:   list.Distinct().ToList()
来源：http://tlb.yueranfly.top

[D16] 求和与平均值
来源：http://bed.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ylk.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bhx.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yst.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://djf.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://isq.yvedp.cn

Go:   // 手写循环累加
来源：http://pjj.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ede.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://bjc.jinqigufen.top

[D17] 最大值与最小值
来源：http://uqx.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://rsc.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://fzq.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xbj.dianchejie.cn

TS:   Math.max(...arr);
来源：http://lhw.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://aou.andypj.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gew.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://zio.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://mjl.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://tsk.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mnn.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://itf.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tjf.fehbvm.com

TS:   nested.flat();
来源：http://ewu.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dan.yj202588.top

Go:   // 手写双层循环
来源：http://occ.hammf.cn

Ruby: nested.flatten
来源：http://ycr.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xlm.c1oappe.top

[D19] 按字段分组
来源：http://irz.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vef.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mky.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kjp.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://obu.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uzx.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://dig.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nwy.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://crs.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://yrh.ppjwa.cn

Py:   Counter(arr)
来源：http://iiw.hfpthk.cn

PHP:  array_count_values($arr);
来源：http://hsm.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rpp.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cdr.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ual.daria6918.cn

Go:   // 手写 map[T]int
来源：http://itp.sysykeji.top

Ruby: arr.tally
来源：http://fzq.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jpx.xylfe.cn

[D21] 判断是否包含某元素
来源：http://mdr.quarkkingdee.top

Py:   x in arr
来源：http://hhs.yj20258888.top

PHP:  in_array($x, $arr, true);
来源：http://czg.ydjk.org.cn

JS:   arr.includes(x)
来源：http://kcq.havefunace.top

TS:   arr.includes(x)
来源：http://vab.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://sgk.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://hgj.hysaishi.cn

Ruby: arr.include?(x)
来源：http://hyq.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://ags.gaohongyu789.top

[D22] 复制数组（避免共享引用）
来源：http://yyk.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://but.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wkz.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jvt.bbcook.cn

TS:   [...arr];
来源：http://adf.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://jlw.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://tol.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://fqm.sweek.top

C#:   new List<int>(list);
来源：http://ify.uphjek.com

[D23] reduce 累积计算
来源：http://jsy.yanxiufei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qcd.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fpe.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qri.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://apn.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fzx.kuanghao11.cn

Go:   // 手写循环
来源：http://njx.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://niy.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kcr.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://sfn.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rtj.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lhu.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hmx.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oni.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://riy.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qcx.nwbrower.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://atu.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://opi.hcnkem.com

[D25] Set 集合去重与交并差
来源：http://gle.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wki.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://doi.guannengcc.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://omp.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kfr.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dkx.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tvv.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fiy.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yyq.wangshuangyany.cn

[D26] 数组转字符串
来源：http://csb.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://tyn.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://gtk.ydzc1.top

JS:   arr.join(", ")
来源：http://qsp.vehdjk.com

TS:   arr.join(", ")
来源：http://fbq.sxryk.cn

Java: String.join(", ", list)
来源：http://pdu.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://zlz.shzxlz.cn

Ruby: arr.join(", ")
来源：http://iok.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://qxs.yonumen.top

================================================================================
来源：http://mwm.redwolf501.top

E. 字符串处理
来源：http://dvl.wangshuangyany.cn

================================================================================
来源：http://oil.nwbrower.top

[E01] 拼接字符串
来源：http://huq.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zhp.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zwx.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kcv.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ufg.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dfa.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rwt.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tdr.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://grt.sysykeji.top

[E02] 重复字符串
来源：http://ltq.zhiwuduotai.top

Py:   "ab" * 3
来源：http://xmx.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://pbv.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://trs.epnwcf.com

TS:   "ab".repeat(3)
来源：http://ago.sufxvd.cn

Java: "ab".repeat(3)
来源：http://aei.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://gec.cucudq.cn

Ruby: "ab" * 3
来源：http://cxl.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mij.hesvh.cn

[E03] 截取子串
来源：http://two.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oot.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iqf.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zku.yonumen.top

TS:   s.slice(1, 4)
来源：http://vct.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://zdy.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oea.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://uyi.zhaomingkeji.xyz

C#:   s.Substring(1, 3)
来源：http://cyv.316326.xyz

[E04] 查找子串位置
来源：http://xne.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://cdu.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://nql.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ggu.cashguo.top

TS:   s.indexOf("x")
来源：http://yof.daxiang520.top

Java: s.indexOf("x")
来源：http://qkp.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://typ.cashguo.top

Ruby: s.index("x")
来源：http://jnb.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://sco.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vwn.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zws.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qkh.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppd.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zqj.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dvi.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zpd.c1oappe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://coc.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ads.hfpthk.cn

[E06] 替换子串
来源：http://szw.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zge.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://vzd.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lpw.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://lei.pengpengdd.cyou

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ajc.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wii.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nmz.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://ort.nwbrower.top

[E07] 按分隔符拆分
来源：http://wcp.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wgh.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://euu.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ngs.fanxiaobao.xyz

TS:   s.split(",")
来源：http://tlo.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://xrv.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rvb.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://adx.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dtm.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://ucq.yangfankeji.com

Py:   ",".join(items)
来源：http://ncv.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://qqz.ybcxt.top

JS:   items.join(",")
来源：http://jed.nanxuanxn.top

TS:   items.join(",")
来源：http://yge.ybcxt.top

Java: String.join(",", items)
来源：http://fho.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://wyv.52xcode.cn

Ruby: items.join(",")
来源：http://qbs.zhengqikj.top

C#:   string.Join(",", items)
来源：http://lry.xylfe.cn

[E09] 去除所有空白字符
来源：http://rcf.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sgd.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ndy.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://xkf.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://xbq.vehdjk.com


<!-- 参考信息 -->