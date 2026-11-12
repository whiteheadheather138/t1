代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rfg.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://grr.jianghu66.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hyi.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hdn.gogol.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lvb.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zun.epnwcf.com

[D05] 访问与修改元素
来源：http://fgt.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kzz.chenzaomai.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ror.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hmq.gogol.net.cn

TS:   arr[0]; arr.at(-1);
来源：http://nel.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://gxe.jyoumei.cn

Go:   arr[0]; arr[0] = 9
来源：http://clb.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hat.wangshuangyany.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bfj.yj202588.top

[D06] 数组长度
来源：http://srn.meibo888.top

Py:   len(arr)
来源：http://jqn.yongpay.top

PHP:  count($arr);
来源：http://czc.vqdsnc.cn

JS:   arr.length
来源：http://wsd.hysaishi.cn

TS:   arr.length
来源：http://snw.sweek.top

Java: list.size();
来源：http://alk.mhx1999.top

Go:   len(arr)
来源：http://hjx.nwbrower.top

Ruby: arr.length; arr.size
来源：http://frt.jqgfzy.top

C#:   list.Count;
来源：http://max.sweek.top

[D07] 切片 / 取子数组
来源：http://coj.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://clg.cdnleiting.top

PHP:  array_slice($arr, 1, 3);
来源：http://ijh.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://cde.jinyuanbaomall.cn

TS:   arr.slice(1, 4);
来源：http://gng.zdbjq.cn

Java: list.subList(1, 4);
来源：http://wfc.tarul.cn

Go:   arr[1:4]
来源：http://tdq.iojbl.cn

Ruby: arr[1, 3]
来源：http://tuf.nanxuanxn.top

C#:   list.GetRange(1, 3);
来源：http://wyy.hnqzz.top

[D08] 合并两个数组
来源：http://frc.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://qxs.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://gbf.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://sbn.meibo888.top

TS:   [...a, ...b];
来源：http://pre.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xiu.ctjpmb.com

Go:   append(a, b...)
来源：http://mye.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://ynu.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://tzr.ydzc1.top

[D09] 排序（升序）
来源：http://cos.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://caa.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://bhy.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mpb.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://bwp.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rmq.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://grl.svipenyu.cn

Ruby: arr.sort
来源：http://pjc.yj202588.top

C#:   list.Sort();
来源：http://knm.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://khx.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tdl.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xkv.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pce.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uyk.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xpz.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ajj.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lei.jiagoushi.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vhn.yongpay.top

[D11] 反转数组
来源：http://rjm.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nyf.316326.xyz

PHP:  array_reverse($arr);
来源：http://wny.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wqx.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://yoa.fanxiaobao.xyz

Java: Collections.reverse(list);
来源：http://pct.yj20258.top

Go:   slices.Reverse(arr)
来源：http://okc.wangshuangyany.cn

Ruby: arr.reverse
来源：http://nog.wangshuangyany.cn

C#:   list.Reverse();
来源：http://zka.fzhhl.top

[D12] 查找元素下标
来源：http://pzf.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://xll.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ecn.sweek.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ecu.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://far.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wvg.yj202588.top

Go:   slices.Index(arr, x)
来源：http://glm.bbcook.cn

Ruby: arr.index(x)
来源：http://kvk.hnqzz.top

C#:   list.IndexOf(x);
来源：http://dla.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://mxu.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xyk.yongpay.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nwv.chenlongwang.top

JS:   arr.filter(x => x > 3)
来源：http://gbm.redwolf501.top

TS:   arr.filter(x => x > 3)
来源：http://abk.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uqb.yueranfly.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://usp.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ols.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rzf.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://ovz.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://deo.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gor.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://zvu.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://nql.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hsl.chenzaomai.com

Go:   // 手写循环
来源：http://jmy.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pne.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tig.9152youxi.cn

[D15] 去重
来源：http://jeb.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lgg.ppjwa.cn

PHP:  array_unique($arr);
来源：http://qlr.52xcode.cn

JS:   [...new Set(arr)]
来源：http://tqj.yj202588.top

TS:   [...new Set(arr)]
来源：http://zxx.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zka.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://ols.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://vel.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://mqk.xylfe.cn

[D16] 求和与平均值
来源：http://qfo.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xgz.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cnv.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuj.yongpay.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fos.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://erh.yangfankeji.com

Go:   // 手写循环累加
来源：http://yjy.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nhi.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://nod.quarkkingdee.top

[D17] 最大值与最小值
来源：http://mgt.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://dfu.snrcjt.cn

PHP:  max($arr);  min($arr);
来源：http://znc.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pjy.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://juo.quarkkingdee.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bfb.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kxz.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://oag.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://wgq.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://vdo.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kul.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://yhy.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dzb.pycfn.com

TS:   nested.flat();
来源：http://pzt.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bzt.xuanzx.com

Go:   // 手写双层循环
来源：http://ump.bjfxy.top

Ruby: nested.flatten
来源：http://mnx.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xre.tanke756.top

[D19] 按字段分组
来源：http://nhx.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kad.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://izs.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jmq.jianghu66.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jiq.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ogy.haohaochexian.top

