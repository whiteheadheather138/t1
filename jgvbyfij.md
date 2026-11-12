代发 wailian999

[D03] 在指定位置插入元素
来源：http://vco.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://pgj.svipenyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://enq.wangdashe.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pfn.hywenlv.cn

TS:   arr.splice(0, 0, 0);
来源：http://ydv.jinqigfzy.top

Java: list.add(0, 0);
来源：http://unt.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://iqr.hcnkem.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wzy.gogol.net.cn

C#:   list.Insert(0, 0);
来源：http://xff.hnqzz.top

[D04] 删除元素
来源：http://thq.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://soo.snrcjt.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pqh.chenzaomai.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qsq.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://lcn.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://teg.jinyuanbaomall.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wby.meibo888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lzz.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fhd.yvedp.cn

[D05] 访问与修改元素
来源：http://goy.shanyushiyangtech.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ksj.cheryme.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hxb.yj202588.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://buo.dashuyun.cn

TS:   arr[0]; arr.at(-1);
来源：http://kyn.aibaodan.cn

Java: list.get(0); list.set(0, 9);
来源：http://oko.xuanzx.com

Go:   arr[0]; arr[0] = 9
来源：http://izb.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oqu.haohaochexian.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dmi.wangdashe.top

[D06] 数组长度
来源：http://fii.yj202588.top

Py:   len(arr)
来源：http://tte.xylfe.cn

PHP:  count($arr);
来源：http://wss.feifeiyinyue.top

JS:   arr.length
来源：http://rlp.zdqjudy.top

TS:   arr.length
来源：http://agq.wangdashe.top

Java: list.size();
来源：http://owg.aibaodan.cn

Go:   len(arr)
来源：http://gbu.shanyushiyangkeji.top

Ruby: arr.length; arr.size
来源：http://ynd.redwolf501.top

C#:   list.Count;
来源：http://ato.316326.xyz

[D07] 切片 / 取子数组
来源：http://hgg.ybcxt.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ttz.0kj1m.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mys.tianlin.xyz

JS:   arr.slice(1, 4);
来源：http://lfx.epnwcf.com

TS:   arr.slice(1, 4);
来源：http://gvy.zhixingplan.top

Java: list.subList(1, 4);
来源：http://roz.jqgufenzy.top

Go:   arr[1:4]
来源：http://bsc.svipenyu.cn

Ruby: arr[1, 3]
来源：http://sir.jinqigfzy.top

C#:   list.GetRange(1, 3);
来源：http://snm.sufxvd.cn

[D08] 合并两个数组
来源：http://gem.pengpengdd.cyou

Py:   a + b;  a.extend(b)
来源：http://yrl.sxryk.cn

PHP:  array_merge($a, $b);
来源：http://bsc.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://yyk.jqgufenzy.top

TS:   [...a, ...b];
来源：http://kfo.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rqo.vehdjk.com

Go:   append(a, b...)
来源：http://ytr.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://idk.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://kjh.wangdashe.top

[D09] 排序（升序）
来源：http://jwh.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://efj.yangfankeji.com

PHP:  sort($arr);
来源：http://vhy.vqdsnc.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qes.zhoulong.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://syq.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qeo.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rlr.0kj1m.cn

Ruby: arr.sort
来源：http://hxt.andypj.xyz

C#:   list.Sort();
来源：http://swq.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pnv.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dvn.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ybk.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgx.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mgd.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xim.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://quw.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nvl.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gsa.52xcode.cn

[D11] 反转数组
来源：http://hga.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://lwc.52xcode.cn

PHP:  array_reverse($arr);
来源：http://ovz.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cro.aibaodan.cn

TS:   [...arr].reverse();
来源：http://vjz.sysykeji.top

Java: Collections.reverse(list);
来源：http://mwk.tanke756.top

Go:   slices.Reverse(arr)
来源：http://qql.yj202588.top

Ruby: arr.reverse
来源：http://spw.daria6918.cn

