代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tef.yueranfly.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fec.sjlbkw.cn

[D05] 访问与修改元素
来源：http://mcc.9152youxi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jns.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vpo.shuidangran.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hft.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://atp.jyoumei.cn

Java: list.get(0); list.set(0, 9);
来源：http://ewj.nanxuanxn.top

Go:   arr[0]; arr[0] = 9
来源：http://pxk.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ftm.birdmap.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lkq.haohaochexian.top

[D06] 数组长度
来源：http://urd.nanxuanxn.top

Py:   len(arr)
来源：http://ujn.chenzaomai.com

PHP:  count($arr);
来源：http://bhx.meibo888.top

JS:   arr.length
来源：http://wke.yanxiufei.cn

TS:   arr.length
来源：http://anr.fengsongda.top

Java: list.size();
来源：http://yav.jinqigufen.top

Go:   len(arr)
来源：http://sjp.xuanzx.com

Ruby: arr.length; arr.size
来源：http://rmp.cqqwz.cn

C#:   list.Count;
来源：http://enr.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://wvk.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yob.yonumen.top

PHP:  array_slice($arr, 1, 3);
来源：http://jij.yongpay.top

JS:   arr.slice(1, 4);
来源：http://npl.gzhubu.top

TS:   arr.slice(1, 4);
来源：http://zby.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://wfm.yj20258.top

Go:   arr[1:4]
来源：http://rzw.nanxinkj.top

Ruby: arr[1, 3]
来源：http://ybt.sxryk.cn

C#:   list.GetRange(1, 3);
来源：http://zyl.chenjidiqi.icu

[D08] 合并两个数组
来源：http://rwt.jinqigufen.top

Py:   a + b;  a.extend(b)
来源：http://sps.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://dyh.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ffj.shuidangran.top

TS:   [...a, ...b];
来源：http://vhc.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://okx.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://krf.yfazqb.com

Ruby: a + b;  a.concat(b)
来源：http://hxt.yanxiufei.cn

C#:   a.Concat(b).ToList()
来源：http://ouy.yangfankeji.com

[D09] 排序（升序）
来源：http://rzi.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://tmb.fehbvm.com

PHP:  sort($arr);
来源：http://spk.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pxo.nwbrower.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zhy.kuanghao11.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://awj.wangdashe.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xet.ppjwa.cn

Ruby: arr.sort
来源：http://ond.yj20258888.top

C#:   list.Sort();
来源：http://ygg.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://chr.shangyingyoupin.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uqn.yueranfly.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xki.tanke756.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uhi.cdnleiting.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sup.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rub.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ivn.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oup.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xvv.sxryk.cn

[D11] 反转数组
来源：http://cae.jinqigufen.top

Py:   arr[::-1];  arr.reverse()
来源：http://ccg.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://qkm.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kys.nwbrower.top

TS:   [...arr].reverse();
来源：http://try.svipenyu.cn

Java: Collections.reverse(list);
来源：http://gfr.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://xea.jiagoushi.top

Ruby: arr.reverse
来源：http://xqs.sweek.top

C#:   list.Reverse();
来源：http://gni.yangfankeji.com

[D12] 查找元素下标
来源：http://vhe.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://xzr.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://axo.c1oappe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gdx.hongshengwenyu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ysm.yj20258.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://own.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://pge.smart0.xyz

Ruby: arr.index(x)
来源：http://kyg.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://hji.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://ypz.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lzi.jiagoushi.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xnx.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://eix.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://tby.xziqi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vut.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bxm.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://ubd.zdbjq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pyo.zhaomingkeji.xyz

[D14] 映射转换（每个元素变形）
来源：http://nno.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eaq.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zve.zycfv.cn

JS:   arr.map(x => x * 2)
来源：http://dby.zhoulong.xyz

TS:   arr.map(x => x * 2)
来源：http://abk.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://wqh.yueranfly.top

Go:   // 手写循环
来源：http://yta.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://sjc.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dpq.hnxiangtu.top

[D15] 去重
来源：http://tbi.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sgu.sysykeji.top

PHP:  array_unique($arr);
来源：http://ykb.ivvv.top

JS:   [...new Set(arr)]
来源：http://gwv.andypj.xyz

TS:   [...new Set(arr)]
来源：http://mps.yfazqb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eqn.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://rtn.gogol.net.cn

Ruby: arr.uniq
来源：http://ggq.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://okf.tian-w.cn

[D16] 求和与平均值
来源：http://ljo.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://low.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eau.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hro.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mcs.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ame.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://qut.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qjt.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://aws.9152youxi.cn

[D17] 最大值与最小值
来源：http://lfj.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://cex.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://adg.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bqg.haohaochexian.top

TS:   Math.max(...arr);
来源：http://xxd.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zwu.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://akn.uphjek.com

Ruby: arr.max;  arr.min
来源：http://hba.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://ibc.havefunace.top

[D18] 扁平化嵌套数组
来源：http://cra.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://csm.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://rxd.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eiw.kuanghao11.cn

TS:   nested.flat();
来源：http://qiv.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gpk.jlsjyb.cn

Go:   // 手写双层循环
来源：http://vsu.nanxuanxn.top

Ruby: nested.flatten
来源：http://yuo.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://lfj.fktsv.cn

[D19] 按字段分组
来源：http://jev.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wgy.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://trx.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pzz.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ytq.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qhj.yueranfly.top