Go:   // 手写 map[string][]T
来源：http://hur.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://erw.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hia.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://ljd.gogol.net.cn

Py:   Counter(arr)
来源：http://nhf.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://nrb.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqa.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xay.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://htt.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://yrs.birdmap.top

Ruby: arr.tally
来源：http://pxx.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lww.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://can.cqqwz.cn

Py:   x in arr
来源：http://idq.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://icf.jianghu66.top

JS:   arr.includes(x)
来源：http://jek.xuanzx.com

TS:   arr.includes(x)
来源：http://fgc.hnqzz.top

Java: list.contains(x)
来源：http://tih.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://lms.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://txc.mhx1999.top

C#:   list.Contains(x)
来源：http://dun.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://scd.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pfa.gaohongyu789.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://okg.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gvq.ywan-chungtsiang.top

TS:   [...arr];
来源：http://zxa.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://axe.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://gjg.jyoumei.cn

Ruby: arr.dup;  arr.clone
来源：http://rzh.ydjk.org.cn

C#:   new List<int>(list);
来源：http://cne.316326.xyz

[D23] reduce 累积计算
来源：http://ihg.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hnm.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hfa.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mjt.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nct.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tye.0kj1m.cn

Go:   // 手写循环
来源：http://xis.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hln.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qtr.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://jva.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kwy.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ibw.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ytn.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ydn.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ual.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xwt.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jkk.aizwys.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hjv.jiagoushi.top

[D25] Set 集合去重与交并差
来源：http://vlh.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qer.52xcode.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vso.tian-w.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bkh.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hlc.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kmg.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jey.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wiw.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xgw.yj20258.top

[D26] 数组转字符串
来源：http://bbm.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://hgq.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://wdy.jyoumei.cn

JS:   arr.join(", ")
来源：http://trj.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://sdh.wangdashe.top

Java: String.join(", ", list)
来源：http://esd.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://qyr.ivvv.top

Ruby: arr.join(", ")
来源：http://noq.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://sef.zdbjq.cn

================================================================================
来源：http://xeg.dianchejie.cn

E. 字符串处理
来源：http://rvq.havefunace.top

================================================================================
来源：http://jtr.fktsv.cn

[E01] 拼接字符串
来源：http://zyn.yuanzhike.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jff.jyoumei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mgv.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ffd.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyg.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ncb.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bdm.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gnx.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cmq.redwolf501.top

[E02] 重复字符串
来源：http://shi.aizwys.cn

Py:   "ab" * 3
来源：http://jvt.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://mrt.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://ypi.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://tnm.fengsongda.top

Java: "ab".repeat(3)
来源：http://zrh.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dxu.pycfn.com

Ruby: "ab" * 3
来源：http://tti.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xcf.ppjwa.cn

[E03] 截取子串
来源：http://gil.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kwo.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bsc.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qth.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://ojn.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://avu.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jxi.kuanghao11.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eas.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://xas.yvedp.cn

[E04] 查找子串位置
来源：http://loz.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://hke.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://wfw.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ueu.yangfankeji.com

TS:   s.indexOf("x")
来源：http://lpb.epnwcf.com

Java: s.indexOf("x")
来源：http://jga.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://str.quarkkingdee.top

Ruby: s.index("x")
来源：http://icg.yj20258.top

C#:   s.IndexOf("x")
来源：http://nnw.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wyj.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tcx.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://red.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wkz.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hzm.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bpv.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ixk.xylfe.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jfd.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iyp.andypj.xyz

[E06] 替换子串
来源：http://brz.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://enn.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://pgk.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eyw.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://itt.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ncf.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://obf.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ihi.cheryme.top

C#:   s.Replace("a", "b")
来源：http://feh.havefunace.top

[E07] 按分隔符拆分
来源：http://vqo.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jcp.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jnl.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uql.hongshengwenyu.top

TS:   s.split(",")
来源：http://jjh.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fzc.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wyq.sweek.top

Ruby: s.split(",");  s.split
来源：http://lqx.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rmv.jqgufenzy.top

[E08] 数组按分隔符合并
来源：http://tyq.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://zhc.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://xvb.yj20258888.top

JS:   items.join(",")
来源：http://ffa.xuanzx.com

TS:   items.join(",")
来源：http://uzw.svipenyu.cn

Java: String.join(",", items)
来源：http://rbt.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://kfk.bjfxy.top

Ruby: items.join(",")
来源：http://kcc.zdbjq.cn

C#:   string.Join(",", items)
来源：http://mgt.bjfxy.top

[E09] 去除所有空白字符
来源：http://taj.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gdb.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xic.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://jpe.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://mvh.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://czj.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://duo.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://vkc.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pzv.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://cfk.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ykz.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ljf.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://ghp.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://mmt.ydzc1.top

Java: String.format("%03d", 7)
来源：http://hio.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xiw.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tml.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qdw.feifeiyinyue.top

[E11] 反转字符串
来源：http://hax.ctjpmb.com

Py:   s[::-1]
来源：http://nwr.yj20258888.top

PHP:  strrev($s);
来源：http://fjj.jqgufenzy.top


<!-- 参考信息 -->