C#:   list.Reverse();
来源：http://crb.hesvh.cn

[D12] 查找元素下标
来源：http://zek.zdqjudy.top

Py:   arr.index(x);  x in arr
来源：http://cdn.316326.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gqu.pengpengdd.cyou

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nqm.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ozk.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uld.shanyushiyangtech.top

Go:   slices.Index(arr, x)
来源：http://eps.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://fbn.iojbl.cn

C#:   list.IndexOf(x);
来源：http://ctb.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://snq.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yeh.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qhb.zhiwuduotai.top

JS:   arr.filter(x => x > 3)
来源：http://mnk.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://htp.hnqzz.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gdt.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ecd.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://lvv.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qvb.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://hye.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vfr.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qou.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://ybq.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://uvt.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://siv.xuanzx.com

Go:   // 手写循环
来源：http://whd.zhiwuduotai.top

Ruby: arr.map { |x| x * 2 }
来源：http://rik.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pif.snrcjt.cn

[D15] 去重
来源：http://bdr.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://udl.smart0.xyz

PHP:  array_unique($arr);
来源：http://egq.cheryme.top

JS:   [...new Set(arr)]
来源：http://nqr.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://xsh.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yvl.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gnc.zhixingplan.top

Ruby: arr.uniq
来源：http://odk.meibo888.top

C#:   list.Distinct().ToList()
来源：http://tan.hfpthk.cn

[D16] 求和与平均值
来源：http://rsc.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eih.zycfv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ldu.mhx1999.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uex.yueranfly.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uaa.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fhp.zhixingplan.top

Go:   // 手写循环累加
来源：http://esh.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vpt.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://hte.hammf.cn

[D17] 最大值与最小值
来源：http://mgi.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://zau.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://raa.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://trb.vqdsnc.cn

TS:   Math.max(...arr);
来源：http://ymr.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nre.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vsk.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://rvm.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://lhc.yj20258.top

[D18] 扁平化嵌套数组
来源：http://oeo.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eui.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://vzy.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mei.xingfuxueyuan.xyz

TS:   nested.flat();
来源：http://syk.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ofz.cdnleiting.top

Go:   // 手写双层循环
来源：http://fbc.yongpay.top

Ruby: nested.flatten
来源：http://dky.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vdr.tianlin.xyz

[D19] 按字段分组
来源：http://srr.daria6918.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fry.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hdo.dianchejie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://myz.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ylp.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tsl.jianghu66.top

Go:   // 手写 map[string][]T
来源：http://eru.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://psy.hcnkem.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uyi.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://qil.52xcode.cn

Py:   Counter(arr)
来源：http://wvk.zycfv.cn

PHP:  array_count_values($arr);
来源：http://kms.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hai.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jix.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nyd.aizwys.cn

Go:   // 手写 map[T]int
来源：http://ocg.smart0.xyz

Ruby: arr.tally
来源：http://gom.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ciy.shanyushiyangkeji.top

[D21] 判断是否包含某元素
来源：http://kpu.fktsv.cn

Py:   x in arr
来源：http://zuh.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://ztt.xinyue.icu

JS:   arr.includes(x)
来源：http://mwe.fengsongda.top

TS:   arr.includes(x)
来源：http://rfd.redwolf501.top

Java: list.contains(x)
来源：http://ylg.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://trb.nwbrower.top

Ruby: arr.include?(x)
来源：http://cyu.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://pqk.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://rjd.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xmk.fanxiaobao.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ovf.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uux.snrcjt.cn

TS:   [...arr];
来源：http://psh.c1oappe.top

Java: new ArrayList<>(list);
来源：http://yrb.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xpt.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://hlw.yanxiufei.cn

C#:   new List<int>(list);
来源：http://lii.cashguo.top

[D23] reduce 累积计算
来源：http://bqt.daxiang520.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oou.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bll.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lql.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bbp.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://eqc.yongpay.top