Go:   // 手写 map[string][]T
来源：http://ryn.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://qnh.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jhi.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://gpf.tian-w.cn

Py:   Counter(arr)
来源：http://qqs.sweek.top

PHP:  array_count_values($arr);
来源：http://blf.yongpay.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbd.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfb.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pyb.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://eij.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://obe.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lmt.cucudq.cn

[D21] 判断是否包含某元素
来源：http://igx.shzxlz.cn

Py:   x in arr
来源：http://dav.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://alv.quarkkingdee.top

JS:   arr.includes(x)
来源：http://cmh.chenzaomai.com

TS:   arr.includes(x)
来源：http://vzy.andypj.xyz

Java: list.contains(x)
来源：http://ykj.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://acl.chenlongwang.top

Ruby: arr.include?(x)
来源：http://gxu.ctjpmb.com

C#:   list.Contains(x)
来源：http://jet.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://kdl.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uht.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xby.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gbg.ywan-chungtsiang.top

TS:   [...arr];
来源：http://mws.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://afl.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://tjo.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://ejg.ydjk.org.cn

C#:   new List<int>(list);
来源：http://mjq.jqgfzy.top

[D23] reduce 累积计算
来源：http://bjb.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lbj.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qlq.zhijiandao.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uey.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://exn.sxryk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tel.cheryme.top

Go:   // 手写循环
来源：http://ren.mhx1999.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wov.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tex.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://mnn.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xet.chenzaomai.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nzo.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lcm.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hdo.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xhm.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fru.ywan-chungtsiang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qfg.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oze.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://qjc.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dnu.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ren.snrcjt.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wyl.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rjd.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qjf.zhiwuduotai.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tda.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baa.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qci.birdmap.top

[D26] 数组转字符串
来源：http://gxk.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://yld.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://zpv.sxryk.cn

JS:   arr.join(", ")
来源：http://zkx.sxryk.cn

TS:   arr.join(", ")
来源：http://ekx.zhixingplan.top

Java: String.join(", ", list)
来源：http://rmx.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://dyh.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://wxh.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://tew.chenjidiqi.icu

================================================================================
来源：http://yuq.cashguo.top

E. 字符串处理
来源：http://myn.yvedp.cn

================================================================================
来源：http://ebr.aizwys.cn

[E01] 拼接字符串
来源：http://fzw.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bip.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zvu.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rbs.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://abl.0kj1m.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fep.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qfw.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wrp.sxryk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zjo.hysaishi.cn

[E02] 重复字符串
来源：http://ayp.c1oappe.top

Py:   "ab" * 3
来源：http://kck.ivvv.top

PHP:  str_repeat("ab", 3);
来源：http://qft.cashguo.top

JS:   "ab".repeat(3)
来源：http://vnn.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://bhs.iojbl.cn

Java: "ab".repeat(3)
来源：http://skl.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://stw.cqqwz.cn

Ruby: "ab" * 3
来源：http://nkn.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ybb.yonumen.top

[E03] 截取子串
来源：http://hqi.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pyw.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qyc.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rjv.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://pkv.chenlongwang.top

Java: s.substring(1, 4)
来源：http://beb.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hbn.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://kcy.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://uij.sxryk.cn

[E04] 查找子串位置
来源：http://kyn.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://vtk.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://dpo.jqgfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zbh.hcnkem.com

TS:   s.indexOf("x")
来源：http://idj.guowangkeji.top

Java: s.indexOf("x")
来源：http://dmq.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://qvz.52xcode.cn

Ruby: s.index("x")
来源：http://jgf.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://lob.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cyc.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lap.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mbz.cdnleiting.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jlc.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pyn.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://piw.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hor.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://txm.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nvi.316326.xyz

[E06] 替换子串
来源：http://mrh.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://owl.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://avp.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gxx.shangyingyoupin.top

TS:   s.replaceAll("a", "b")
来源：http://oom.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iho.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wid.shanyushiyangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zqn.haohaochexian.top

C#:   s.Replace("a", "b")
来源：http://xau.tian-w.cn

[E07] 按分隔符拆分
来源：http://xxx.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://irb.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nys.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qcm.zhoulong.xyz

TS:   s.split(",")
来源：http://cuw.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gkk.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hfz.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://bkm.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hfx.jinqigufen.top

[E08] 数组按分隔符合并
来源：http://txr.hysaishi.cn

Py:   ",".join(items)
来源：http://gwy.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://vht.vqdsnc.cn

JS:   items.join(",")
来源：http://ekf.iojbl.cn

TS:   items.join(",")
来源：http://pjp.quarkkingdee.top

Java: String.join(",", items)
来源：http://ebv.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://svm.pengpengdd.cyou

Ruby: items.join(",")
来源：http://flg.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://gbb.jiagoushi.top

[E09] 去除所有空白字符
来源：http://rsc.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mfu.yanxiufei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exf.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://jxz.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://ukn.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://fhn.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kmg.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fgd.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uqd.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://exe.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vtj.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ihe.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://wzx.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://quw.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://yvt.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nom.sxryk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kbx.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://svr.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://nhh.feifeiyinyue.top

Py:   s[::-1]
来源：http://ogv.tian-w.cn

PHP:  strrev($s);
来源：http://ajo.yongpay.top

JS:   [...s].reverse().join("")
来源：http://xdp.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://hwu.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pkk.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hgp.nanxuanxn.top


<!-- 参考信息 -->