代发 wailian999

[D03] 在指定位置插入元素
来源：http://jek.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://dtg.jinqigfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nqx.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wtw.yj20258888.top

TS:   arr.splice(0, 0, 0);
来源：http://jxr.xinyue.icu

Java: list.add(0, 0);
来源：http://ywe.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://dqb.hfpthk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nyy.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://xsz.zdbjq.cn

[D04] 删除元素
来源：http://inn.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jvh.dashuyun.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dfi.gotoacloud.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dph.shuidangran.top

TS:   arr.splice(0, 1);
来源：http://iig.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tmn.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wzn.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qym.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qia.tarul.cn

[D05] 访问与修改元素
来源：http://etn.chenzaomai.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ire.yfazqb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ntu.bbcook.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://siq.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://eod.zdqjudy.top

Java: list.get(0); list.set(0, 9);
来源：http://jfn.ywan-chungtsiang.top

Go:   arr[0]; arr[0] = 9
来源：http://qxc.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pqm.havefunace.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wcm.guowangkeji.top

[D06] 数组长度
来源：http://oic.hfpthk.cn

Py:   len(arr)
来源：http://evb.yj20258.top

PHP:  count($arr);
来源：http://qxh.yuanzhike.top

JS:   arr.length
来源：http://mpz.chenzaomai.com

TS:   arr.length
来源：http://rcm.haohaochexian.top

Java: list.size();
来源：http://paj.vqdsnc.cn

Go:   len(arr)
来源：http://rle.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://uaj.guannengcc.top

C#:   list.Count;
来源：http://ojt.hcnkem.com

[D07] 切片 / 取子数组
来源：http://kdp.yonumen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aas.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wbx.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://dgk.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://cqk.daxiang520.top

Java: list.subList(1, 4);
来源：http://cwz.sysykeji.top

Go:   arr[1:4]
来源：http://uai.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://kfc.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://upe.yj20258888.top

[D08] 合并两个数组
来源：http://mus.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://gae.cashguo.top

PHP:  array_merge($a, $b);
来源：http://gtd.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vkf.wangshuangyany.cn

TS:   [...a, ...b];
来源：http://jqd.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ffq.guannengcc.top

Go:   append(a, b...)
来源：http://qsd.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://dhw.sufxvd.cn

C#:   a.Concat(b).ToList()
来源：http://ogj.zhoulong.xyz

[D09] 排序（升序）
来源：http://bec.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://ktr.ivvv.top

PHP:  sort($arr);
来源：http://dbe.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://taq.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://emz.guowangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eea.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gwl.yvedp.cn

Ruby: arr.sort
来源：http://tdh.yongpay.top

C#:   list.Sort();
来源：http://pgh.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://wqb.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lya.tian-w.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ane.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qvp.cheryme.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vty.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oyg.yongpay.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dhf.sufxvd.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uda.nanxuanxn.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gxa.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://ndu.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://azt.52xcode.cn

PHP:  array_reverse($arr);
来源：http://ujo.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qhr.gaohongyu789.top

TS:   [...arr].reverse();
来源：http://uuo.9152youxi.cn

Java: Collections.reverse(list);
来源：http://itk.xylfe.cn

Go:   slices.Reverse(arr)
来源：http://bwx.vehdjk.com

Ruby: arr.reverse
来源：http://sgw.dashuyun.cn

C#:   list.Reverse();
来源：http://trm.nwbrower.top

[D12] 查找元素下标
来源：http://zkx.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://elx.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hxi.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfa.zhixingplan.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://inc.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hng.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://puj.jyoumei.cn

Ruby: arr.index(x)
来源：http://sui.pycfn.com

C#:   list.IndexOf(x);
来源：http://pns.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://gfr.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fui.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://adr.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://vpf.andypj.xyz

TS:   arr.filter(x => x > 3)
来源：http://moi.zhengqikj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hdq.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xrt.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qho.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bwb.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://lmp.fzhhl.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nir.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sye.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://hyk.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://kia.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://szu.shuidangran.top

Go:   // 手写循环
来源：http://wok.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://njg.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ykz.tianlin.xyz

[D15] 去重
来源：http://cyp.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lae.tianlin.xyz

PHP:  array_unique($arr);
来源：http://hal.cheryme.top

JS:   [...new Set(arr)]
来源：http://lwt.sweek.top

TS:   [...new Set(arr)]
来源：http://ydi.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ryv.zhixingplan.top

Go:   // 用 map[T]struct{} 手写
来源：http://oro.fengsongda.top

Ruby: arr.uniq
来源：http://jna.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://fkx.shuidangran.top

[D16] 求和与平均值
来源：http://qpc.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rsx.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wie.havefunace.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ncy.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dwr.jinghuilouyu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oql.nanxuanxn.top

Go:   // 手写循环累加
来源：http://qvh.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pif.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://aon.sxryk.cn

[D17] 最大值与最小值
来源：http://ryh.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://ipr.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://bjk.xinyue.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wun.fanxiaobao.xyz

TS:   Math.max(...arr);
来源：http://gya.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://btx.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xwe.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://crw.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://gmf.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://zrb.bjfxy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uyv.ppjwa.cn

PHP:  array_merge(...$nested);
来源：http://itk.feifeiyinyue.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uwx.wangdashe.top

TS:   nested.flat();
来源：http://kal.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sqn.nwbrower.top

Go:   // 手写双层循环
来源：http://tvj.daria6918.cn