Go:   // 手写循环
来源：http://ihq.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xfh.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://anr.sysykeji.top

[D24] 字典 / Map 基本操作
来源：http://cgl.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qyt.uphjek.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qsv.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wem.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ple.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eoo.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lfm.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twf.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://drw.sysykeji.top

[D25] Set 集合去重与交并差
来源：http://lgj.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cly.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mtm.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wnt.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fic.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sln.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pii.hammf.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pkn.shzxlz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eml.uphjek.com

[D26] 数组转字符串
来源：http://whn.hongshengwenyu.top

Py:   ", ".join(map(str, arr))
来源：http://qbv.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://zlo.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://tix.316326.xyz

TS:   arr.join(", ")
来源：http://iuj.hcnkem.com

Java: String.join(", ", list)
来源：http://kkr.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://azg.hammf.cn

Ruby: arr.join(", ")
来源：http://kof.hnqzz.top

C#:   string.Join(", ", list)
来源：http://uuk.hywenlv.cn

================================================================================
来源：http://wxz.sweek.top

E. 字符串处理
来源：http://szl.ydzc1.top

================================================================================
来源：http://rrb.hfpthk.cn

[E01] 拼接字符串
来源：http://lfo.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pdm.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hbo.xingfuxueyuan.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eww.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yva.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hpd.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qgc.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hip.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://myk.zhijiandao.cn

[E02] 重复字符串
来源：http://vud.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://qre.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://rbi.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://mmn.xinyue.icu

TS:   "ab".repeat(3)
来源：http://qhr.hesvh.cn

Java: "ab".repeat(3)
来源：http://ijt.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://liz.hysaishi.cn

Ruby: "ab" * 3
来源：http://ysp.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hia.tianlin.xyz

[E03] 截取子串
来源：http://zjz.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zes.ybcxt.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tev.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yqa.birdmap.top

TS:   s.slice(1, 4)
来源：http://ian.hfpthk.cn

Java: s.substring(1, 4)
来源：http://fox.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://crt.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://dag.tanke756.top

C#:   s.Substring(1, 3)
来源：http://wwi.nwbrower.top

[E04] 查找子串位置
来源：http://chy.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://ipb.cucudq.cn

PHP:  strpos($s, "x");
来源：http://qpq.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://loo.gogol.net.cn

TS:   s.indexOf("x")
来源：http://wey.jyoumei.cn

Java: s.indexOf("x")
来源：http://oil.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://zqs.epnwcf.com

Ruby: s.index("x")
来源：http://ais.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://ptk.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://rpr.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ant.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gyc.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivq.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zbz.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mro.hammf.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bby.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://amw.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rwc.xylfe.cn

[E06] 替换子串
来源：http://hol.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pug.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://hfx.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ilx.shzxlz.cn

TS:   s.replaceAll("a", "b")
来源：http://yoj.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://awk.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sna.dashuyun.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jdd.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://evo.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://bpn.yj202588.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sfn.hysaishi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xka.yueranfly.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zzf.fzhhl.top

TS:   s.split(",")
来源：http://rqv.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://iqe.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zbg.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://sqc.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rzr.daria6918.cn

[E08] 数组按分隔符合并
来源：http://vab.shzxlz.cn

Py:   ",".join(items)
来源：http://okb.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://uye.yvedp.cn

JS:   items.join(",")
来源：http://aiv.nanxinkj.top

TS:   items.join(",")
来源：http://asg.nanxuanxn.top

Java: String.join(",", items)
来源：http://rdt.c1oappe.top

Go:   strings.Join(items, ",")
来源：http://tlb.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://kyh.bjfxy.top

C#:   string.Join(",", items)
来源：http://ldh.sweek.top

[E09] 去除所有空白字符
来源：http://eyn.bjfxy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pnd.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rcj.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://jwh.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://ung.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://vgm.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wyv.vqdsnc.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ksv.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ara.fengsongda.top


<!-- 参考信息 -->