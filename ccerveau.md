代发 wailian999

[D03] 在指定位置插入元素
来源：http://pji.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://idf.jianghu66.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iob.jyoumei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jty.vehdjk.com

TS:   arr.splice(0, 0, 0);
来源：http://ldu.jqgfzy.top

Java: list.add(0, 0);
来源：http://vfi.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tzs.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://api.sufxvd.cn

C#:   list.Insert(0, 0);
来源：http://bhv.shzxlz.cn

[D04] 删除元素
来源：http://pdj.shanyushiyangkeji.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hja.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xzk.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dhe.nwbrower.top

TS:   arr.splice(0, 1);
来源：http://fhy.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qon.chenjidiqi.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ttj.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://awq.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sfo.bbcook.cn

[D05] 访问与修改元素
来源：http://aov.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://obq.nanxinkj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lce.jinqigfzy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ill.ppjwa.cn

TS:   arr[0]; arr.at(-1);
来源：http://nib.epnwcf.com

Java: list.get(0); list.set(0, 9);
来源：http://tyw.jlsjyb.cn

Go:   arr[0]; arr[0] = 9
来源：http://oic.birdmap.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sgi.ywan-chungtsiang.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://njm.yj20258.top

[D06] 数组长度
来源：http://npb.hysaishi.cn

Py:   len(arr)
来源：http://wxk.sweek.top

PHP:  count($arr);
来源：http://psq.wangdashe.top

JS:   arr.length
来源：http://beo.tarul.cn

TS:   arr.length
来源：http://vsw.ctjpmb.com

Java: list.size();
来源：http://njp.hongshengwenyu.top

Go:   len(arr)
来源：http://czl.epnwcf.com

Ruby: arr.length; arr.size
来源：http://wat.daxiang520.top

C#:   list.Count;
来源：http://ghe.vehdjk.com

[D07] 切片 / 取子数组
来源：http://tcu.hnqzz.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uat.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gmg.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://zgn.xinyue.icu

TS:   arr.slice(1, 4);
来源：http://mko.hcnkem.com

Java: list.subList(1, 4);
来源：http://cfj.redwolf501.top

Go:   arr[1:4]
来源：http://doj.fktsv.cn

Ruby: arr[1, 3]
来源：http://shw.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://ica.tarul.cn

[D08] 合并两个数组
来源：http://ulb.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://utu.meibo888.top

PHP:  array_merge($a, $b);
来源：http://igw.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lvo.redwolf501.top

TS:   [...a, ...b];
来源：http://xlq.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vuv.gogol.net.cn

Go:   append(a, b...)
来源：http://mqo.andypj.xyz

Ruby: a + b;  a.concat(b)
来源：http://agx.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://yvz.zhoulong.xyz

[D09] 排序（升序）
来源：http://mzo.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://bqi.0kj1m.cn

PHP:  sort($arr);
来源：http://mvt.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uxv.yj20258.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tup.ehwqpu.com

Java: Collections.sort(list);  list.sort(null);
来源：http://izz.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qvv.bjfxy.top

Ruby: arr.sort
来源：http://qbs.yfazqb.com

C#:   list.Sort();
来源：http://sos.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qhw.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jex.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://htn.hongshengwenyu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mro.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qou.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wda.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://emj.ydjk.org.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ijv.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://elk.gogol.net.cn

[D11] 反转数组
来源：http://dsh.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://ydd.sweek.top

PHP:  array_reverse($arr);
来源：http://mti.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://eir.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://mik.ivvv.top

Java: Collections.reverse(list);
来源：http://luf.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://snj.zycfv.cn

Ruby: arr.reverse
来源：http://biu.cucudq.cn

C#:   list.Reverse();
来源：http://udd.daria6918.cn

[D12] 查找元素下标
来源：http://ujd.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://kuy.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fxc.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nbi.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hjj.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oqt.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://ons.hnqzz.top

Ruby: arr.index(x)
来源：http://xhn.tarul.cn

C#:   list.IndexOf(x);
来源：http://bhg.yj20258.top

[D13] 过滤（保留满足条件的）
来源：http://nlw.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fqt.pengpengdd.cyou

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://waj.dianchejie.cn

JS:   arr.filter(x => x > 3)
来源：http://pjm.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://xnw.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xlk.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://clk.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://xbs.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dpg.nanxuanxn.top

[D14] 映射转换（每个元素变形）
来源：http://zrg.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hms.cqqwz.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jyo.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ziy.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://slx.hywenlv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ikh.sysykeji.top

Go:   // 手写循环
来源：http://hir.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://hfv.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ffi.bbcook.cn

[D15] 去重
来源：http://wgo.hnqzz.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rug.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://rqs.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://erj.316326.xyz

TS:   [...new Set(arr)]
来源：http://vxs.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hkb.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://fyj.yfazqb.com

Ruby: arr.uniq
来源：http://vft.hesvh.cn

C#:   list.Distinct().ToList()
来源：http://ppf.ybcxt.top

[D16] 求和与平均值
来源：http://rio.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysc.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ute.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ntu.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://szn.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://amt.dianchejie.cn

Go:   // 手写循环累加
来源：http://mtt.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cco.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://jfz.xuanzx.com

[D17] 最大值与最小值
来源：http://pjf.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://wbl.hnqzz.top

PHP:  max($arr);  min($arr);
来源：http://ujr.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wmp.birdmap.top

