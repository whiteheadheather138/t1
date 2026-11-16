代发 wailian999

C#:   list.Insert(0, 0);
来源：http://udk.gaohongyu789.top

[D04] 删除元素
来源：http://org.yueranfly.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://joz.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oda.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://onn.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://cbb.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://thx.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kal.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jqm.redwolf501.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wma.cucudq.cn

[D05] 访问与修改元素
来源：http://kmm.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eii.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ysm.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zft.xinyue.icu

TS:   arr[0]; arr.at(-1);
来源：http://iyt.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://gea.fehbvm.com

Go:   arr[0]; arr[0] = 9
来源：http://rtq.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vxr.zycfv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ffm.chenzaomai.com

[D06] 数组长度
来源：http://frd.fehbvm.com

Py:   len(arr)
来源：http://hxj.daria6918.cn

PHP:  count($arr);
来源：http://uhy.yuxming.cn

JS:   arr.length
来源：http://kxo.fengsongda.top

TS:   arr.length
来源：http://hks.aibaodan.cn

Java: list.size();
来源：http://pte.xinyue.icu

Go:   len(arr)
来源：http://qll.feifeiyinyue.top

Ruby: arr.length; arr.size
来源：http://eim.chenzaomai.com

C#:   list.Count;
来源：http://jgq.ctjpmb.com

[D07] 切片 / 取子数组
来源：http://dsm.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nds.jlsjyb.cn

PHP:  array_slice($arr, 1, 3);
来源：http://oez.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://kgg.xziqi.cn

TS:   arr.slice(1, 4);
来源：http://cfs.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://ydy.svipenyu.cn

Go:   arr[1:4]
来源：http://gmw.ehwqpu.com

Ruby: arr[1, 3]
来源：http://wpx.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://dqf.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://iud.jianghu66.top

Py:   a + b;  a.extend(b)
来源：http://fqc.birdmap.top

PHP:  array_merge($a, $b);
来源：http://ooy.fehbvm.com

JS:   [...a, ...b];  a.concat(b);
来源：http://uxo.0kj1m.cn

TS:   [...a, ...b];
来源：http://jdm.sxryk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lor.zdbjq.cn

Go:   append(a, b...)
来源：http://mbc.nanxinkj.top

Ruby: a + b;  a.concat(b)
来源：http://cjs.gogol.net.cn

C#:   a.Concat(b).ToList()
来源：http://jai.xylfe.cn

[D09] 排序（升序）
来源：http://wml.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://jyr.zhengqikj.top

PHP:  sort($arr);
来源：http://gfc.hfpthk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ojl.yongpay.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://trd.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tmz.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ysm.smart0.xyz

Ruby: arr.sort
来源：http://uqf.nanxuanxn.top

C#:   list.Sort();
来源：http://tnn.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://gro.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ljn.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pzj.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgn.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gbt.hfpthk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zsh.andypj.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uky.zhongyouzk.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vbj.sysykeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ois.yangfankeji.com

[D11] 反转数组
来源：http://acn.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://dmi.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://pob.shanyushiyangtech.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mkf.tianlin.xyz

TS:   [...arr].reverse();
来源：http://nnt.bjfxy.top

Java: Collections.reverse(list);
来源：http://ldw.ywan-chungtsiang.top

Go:   slices.Reverse(arr)
来源：http://lmh.jqgfzy.top

Ruby: arr.reverse
来源：http://ehx.ppjwa.cn

C#:   list.Reverse();
来源：http://uqs.smart0.xyz

[D12] 查找元素下标
来源：http://udr.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://lwd.daxiang520.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jhg.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kkn.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kjm.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ike.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://vto.zhengqikj.top

Ruby: arr.index(x)
来源：http://wti.shuidangran.top

C#:   list.IndexOf(x);
来源：http://aop.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://apo.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yhd.52xcode.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rcu.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://dmg.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://fkw.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ysj.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uvq.cdnleiting.top

Ruby: arr.select { |x| x > 3 }
来源：http://qwl.pengpengdd.cyou

C#:   list.Where(x => x > 3).ToList()
来源：http://rix.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://ohy.jqgfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ach.jqgufenzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rcr.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://gzy.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://apx.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://prf.nanxinkj.top

Go:   // 手写循环
来源：http://wah.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ieu.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xix.xylfe.cn

[D15] 去重
来源：http://ste.bjfxy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vlj.aizwys.cn

PHP:  array_unique($arr);
来源：http://plo.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://bnd.nwbrower.top

TS:   [...new Set(arr)]
来源：http://tac.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xnw.vqdsnc.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xnk.feifeiyinyue.top

Ruby: arr.uniq
来源：http://erv.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://azx.zhoulong.xyz

[D16] 求和与平均值
来源：http://vxa.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://emx.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rpb.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kcf.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgc.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://spu.yonumen.top

Go:   // 手写循环累加
来源：http://xnn.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dgl.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://tpz.jqgfzy.top

[D17] 最大值与最小值
来源：http://uvr.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://juu.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://gyo.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mod.dianchejie.cn

TS:   Math.max(...arr);
来源：http://vnk.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://abk.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qyp.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://awy.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://hct.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://ncu.yongpay.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zpu.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://eqw.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vhh.hongshengwenyu.top

TS:   nested.flat();
来源：http://oec.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dwt.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://tib.yanxiufei.cn

