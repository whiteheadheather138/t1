代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tic.hysaishi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ncl.feifeiyinyue.top

TS:   arr[0]; arr.at(-1);
来源：http://xdv.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://wwg.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://wvo.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hhp.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://abl.aibaodan.cn

[D06] 数组长度
来源：http://nky.feifeiyinyue.top

Py:   len(arr)
来源：http://nnz.cqqwz.cn

PHP:  count($arr);
来源：http://ggx.yanxiufei.cn

JS:   arr.length
来源：http://tiy.sysykeji.top

TS:   arr.length
来源：http://dxi.nwbrower.top

Java: list.size();
来源：http://bwz.ywan-chungtsiang.top

Go:   len(arr)
来源：http://tiy.bjfxy.top

Ruby: arr.length; arr.size
来源：http://gba.yanxiufei.cn

C#:   list.Count;
来源：http://jbw.cheryme.top

[D07] 切片 / 取子数组
来源：http://xmb.shanyushiyangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://syu.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://ent.jiagoushi.top

JS:   arr.slice(1, 4);
来源：http://bgc.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://jfe.smart0.xyz

Java: list.subList(1, 4);
来源：http://szr.52xcode.cn

Go:   arr[1:4]
来源：http://ayb.meibo888.top

Ruby: arr[1, 3]
来源：http://ilo.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://ulz.zhiwuduotai.top

[D08] 合并两个数组
来源：http://wed.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://omi.birdmap.top

PHP:  array_merge($a, $b);
来源：http://vov.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tia.hnxiangtu.top

TS:   [...a, ...b];
来源：http://ssq.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cjl.yuxming.cn

Go:   append(a, b...)
来源：http://psv.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://kzk.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://cfw.jiagoushi.top

[D09] 排序（升序）
来源：http://tlg.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://umk.fehbvm.com

PHP:  sort($arr);
来源：http://mgw.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://syq.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fbf.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://ioz.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sgu.ehwqpu.com

Ruby: arr.sort
来源：http://keo.sysykeji.top

C#:   list.Sort();
来源：http://ayw.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rvi.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zus.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ukq.ctjpmb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ejx.gaohongyu789.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nkp.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://skb.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ghr.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kxz.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://slf.birdmap.top

[D11] 反转数组
来源：http://hrt.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://gdh.yonumen.top

PHP:  array_reverse($arr);
来源：http://niv.vqdsnc.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gcd.ivvv.top

TS:   [...arr].reverse();
来源：http://wcs.yvedp.cn

Java: Collections.reverse(list);
来源：http://gmm.hesvh.cn

Go:   slices.Reverse(arr)
来源：http://jit.guowangkeji.top

Ruby: arr.reverse
来源：http://duk.sxryk.cn

C#:   list.Reverse();
来源：http://fyv.aibaodan.cn

[D12] 查找元素下标
来源：http://bwb.ydzc1.top

Py:   arr.index(x);  x in arr
来源：http://kag.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://skt.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://orf.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xyt.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lao.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://uzt.yangfankeji.com

Ruby: arr.index(x)
来源：http://xui.daxiang520.top

C#:   list.IndexOf(x);
来源：http://rgw.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://euc.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mdc.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sog.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://aah.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://fag.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vii.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ymo.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://mae.yuanzhike.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qlo.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://tmi.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zow.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://krb.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://tud.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://mef.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wnq.hysaishi.cn

Go:   // 手写循环
来源：http://aef.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://sxv.zhengqikj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fkj.yanxiufei.cn

[D15] 去重
来源：http://xnz.fanxiaobao.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iwf.yueranfly.top

PHP:  array_unique($arr);
来源：http://wyc.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://iir.guowangkeji.top

TS:   [...new Set(arr)]
来源：http://ufk.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sxg.ywan-chungtsiang.top

Go:   // 用 map[T]struct{} 手写
来源：http://nxb.yonumen.top

Ruby: arr.uniq
来源：http://rmh.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://dca.jinqigufen.top

[D16] 求和与平均值
来源：http://eyy.c1oappe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yjr.yonumen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rxd.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dom.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zts.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qwg.andypj.xyz

Go:   // 手写循环累加
来源：http://kov.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fjm.tian-w.cn

C#:   list.Sum();  list.Average()
来源：http://hwe.pengpengdd.cyou

[D17] 最大值与最小值
来源：http://ocs.uphjek.com

Py:   max(arr);  min(arr)
来源：http://uxi.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://wln.jqgufenzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qdm.guowangkeji.top

TS:   Math.max(...arr);
来源：http://idw.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yti.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hqr.tarul.cn

Ruby: arr.max;  arr.min
来源：http://aox.meibo888.top

C#:   list.Max();  list.Min()
来源：http://kiz.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://lsg.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://odt.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://kjp.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iky.bjfxy.top

TS:   nested.flat();
来源：http://nac.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mwz.sxryk.cn

Go:   // 手写双层循环
来源：http://yde.jianghu66.top

Ruby: nested.flatten
来源：http://clt.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jhq.xuetiantiany.cn

[D19] 按字段分组
来源：http://fvz.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ydz.jiagoushi.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kfi.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zan.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://anb.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://klx.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://rta.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kxc.yuanzhike.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cef.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://ysp.guowangkeji.top