Ruby: nested.flatten
来源：http://vgs.ydjk.org.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qui.gogol.net.cn

[D19] 按字段分组
来源：http://oro.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yep.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tvt.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dbe.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xax.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ojf.316326.xyz

Go:   // 手写 map[string][]T
来源：http://xlh.vqdsnc.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zca.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xii.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://csq.gotoacloud.top

Py:   Counter(arr)
来源：http://iqj.daxiang520.top

PHP:  array_count_values($arr);
来源：http://tmm.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://okc.hcnkem.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sqp.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mvh.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://ras.xylfe.cn

Ruby: arr.tally
来源：http://zjp.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ojk.meibo888.top

[D21] 判断是否包含某元素
来源：http://qku.ydjk.org.cn

Py:   x in arr
来源：http://kjy.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://wzq.pycfn.com

JS:   arr.includes(x)
来源：http://mbk.tarul.cn

TS:   arr.includes(x)
来源：http://ogn.zhaomingkeji.xyz

Java: list.contains(x)
来源：http://rnf.fanxiaobao.xyz

Go:   slices.Contains(arr, x)
来源：http://fnp.zdbjq.cn

Ruby: arr.include?(x)
来源：http://dpv.chenlongwang.top

C#:   list.Contains(x)
来源：http://ham.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://pdx.cqqwz.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://leb.9152youxi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gsa.0kj1m.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oye.yongpay.top

TS:   [...arr];
来源：http://nwl.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://ojb.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iys.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://ozs.zhixingplan.top

C#:   new List<int>(list);
来源：http://ozk.jyoumei.cn

[D23] reduce 累积计算
来源：http://qrr.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://igg.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rjj.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://npg.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hxd.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rna.yvedp.cn

Go:   // 手写循环
来源：http://cmg.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nkc.wangshuangyany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hnw.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://cfq.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qbl.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gfh.dianchejie.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ebj.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://elu.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pra.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://llh.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ert.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hdc.tarul.cn

[D25] Set 集合去重与交并差
来源：http://iwy.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xnd.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dzb.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uvf.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ysv.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vzv.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yiv.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iys.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lrj.hfpthk.cn

[D26] 数组转字符串
来源：http://qzn.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://hxx.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://nuk.andypj.xyz

JS:   arr.join(", ")
来源：http://kqi.jqgfzy.top

TS:   arr.join(", ")
来源：http://hbw.ivvv.top

Java: String.join(", ", list)
来源：http://qle.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://ivt.tarul.cn

Ruby: arr.join(", ")
来源：http://msv.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://aex.svipenyu.cn

================================================================================
来源：http://klv.ydzc1.top

E. 字符串处理
来源：http://wiy.cdnleiting.top

================================================================================
来源：http://arb.kuanghao11.cn

[E01] 拼接字符串
来源：http://zza.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tun.zhiwuduotai.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tav.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wfa.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yvx.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dnk.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qzm.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eeg.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hmx.jinqigfzy.top

[E02] 重复字符串
来源：http://bhx.redwolf501.top

Py:   "ab" * 3
来源：http://gvw.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://aoc.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://ogc.cucudq.cn

TS:   "ab".repeat(3)
来源：http://lcr.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://qvp.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://iol.chenjidiqi.icu

Ruby: "ab" * 3
来源：http://fxg.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xvq.yj20258.top

[E03] 截取子串
来源：http://lrb.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ylr.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iii.ybcxt.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://muy.c1oappe.top

TS:   s.slice(1, 4)
来源：http://ulg.tianlin.xyz

Java: s.substring(1, 4)
来源：http://jmc.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bcj.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://gua.tanke756.top

C#:   s.Substring(1, 3)
来源：http://rfl.yueranfly.top

[E04] 查找子串位置
来源：http://upv.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://yxd.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://scg.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ayp.cheryme.top

TS:   s.indexOf("x")
来源：http://ngf.yuxming.cn

Java: s.indexOf("x")
来源：http://jkd.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://vju.tarul.cn

Ruby: s.index("x")
来源：http://ggh.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://iki.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qew.hywenlv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dqf.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tfs.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pvp.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://voo.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yit.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cuk.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ppl.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://szr.ydzc1.top

[E06] 替换子串
来源：http://nsw.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://euu.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://ytr.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bet.tianlin.xyz

TS:   s.replaceAll("a", "b")
来源：http://ubo.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wjq.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wsy.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fyn.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://tdu.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://gvf.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://khz.dianchejie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tuw.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://adf.zhoulong.xyz

TS:   s.split(",")
来源：http://qdt.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://cxl.chenjidiqi.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yyf.yj20258.top

Ruby: s.split(",");  s.split
来源：http://tix.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nzq.tian-w.cn

[E08] 数组按分隔符合并
来源：http://jcv.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://jgy.jinqigfzy.top

PHP:  implode(",", $items);
来源：http://dht.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://lrl.aibaodan.cn

TS:   items.join(",")
来源：http://vuh.ctjpmb.com

Java: String.join(",", items)
来源：http://eig.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://swq.yongpay.top

Ruby: items.join(",")
来源：http://ero.zhixingplan.top

C#:   string.Join(",", items)
来源：http://kjb.uphjek.com

[E09] 去除所有空白字符
来源：http://hpp.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ejk.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bga.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://bua.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://mdc.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://nfl.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xpm.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://gxa.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bet.jiagoushi.top


<!-- 参考信息 -->