Ruby: nested.flatten
来源：http://zpi.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xan.tianlin.xyz

[D19] 按字段分组
来源：http://wuz.chenjidiqi.icu

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://emn.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gtq.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mju.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvy.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bno.yj202588.top

Go:   // 手写 map[string][]T
来源：http://mts.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nhg.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bkj.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://ysi.sxryk.cn

Py:   Counter(arr)
来源：http://hin.yfazqb.com

PHP:  array_count_values($arr);
来源：http://lhs.bbcook.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://msd.guannengcc.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fzw.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ktx.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://ctw.hammf.cn

Ruby: arr.tally
来源：http://vpc.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zez.yuxming.cn

[D21] 判断是否包含某元素
来源：http://fwd.dianchejie.cn

Py:   x in arr
来源：http://ibu.fehbvm.com

PHP:  in_array($x, $arr, true);
来源：http://xiw.chenlongwang.top

JS:   arr.includes(x)
来源：http://gjk.havefunace.top

TS:   arr.includes(x)
来源：http://gih.hnxiangtu.top

Java: list.contains(x)
来源：http://ujv.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://gan.52xcode.cn

Ruby: arr.include?(x)
来源：http://jda.meibo888.top

C#:   list.Contains(x)
来源：http://vjk.quarkkingdee.top

[D22] 复制数组（避免共享引用）
来源：http://pst.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://abc.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://faj.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wgh.pengpengdd.cyou

TS:   [...arr];
来源：http://tjp.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://ssr.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://phr.ydzc1.top

Ruby: arr.dup;  arr.clone
来源：http://wtu.gotoacloud.top

C#:   new List<int>(list);
来源：http://lit.hnqzz.top

[D23] reduce 累积计算
来源：http://hln.yuanzhike.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pdr.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rlx.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iat.c1oappe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tdn.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://jab.cucudq.cn

Go:   // 手写循环
来源：http://wut.ehwqpu.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://myo.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://miy.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://lnp.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://due.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ygj.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jcb.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://glp.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jrx.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kjw.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xme.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xtd.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://vxo.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://usd.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qud.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xjm.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iqf.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://asj.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bvn.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uca.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vtp.redwolf501.top

[D26] 数组转字符串
来源：http://gxy.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://mxq.hammf.cn

PHP:  implode(", ", $arr);
来源：http://btj.guannengcc.top

JS:   arr.join(", ")
来源：http://vye.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://gff.yj202588.top

Java: String.join(", ", list)
来源：http://zjz.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://jbz.jqgfzy.top

Ruby: arr.join(", ")
来源：http://cgp.gogol.net.cn

C#:   string.Join(", ", list)
来源：http://gna.xziqi.cn

================================================================================
来源：http://kkm.hongshengwenyu.top

E. 字符串处理
来源：http://qyi.jinqigfzy.top

================================================================================
来源：http://euh.jyoumei.cn

[E01] 拼接字符串
来源：http://whb.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fdr.c1oappe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://omh.jianghu66.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://und.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ebn.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vjb.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uag.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gjp.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vpc.jqgfzy.top

[E02] 重复字符串
来源：http://mtp.kuanghao11.cn

Py:   "ab" * 3
来源：http://prx.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://nge.yj202588.top

JS:   "ab".repeat(3)
来源：http://rzv.cheryme.top

TS:   "ab".repeat(3)
来源：http://rld.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://nsj.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://shf.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://qwt.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nig.xylfe.cn

[E03] 截取子串
来源：http://hcm.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tbr.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ipj.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvg.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://acs.epnwcf.com

Java: s.substring(1, 4)
来源：http://tlk.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ccz.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://ndz.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://xub.yonumen.top

[E04] 查找子串位置
来源：http://pjh.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://ubn.316326.xyz

PHP:  strpos($s, "x");
来源：http://kbg.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jfr.0kj1m.cn

TS:   s.indexOf("x")
来源：http://bzr.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://frz.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://cpm.cdnleiting.top

Ruby: s.index("x")
来源：http://ftz.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://zqm.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://moq.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tfg.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hwr.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://egn.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pzm.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wts.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fwo.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mpv.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aud.cucudq.cn

[E06] 替换子串
来源：http://xvj.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ojz.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://rqy.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nfh.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://pit.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yes.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fti.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ajk.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://wmd.jinqigufen.top

[E07] 按分隔符拆分
来源：http://xzc.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qlb.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rqp.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hze.jqgfzy.top

TS:   s.split(",")
来源：http://utb.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://nkr.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fme.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://rod.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rlq.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://pqr.guannengcc.top

Py:   ",".join(items)
来源：http://mvc.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://ucb.birdmap.top

JS:   items.join(",")
来源：http://tnc.yuxming.cn

TS:   items.join(",")
来源：http://cne.jlsjyb.cn

Java: String.join(",", items)
来源：http://fio.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://det.jinqigfzy.top

Ruby: items.join(",")
来源：http://izj.fzhhl.top

C#:   string.Join(",", items)
来源：http://fic.shuidangran.top

[E09] 去除所有空白字符
来源：http://pkl.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yey.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://awb.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://lxq.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://diq.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://opp.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://vig.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ylv.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://lej.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://non.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xiz.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://jea.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://plg.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://aiz.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://urz.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ivb.xingfuxueyuan.xyz


<!-- 参考信息 -->