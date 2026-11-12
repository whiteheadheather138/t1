代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://cgq.aizwys.cn

Java: list.add(0, 0);
来源：http://iyg.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ike.jinyuanbaomall.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tkr.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://yrf.nwbrower.top

[D04] 删除元素
来源：http://nst.gogol.net.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xnw.daxiang520.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mdx.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qvw.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://ytm.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rep.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ifp.mhx1999.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ieg.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zda.vehdjk.com

[D05] 访问与修改元素
来源：http://vaf.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tkq.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wnp.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ica.ybcxt.top

TS:   arr[0]; arr.at(-1);
来源：http://wlw.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://lbo.jqgufenzy.top

Go:   arr[0]; arr[0] = 9
来源：http://dhk.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qcd.jianghu66.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://byl.hywenlv.cn

[D06] 数组长度
来源：http://izf.quarkkingdee.top

Py:   len(arr)
来源：http://mfi.guannengcc.top

PHP:  count($arr);
来源：http://raq.wangdashe.top

JS:   arr.length
来源：http://cek.shzxlz.cn

TS:   arr.length
来源：http://jpx.sxryk.cn

Java: list.size();
来源：http://gyp.feifeiyinyue.top

Go:   len(arr)
来源：http://jvp.yvedp.cn

Ruby: arr.length; arr.size
来源：http://nrh.zhaomingkeji.xyz

C#:   list.Count;
来源：http://zkl.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://yzx.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bqr.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://ert.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://pbe.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://ybe.hfpthk.cn

Java: list.subList(1, 4);
来源：http://sgr.bbcook.cn

Go:   arr[1:4]
来源：http://kdw.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://djp.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://nbu.yuanzhike.top

[D08] 合并两个数组
来源：http://dhu.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://suo.yfazqb.com

PHP:  array_merge($a, $b);
来源：http://qvd.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tpg.hesvh.cn

TS:   [...a, ...b];
来源：http://fkx.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ihd.yfazqb.com

Go:   append(a, b...)
来源：http://mmf.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://nlk.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://vrv.xingfuxueyuan.xyz

[D09] 排序（升序）
来源：http://xqb.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://opn.fengsongda.top

PHP:  sort($arr);
来源：http://mgm.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ncm.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ykv.yfazqb.com

Java: Collections.sort(list);  list.sort(null);
来源：http://wvi.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hjb.sweek.top

Ruby: arr.sort
来源：http://dsv.sxryk.cn

C#:   list.Sort();
来源：http://ksg.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://wsu.tianlin.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qta.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yvo.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uki.yuanzhike.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfz.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ypb.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bdn.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ksn.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tlr.yonumen.top

[D11] 反转数组
来源：http://fzr.wangshuangyany.cn

Py:   arr[::-1];  arr.reverse()
来源：http://can.daxiang520.top

PHP:  array_reverse($arr);
来源：http://idb.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tak.zhaomingkeji.xyz

TS:   [...arr].reverse();
来源：http://vtb.birdmap.top

Java: Collections.reverse(list);
来源：http://hng.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://fcr.zhiwuduotai.top

Ruby: arr.reverse
来源：http://apn.hcnkem.com

C#:   list.Reverse();
来源：http://gia.hcnkem.com

[D12] 查找元素下标
来源：http://ztg.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://wyg.ywan-chungtsiang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nib.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gyw.yfazqb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hqa.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xco.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://wxh.jyoumei.cn

Ruby: arr.index(x)
来源：http://tpd.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://nnv.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://ekf.sysykeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yxn.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vaa.svipenyu.cn

JS:   arr.filter(x => x > 3)
来源：http://gpc.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://hbl.chenlongwang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vcb.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pmh.epnwcf.com

Ruby: arr.select { |x| x > 3 }
来源：http://ety.daxiang520.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uvw.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://mdo.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rsw.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yft.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://zsv.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://rvi.ppjwa.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://npg.pycfn.com

Go:   // 手写循环
来源：http://cqr.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jym.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://beg.fktsv.cn

[D15] 去重
来源：http://kbu.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dvs.bjfxy.top

PHP:  array_unique($arr);
来源：http://wnb.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://xoh.yuxming.cn

TS:   [...new Set(arr)]
来源：http://rxk.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zlo.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://frr.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://vkc.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://rfw.dashuyun.cn

[D16] 求和与平均值
来源：http://kap.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oed.meibo888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uny.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nrx.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kal.yanxiufei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hgg.hfpthk.cn

Go:   // 手写循环累加
来源：http://fre.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uty.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://glf.cheryme.top

[D17] 最大值与最小值
来源：http://pui.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://axf.chenlongwang.top

PHP:  max($arr);  min($arr);
来源：http://kag.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sgh.chenlongwang.top

TS:   Math.max(...arr);
来源：http://sdt.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ymt.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mit.yongpay.top

Ruby: arr.max;  arr.min
来源：http://lpn.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://yws.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://dlr.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://csw.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://bze.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tdi.nanxuanxn.top

TS:   nested.flat();
来源：http://jyg.hfpthk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cwq.hongshengwenyu.top

Go:   // 手写双层循环
来源：http://sjd.xuetiantiany.cn

Ruby: nested.flatten
来源：http://obz.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://msf.kuanghao11.cn