TS:   Math.max(...arr);
来源：http://mad.shzxlz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jcr.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cys.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://wfi.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://teu.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://obv.sysykeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ogi.meibo888.top

PHP:  array_merge(...$nested);
来源：http://amz.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rsw.yj20258.top

TS:   nested.flat();
来源：http://jcu.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rrx.sxryk.cn

Go:   // 手写双层循环
来源：http://dyk.andypj.xyz

Ruby: nested.flatten
来源：http://ram.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qrl.shanyushiyangtech.top

[D19] 按字段分组
来源：http://ujy.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gke.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mmw.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hma.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://djz.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dmz.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://jji.zhiwuduotai.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dpe.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tyh.pycfn.com

[D20] 统计每个元素出现次数
来源：http://xwn.jianghu66.top

Py:   Counter(arr)
来源：http://vpz.meibo888.top

PHP:  array_count_values($arr);
来源：http://jaa.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kil.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yaz.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dfx.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://vuc.shanyushiyangtech.top

Ruby: arr.tally
来源：http://zkj.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dmm.chenjidiqi.icu

[D21] 判断是否包含某元素
来源：http://fhj.zhongyouzk.top

Py:   x in arr
来源：http://sgp.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://iun.yonumen.top

JS:   arr.includes(x)
来源：http://ilp.zdbjq.cn

TS:   arr.includes(x)
来源：http://eeg.yangfankeji.com

Java: list.contains(x)
来源：http://qmi.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://tzb.yj20258888.top

Ruby: arr.include?(x)
来源：http://zgh.yj20258888.top

C#:   list.Contains(x)
来源：http://uke.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://vcq.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vvs.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lha.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sia.hnxiangtu.top

TS:   [...arr];
来源：http://qii.bjfxy.top

Java: new ArrayList<>(list);
来源：http://knm.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://vko.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://ggs.vehdjk.com

C#:   new List<int>(list);
来源：http://lzt.jinqigufen.top

[D23] reduce 累积计算
来源：http://jth.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://url.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wvk.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bgl.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cuj.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wxh.chenlongwang.top

Go:   // 手写循环
来源：http://xwm.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://diy.xuanzx.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ypo.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://urx.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ces.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ybe.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://coz.hnqzz.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jbd.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wkh.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hqh.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wlr.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uzp.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://pud.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xru.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lso.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://upo.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vnu.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://awi.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rey.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://crz.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://stm.tian-w.cn

[D26] 数组转字符串
来源：http://mdt.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://kva.wangshuangyany.cn

PHP:  implode(", ", $arr);
来源：http://jyy.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://ddy.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://kqw.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://ovv.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://jsg.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://vwq.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://vzq.yonumen.top

================================================================================
来源：http://gxt.iojbl.cn

E. 字符串处理
来源：http://pdg.jqgufenzy.top

================================================================================
来源：http://nul.fzhhl.top

[E01] 拼接字符串
来源：http://ajw.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://whn.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mgx.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zhy.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xzw.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nfi.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oux.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gzk.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ecx.aizwys.cn

[E02] 重复字符串
来源：http://wtx.sjlbkw.cn

Py:   "ab" * 3
来源：http://efd.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://tpg.gzhubu.top

JS:   "ab".repeat(3)
来源：http://axe.xziqi.cn

TS:   "ab".repeat(3)
来源：http://dzq.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://hde.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://jmq.shzxlz.cn

Ruby: "ab" * 3
来源：http://yup.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kea.yfazqb.com

[E03] 截取子串
来源：http://www.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cie.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ybl.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gul.tarul.cn

TS:   s.slice(1, 4)
来源：http://pmb.cucudq.cn

Java: s.substring(1, 4)
来源：http://gab.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jff.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://ucd.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://akk.hywenlv.cn

[E04] 查找子串位置
来源：http://ekm.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://ykm.daxiang520.top

PHP:  strpos($s, "x");
来源：http://ibt.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://khn.hesvh.cn

TS:   s.indexOf("x")
来源：http://jir.yanxiufei.cn

Java: s.indexOf("x")
来源：http://jix.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://qsy.zhiwuduotai.top

Ruby: s.index("x")
来源：http://xux.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://igt.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kuh.hesvh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mdd.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ntk.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oxj.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://wzr.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivc.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xyf.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qfj.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fof.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://uie.aibaodan.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cxh.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://axz.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://noe.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://slw.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gxq.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://izr.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zhr.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://ren.xuanzx.com

[E07] 按分隔符拆分
来源：http://lvc.vehdjk.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ggt.fzhhl.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bzt.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gja.ctjpmb.com

TS:   s.split(",")
来源：http://ukm.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://pgl.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ndf.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://vjm.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hto.zycfv.cn

[E08] 数组按分隔符合并
来源：http://xvk.hywenlv.cn

Py:   ",".join(items)
来源：http://vie.zdbjq.cn

PHP:  implode(",", $items);
来源：http://rwp.nwbrower.top

JS:   items.join(",")
来源：http://ifi.xziqi.cn

TS:   items.join(",")
来源：http://tcd.tian-w.cn

Java: String.join(",", items)
来源：http://xyf.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://nwx.daria6918.cn

Ruby: items.join(",")
来源：http://con.fehbvm.com

C#:   string.Join(",", items)
来源：http://phn.ybcxt.top

[E09] 去除所有空白字符
来源：http://nhd.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://way.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jlq.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://zvd.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://gii.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://tvd.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jup.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://umv.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nlo.xingfuxueyuan.xyz


<!-- 参考信息 -->