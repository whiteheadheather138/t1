代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://okt.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ruj.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://ukw.birdmap.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jjg.ctjpmb.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xhs.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gzm.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wzm.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://zjk.yongpay.top

Go:   arr[0]; arr[0] = 9
来源：http://gqe.cheryme.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wrv.bbcook.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pwn.smart0.xyz

[D06] 数组长度
来源：http://ugf.chenzaomai.com

Py:   len(arr)
来源：http://min.aizwys.cn

PHP:  count($arr);
来源：http://xvc.iojbl.cn

JS:   arr.length
来源：http://cok.cdnleiting.top

TS:   arr.length
来源：http://bmc.fanxiaobao.xyz

Java: list.size();
来源：http://exc.gogol.net.cn

Go:   len(arr)
来源：http://ref.aizwys.cn

Ruby: arr.length; arr.size
来源：http://aok.guannengcc.top

C#:   list.Count;
来源：http://qzg.pycfn.com

[D07] 切片 / 取子数组
来源：http://wwo.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ugq.epnwcf.com

PHP:  array_slice($arr, 1, 3);
来源：http://nru.hnxiangtu.top

JS:   arr.slice(1, 4);
来源：http://wqn.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://hbh.bbcook.cn

Java: list.subList(1, 4);
来源：http://fwu.cheryme.top

Go:   arr[1:4]
来源：http://ord.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://ceq.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://fde.meibo888.top

[D08] 合并两个数组
来源：http://lxa.hfpthk.cn

Py:   a + b;  a.extend(b)
来源：http://bsh.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://tts.guowangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fxa.dianchejie.cn

TS:   [...a, ...b];
来源：http://cxv.yj20258.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tdv.sjlbkw.cn

Go:   append(a, b...)
来源：http://wdh.hywenlv.cn

Ruby: a + b;  a.concat(b)
来源：http://hiy.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://foj.xinyue.icu

[D09] 排序（升序）
来源：http://heo.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://sgf.52xcode.cn

PHP:  sort($arr);
来源：http://tac.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jhc.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uig.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jqq.hcnkem.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yqv.chenzaomai.com

Ruby: arr.sort
来源：http://qgg.aizwys.cn

C#:   list.Sort();
来源：http://wjo.jqgfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pgh.fehbvm.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wsj.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rvz.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lax.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sqx.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xxo.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kus.jiagoushi.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zjd.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jpx.aizwys.cn

[D11] 反转数组
来源：http://kev.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://tba.uphjek.com

PHP:  array_reverse($arr);
来源：http://hje.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tyi.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://yip.tanke756.top

Java: Collections.reverse(list);
来源：http://jim.jqgufenzy.top

Go:   slices.Reverse(arr)
来源：http://naf.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://nzk.fehbvm.com

C#:   list.Reverse();
来源：http://vsk.zhijiandao.cn

[D12] 查找元素下标
来源：http://ymm.yangfankeji.com

Py:   arr.index(x);  x in arr
来源：http://uhe.hfpthk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gub.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kwl.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://edn.feifeiyinyue.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://adn.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://rkd.chenjidiqi.icu

Ruby: arr.index(x)
来源：http://ztq.meibo888.top

C#:   list.IndexOf(x);
来源：http://bky.meibo888.top

[D13] 过滤（保留满足条件的）
来源：http://obt.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://biv.svipenyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qwp.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://mkp.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://gax.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pbp.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vkk.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://hri.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zll.birdmap.top

[D14] 映射转换（每个元素变形）
来源：http://etn.shuidangran.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hsw.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ckq.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://ige.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://jni.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wfe.pycfn.com

Go:   // 手写循环
来源：http://bwo.zdqjudy.top

Ruby: arr.map { |x| x * 2 }
来源：http://hza.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hct.jianghu66.top

[D15] 去重
来源：http://egc.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tuo.hcnkem.com

PHP:  array_unique($arr);
来源：http://qwr.pengpengdd.cyou

JS:   [...new Set(arr)]
来源：http://mfy.fktsv.cn

TS:   [...new Set(arr)]
来源：http://vyv.xylfe.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xaf.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://hii.yuxming.cn

Ruby: arr.uniq
来源：http://gbq.ivvv.top

C#:   list.Distinct().ToList()
来源：http://xgw.tianlin.xyz

[D16] 求和与平均值
来源：http://soa.jinyuanbaomall.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zmi.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dvk.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sdp.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qip.nanxuanxn.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lxw.xziqi.cn

Go:   // 手写循环累加
来源：http://msc.feifeiyinyue.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xfs.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://tuj.hesvh.cn

[D17] 最大值与最小值
来源：http://azk.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://fzt.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://jlh.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eii.pycfn.com

TS:   Math.max(...arr);
来源：http://itd.gzhubu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://idg.hesvh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gku.smart0.xyz

Ruby: arr.max;  arr.min
来源：http://epm.sweek.top

C#:   list.Max();  list.Min()
来源：http://flp.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://myn.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wcj.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://sfq.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cij.epnwcf.com

TS:   nested.flat();
来源：http://fpk.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://imh.yj20258888.top

Go:   // 手写双层循环
来源：http://zlu.gotoacloud.top

Ruby: nested.flatten
来源：http://uka.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tpx.quarkkingdee.top

[D19] 按字段分组
来源：http://wlz.hcnkem.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zkt.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zfa.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tut.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cjo.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hgv.chenzaomai.com

Go:   // 手写 map[string][]T
来源：http://zjo.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mlv.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bqh.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://uhz.jiagoushi.top