[D19] 按字段分组
来源：http://lcd.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tjs.ybcxt.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ugr.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vll.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://csi.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yqp.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://ywm.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kde.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wnx.yj202588.top

[D20] 统计每个元素出现次数
来源：http://tbn.feifeiyinyue.top

Py:   Counter(arr)
来源：http://edg.bjfxy.top

PHP:  array_count_values($arr);
来源：http://gfh.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wva.dashuyun.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sdq.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ptp.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://nep.xuetiantiany.cn

Ruby: arr.tally
来源：http://cku.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gzd.jianghu66.top

[D21] 判断是否包含某元素
来源：http://pko.zdbjq.cn

Py:   x in arr
来源：http://wnl.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://lad.hnqzz.top

JS:   arr.includes(x)
来源：http://tsa.dashuyun.cn

TS:   arr.includes(x)
来源：http://gxu.bjfxy.top

Java: list.contains(x)
来源：http://mbl.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://zuh.hnqzz.top

Ruby: arr.include?(x)
来源：http://ewn.yanxiufei.cn

C#:   list.Contains(x)
来源：http://nof.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://oqi.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tuf.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lda.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cwu.aizwys.cn

TS:   [...arr];
来源：http://lti.zhengqikj.top

Java: new ArrayList<>(list);
来源：http://bbx.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dok.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://zjx.gzhubu.top

C#:   new List<int>(list);
来源：http://kpw.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://fnv.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yea.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zna.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dri.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://evx.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xbz.tanke756.top

Go:   // 手写循环
来源：http://euo.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eec.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ona.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://ytk.9152youxi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dhk.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ojc.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pmk.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dpc.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://njn.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jwa.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jea.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xyf.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://joq.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xrl.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrs.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bxn.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kst.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://koh.daxiang520.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wcj.xuetiantiany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kkq.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dcp.cashguo.top

[D26] 数组转字符串
来源：http://orm.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://cta.yongpay.top

PHP:  implode(", ", $arr);
来源：http://cmu.ydjk.org.cn

JS:   arr.join(", ")
来源：http://zeo.zhixingplan.top

TS:   arr.join(", ")
来源：http://vit.havefunace.top

Java: String.join(", ", list)
来源：http://jid.guannengcc.top

Go:   strings.Join(strs, ", ")
来源：http://rqs.dianchejie.cn

Ruby: arr.join(", ")
来源：http://ouq.fzhhl.top

C#:   string.Join(", ", list)
来源：http://hix.hammf.cn

================================================================================
来源：http://syx.gaohongyu789.top

E. 字符串处理
来源：http://jkj.aibaodan.cn

================================================================================
来源：http://fmg.tarul.cn

[E01] 拼接字符串
来源：http://nxm.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://stk.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nzo.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyh.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bil.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kle.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cvl.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ile.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uvu.jinqigfzy.top

[E02] 重复字符串
来源：http://xqr.chenlongwang.top

Py:   "ab" * 3
来源：http://wft.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://acy.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://orm.tian-w.cn

TS:   "ab".repeat(3)
来源：http://mut.epnwcf.com

Java: "ab".repeat(3)
来源：http://rha.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ayi.andypj.xyz

Ruby: "ab" * 3
来源：http://dtq.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wcu.xuetiantiany.cn

[E03] 截取子串
来源：http://oeq.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yyo.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://akb.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://utt.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://xsv.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://dsm.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jxv.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://mtg.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://msa.dashuyun.cn

[E04] 查找子串位置
来源：http://gmj.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://bni.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://kmw.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fbg.zdqjudy.top

TS:   s.indexOf("x")
来源：http://shd.xinyue.icu

Java: s.indexOf("x")
来源：http://dvt.yanxiufei.cn

Go:   strings.Index(s, "x")
来源：http://bzg.ydzc1.top

Ruby: s.index("x")
来源：http://ksk.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://sor.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cor.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tli.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://woz.ybcxt.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ona.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xse.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qps.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yiz.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xqr.daria6918.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lbn.yanxiufei.cn

[E06] 替换子串
来源：http://zgm.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sax.nwbrower.top

PHP:  str_replace("a", "b", $s);
来源：http://psi.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ioz.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://kpy.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qbt.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ths.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ddi.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://fmw.shzxlz.cn

[E07] 按分隔符拆分
来源：http://mif.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pdk.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ikl.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://clk.zhongyouzk.top

TS:   s.split(",")
来源：http://uvr.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://jrx.pengpengdd.cyou

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qgx.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://uwt.zdqjudy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xtg.hammf.cn

[E08] 数组按分隔符合并
来源：http://nrb.cucudq.cn

Py:   ",".join(items)
来源：http://qgp.shuidangran.top

PHP:  implode(",", $items);
来源：http://rjv.guannengcc.top

JS:   items.join(",")
来源：http://hbw.xinyue.icu

TS:   items.join(",")
来源：http://atb.fktsv.cn

Java: String.join(",", items)
来源：http://nyd.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://ydv.snrcjt.cn

Ruby: items.join(",")
来源：http://ymn.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://yvm.cucudq.cn

[E09] 去除所有空白字符
来源：http://vdl.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wfq.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ekg.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://wex.shanyushiyangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://pgd.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://lix.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xod.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ryx.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gej.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://okg.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tnx.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zaj.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://kbu.zhoulong.xyz


<!-- 参考信息 -->