Py:   Counter(arr)
来源：http://ixv.daxiang520.top

PHP:  array_count_values($arr);
来源：http://rca.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rat.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ckg.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxm.yangfankeji.com

Go:   // 手写 map[T]int
来源：http://jpa.pycfn.com

Ruby: arr.tally
来源：http://uth.zhoulong.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pdf.yonumen.top

[D21] 判断是否包含某元素
来源：http://uoi.hysaishi.cn

Py:   x in arr
来源：http://qpa.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://cxq.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://lru.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://adt.iojbl.cn

Java: list.contains(x)
来源：http://mgz.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://ytw.smart0.xyz

Ruby: arr.include?(x)
来源：http://orx.bjfxy.top

C#:   list.Contains(x)
来源：http://tyx.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://bsc.zhixingplan.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ytv.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mtl.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hll.nwbrower.top

TS:   [...arr];
来源：http://ilv.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://kth.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cah.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://rnt.xinyue.icu

C#:   new List<int>(list);
来源：http://exj.xuanzx.com

[D23] reduce 累积计算
来源：http://bsb.shangyingyoupin.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gps.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zgr.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ort.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ixo.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hzv.tianlin.xyz

Go:   // 手写循环
来源：http://gnq.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tbs.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nlf.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://jsf.zhaomingkeji.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://utq.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mag.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uhu.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ckh.nwbrower.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://umd.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bvz.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ltu.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dec.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://zqk.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uve.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xfm.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ser.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vgn.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qsr.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rpz.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vjx.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xds.fktsv.cn

[D26] 数组转字符串
来源：http://kzf.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://tlm.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://zrc.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://mrx.fehbvm.com

TS:   arr.join(", ")
来源：http://jpx.jqgfzy.top

Java: String.join(", ", list)
来源：http://ams.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://rwn.ydzc1.top

Ruby: arr.join(", ")
来源：http://afc.daxiang520.top

C#:   string.Join(", ", list)
来源：http://fll.zhoulong.xyz

================================================================================
来源：http://nta.chenjidiqi.icu

E. 字符串处理
来源：http://tnz.ctjpmb.com

================================================================================
来源：http://qqc.bbcook.cn

[E01] 拼接字符串
来源：http://nkz.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://trr.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zpg.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ojm.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iyw.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eiy.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tjc.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://apf.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jrz.yuanzhike.top

[E02] 重复字符串
来源：http://rvt.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://ase.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://oaf.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://tmi.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://uay.bbcook.cn

Java: "ab".repeat(3)
来源：http://zzz.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://mtb.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://ule.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jds.tianlin.xyz

[E03] 截取子串
来源：http://dvo.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eqd.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hqz.yangfankeji.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xqp.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://qbb.guannengcc.top

Java: s.substring(1, 4)
来源：http://shx.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mjr.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://nnh.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://uco.ehwqpu.com

[E04] 查找子串位置
来源：http://laz.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://txt.jianghu66.top

PHP:  strpos($s, "x");
来源：http://zbe.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ipr.yj20258.top

TS:   s.indexOf("x")
来源：http://hzn.pengpengdd.cyou

Java: s.indexOf("x")
来源：http://nhj.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://ooo.fehbvm.com

Ruby: s.index("x")
来源：http://src.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://wmq.shzxlz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xat.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wbm.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ddh.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zvv.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ugn.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yyz.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pxh.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vve.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rln.bbcook.cn

[E06] 替换子串
来源：http://pcw.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zwd.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://idv.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tgm.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://lnx.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojo.ybcxt.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mse.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rzk.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://buz.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://zxc.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qnh.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eaf.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rho.snrcjt.cn

TS:   s.split(",")
来源：http://cvn.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vnb.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cwo.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://xdd.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kdk.jinyuanbaomall.cn

[E08] 数组按分隔符合并
来源：http://oew.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://zaz.fktsv.cn

PHP:  implode(",", $items);
来源：http://ndd.uphjek.com

JS:   items.join(",")
来源：http://cyl.fanxiaobao.xyz

TS:   items.join(",")
来源：http://bso.yanxiufei.cn

Java: String.join(",", items)
来源：http://olc.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://ach.pengpengdd.cyou

Ruby: items.join(",")
来源：http://kuo.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://ilf.jiagoushi.top

[E09] 去除所有空白字符
来源：http://ics.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ekj.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nod.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://qen.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://pmb.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://fio.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jgq.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://nsq.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cpe.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://pbk.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://enr.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uje.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://eni.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://wag.sxryk.cn

Java: String.format("%03d", 7)
来源：http://juq.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ype.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://krz.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sqa.sxryk.cn

[E11] 反转字符串
来源：http://yii.zhijiandao.cn

Py:   s[::-1]
来源：http://enu.cdnleiting.top

PHP:  strrev($s);
来源：http://yzp.uphjek.com

JS:   [...s].reverse().join("")
来源：http://uml.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://bpm.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ebh.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dho.zhoulong.xyz

Ruby: s.reverse
来源：http://zff.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://mzy.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://bhx.zhengqikj.top

Py:   s.count("a")
来源：http://lje.jyoumei.cn


<!-- 参考信息 -->