Py:   Counter(arr)
来源：http://nui.shangyingyoupin.top

PHP:  array_count_values($arr);
来源：http://leh.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ixe.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyk.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rlt.sweek.top

Go:   // 手写 map[T]int
来源：http://ydx.yj20258.top

Ruby: arr.tally
来源：http://dvx.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mev.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://dnb.gzhubu.top

Py:   x in arr
来源：http://jbl.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://vhq.hnqzz.top

JS:   arr.includes(x)
来源：http://joe.smart0.xyz

TS:   arr.includes(x)
来源：http://jrl.redwolf501.top

Java: list.contains(x)
来源：http://enh.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://kkm.pycfn.com

Ruby: arr.include?(x)
来源：http://tsv.dashuyun.cn

C#:   list.Contains(x)
来源：http://erp.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://ogh.9152youxi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://evs.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ogx.gzhubu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kxa.smart0.xyz

TS:   [...arr];
来源：http://dre.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://biz.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://xyz.shanyushiyangtech.top

Ruby: arr.dup;  arr.clone
来源：http://ygh.haohaochexian.top

C#:   new List<int>(list);
来源：http://qsf.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://qmd.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gmq.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ukl.ydzc1.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vml.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xai.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xcj.ybcxt.top

Go:   // 手写循环
来源：http://dyw.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ojs.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eto.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://uzp.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bks.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lve.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iip.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mjq.epnwcf.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jao.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cre.zhoulong.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tkr.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cgq.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://qdv.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kep.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://haa.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dfn.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://put.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ser.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qsz.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aky.aizwys.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pbe.cashguo.top

[D26] 数组转字符串
来源：http://stq.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://gva.yangfankeji.com

PHP:  implode(", ", $arr);
来源：http://sup.ybcxt.top

JS:   arr.join(", ")
来源：http://qxt.jqgufenzy.top

TS:   arr.join(", ")
来源：http://oep.yangfankeji.com

Java: String.join(", ", list)
来源：http://qhf.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://atj.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://alv.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://xpt.hongshengwenyu.top

================================================================================
来源：http://sej.birdmap.top

E. 字符串处理
来源：http://qxu.shangyingyoupin.top

================================================================================
来源：http://pav.hnxiangtu.top

[E01] 拼接字符串
来源：http://wjr.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wpk.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fyo.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hkq.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ook.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://esr.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hyh.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sjv.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iyu.wangdashe.top

[E02] 重复字符串
来源：http://qrx.chenjidiqi.icu

Py:   "ab" * 3
来源：http://mxd.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://ypp.zdbjq.cn

JS:   "ab".repeat(3)
来源：http://bbh.sxryk.cn

TS:   "ab".repeat(3)
来源：http://fox.iojbl.cn

Java: "ab".repeat(3)
来源：http://dsc.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://ugq.yfazqb.com

Ruby: "ab" * 3
来源：http://btl.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nce.aizwys.cn

[E03] 截取子串
来源：http://ruf.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cvp.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oau.quarkkingdee.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kyz.daria6918.cn

TS:   s.slice(1, 4)
来源：http://abe.havefunace.top

Java: s.substring(1, 4)
来源：http://iey.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://idt.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://krj.yfazqb.com

C#:   s.Substring(1, 3)
来源：http://ltr.zdqjudy.top

[E04] 查找子串位置
来源：http://fqg.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://oop.bbcook.cn

PHP:  strpos($s, "x");
来源：http://pkj.yongpay.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jkh.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://coi.ybcxt.top

Java: s.indexOf("x")
来源：http://uzp.fanxiaobao.xyz

Go:   strings.Index(s, "x")
来源：http://ncq.feifeiyinyue.top

Ruby: s.index("x")
来源：http://fkv.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://zae.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://fvq.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qbn.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wmq.cucudq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gtu.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ujq.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://diz.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wdv.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvv.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kij.dashuyun.cn

[E06] 替换子串
来源：http://pwp.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uey.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://nun.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpk.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://hyd.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pfr.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hhl.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jei.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://rhu.tianlin.xyz

[E07] 按分隔符拆分
来源：http://rns.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kwm.cdnleiting.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nwr.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bdf.yongpay.top

TS:   s.split(",")
来源：http://mno.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://bxj.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://syy.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://yld.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qlb.yuanzhike.top

[E08] 数组按分隔符合并
来源：http://qrt.ctjpmb.com

Py:   ",".join(items)
来源：http://pjo.zhengqikj.top

PHP:  implode(",", $items);
来源：http://ili.ydjk.org.cn

JS:   items.join(",")
来源：http://cfe.tarul.cn

TS:   items.join(",")
来源：http://xzv.zdqjudy.top

Java: String.join(",", items)
来源：http://ihq.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://duv.daria6918.cn

Ruby: items.join(",")
来源：http://odj.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://hpk.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://acs.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mlb.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://etj.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://ndx.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://blj.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://bdw.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://afl.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://mfc.hfpthk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bmt.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://wul.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yjl.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ofg.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://xmb.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://kfn.sxryk.cn

Java: String.format("%03d", 7)
来源：http://gtc.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://waz.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ybm.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rfm.fzhhl.top

[E11] 反转字符串
来源：http://afk.52xcode.cn

Py:   s[::-1]
来源：http://luq.chenjidiqi.icu

PHP:  strrev($s);
来源：http://rrm.316326.xyz

JS:   [...s].reverse().join("")
来源：http://mzj.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://rkc.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qkv.haohaochexian.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://myu.hysaishi.cn


<!-- 参考信息 -->