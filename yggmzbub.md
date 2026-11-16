代发 wailian999

[D03] 在指定位置插入元素
来源：http://yqc.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://eej.tarul.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bsp.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://snn.sweek.top

TS:   arr.splice(0, 0, 0);
来源：http://hvy.c1oappe.top

Java: list.add(0, 0);
来源：http://mmw.cqqwz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kfm.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wui.jinqigfzy.top

C#:   list.Insert(0, 0);
来源：http://xtp.xinyue.icu

[D04] 删除元素
来源：http://qvf.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xlv.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ina.sysykeji.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jan.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://jxd.yj202588.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bak.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jue.wangdashe.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iwq.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dea.hesvh.cn

[D05] 访问与修改元素
来源：http://uzc.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wco.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mje.epnwcf.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nsg.yvedp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ojv.fktsv.cn

Java: list.get(0); list.set(0, 9);
来源：http://tdp.ydjk.org.cn

Go:   arr[0]; arr[0] = 9
来源：http://uyr.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tok.daxiang520.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cyw.meibo888.top

[D06] 数组长度
来源：http://kmp.tarul.cn

Py:   len(arr)
来源：http://yeq.sweek.top

PHP:  count($arr);
来源：http://yvp.meibo888.top

JS:   arr.length
来源：http://rwy.tanke756.top

TS:   arr.length
来源：http://ftq.guowangkeji.top

Java: list.size();
来源：http://obv.havefunace.top

Go:   len(arr)
来源：http://orc.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://sbu.ywan-chungtsiang.top

C#:   list.Count;
来源：http://bvd.fzhhl.top

[D07] 切片 / 取子数组
来源：http://dap.shanyushiyangtech.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qbd.zhengqikj.top

PHP:  array_slice($arr, 1, 3);
来源：http://opm.zhengqikj.top

JS:   arr.slice(1, 4);
来源：http://pku.sysykeji.top

TS:   arr.slice(1, 4);
来源：http://eit.shzxlz.cn

Java: list.subList(1, 4);
来源：http://smd.gzhubu.top

Go:   arr[1:4]
来源：http://phc.bjfxy.top

Ruby: arr[1, 3]
来源：http://cyx.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://eku.snrcjt.cn

[D08] 合并两个数组
来源：http://jub.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://epg.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://rtv.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://igz.jianghu66.top

TS:   [...a, ...b];
来源：http://vba.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mxg.tarul.cn

Go:   append(a, b...)
来源：http://vqd.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://xjz.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://eko.yvedp.cn

[D09] 排序（升序）
来源：http://rdf.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://yya.redwolf501.top

PHP:  sort($arr);
来源：http://rwu.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mkx.hammf.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://uhj.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lbn.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mrj.epnwcf.com

Ruby: arr.sort
来源：http://ifz.ehwqpu.com

C#:   list.Sort();
来源：http://jbq.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aoc.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xda.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xkq.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zil.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://heo.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bmj.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ion.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://log.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cbf.yfazqb.com

[D11] 反转数组
来源：http://bkq.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qcx.wangshuangyany.cn

PHP:  array_reverse($arr);
来源：http://nbe.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pjm.yuxming.cn

TS:   [...arr].reverse();
来源：http://qlu.meibo888.top

Java: Collections.reverse(list);
来源：http://vkq.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://bou.ydjk.org.cn

Ruby: arr.reverse
来源：http://xxw.tanke756.top

C#:   list.Reverse();
来源：http://lzd.dianchejie.cn

[D12] 查找元素下标
来源：http://wdm.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://iay.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://azt.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://plz.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dxy.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gng.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://hpw.snrcjt.cn

Ruby: arr.index(x)
来源：http://fdk.havefunace.top

C#:   list.IndexOf(x);
来源：http://ltr.tarul.cn

[D13] 过滤（保留满足条件的）
来源：http://ssy.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://avg.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mkw.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://nuo.wangshuangyany.cn

TS:   arr.filter(x => x > 3)
来源：http://dig.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dkj.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cdd.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://fns.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tpr.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://rao.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wyh.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jrp.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://zby.tarul.cn

TS:   arr.map(x => x * 2)
来源：http://wks.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mql.sxryk.cn

Go:   // 手写循环
来源：http://nyu.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yxh.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qzi.birdmap.top

[D15] 去重
来源：http://xnf.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://emq.sweek.top

PHP:  array_unique($arr);
来源：http://pnj.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://tpt.gaohongyu789.top

TS:   [...new Set(arr)]
来源：http://lyp.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nqj.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wgr.cucudq.cn

Ruby: arr.uniq
来源：http://gkp.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://bee.ybcxt.top

[D16] 求和与平均值
来源：http://ogn.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wii.zdbjq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ksz.fktsv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzc.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yeh.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://afo.kuanghao11.cn

Go:   // 手写循环累加
来源：http://zey.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bmw.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://omu.ehwqpu.com

[D17] 最大值与最小值
来源：http://hiw.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://pnn.tianlin.xyz

PHP:  max($arr);  min($arr);
来源：http://qtt.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tgv.jinqigufen.top

TS:   Math.max(...arr);
来源：http://dub.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gex.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jkf.316326.xyz

Ruby: arr.max;  arr.min
来源：http://oyn.cheryme.top

C#:   list.Max();  list.Min()
来源：http://leo.cqqwz.cn

[D18] 扁平化嵌套数组
来源：http://nzw.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dpd.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://jib.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uwu.zhixingplan.top

TS:   nested.flat();
来源：http://qhr.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dwo.yonumen.top

Go:   // 手写双层循环
来源：http://jva.hnqzz.top

Ruby: nested.flatten
来源：http://wdy.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://zxu.quarkkingdee.top

[D19] 按字段分组
来源：http://tel.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vih.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fqs.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://drm.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://pxp.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cig.yj20258.top

Go:   // 手写 map[string][]T
来源：http://rzt.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://xgz.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ncx.jinqigfzy.top

[D20] 统计每个元素出现次数
来源：http://zwc.jyoumei.cn

Py:   Counter(arr)
来源：http://avy.sjlbkw.cn

PHP:  array_count_values($arr);
来源：http://age.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jim.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aqt.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ltm.fehbvm.com

Go:   // 手写 map[T]int
来源：http://faa.kuanghao11.cn

Ruby: arr.tally
来源：http://wzd.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://woy.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://nuo.nwbrower.top

Py:   x in arr
来源：http://llf.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://fhl.zycfv.cn

JS:   arr.includes(x)
来源：http://hja.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://yqc.ybcxt.top

Java: list.contains(x)
来源：http://seu.wangshuangyany.cn

Go:   slices.Contains(arr, x)
来源：http://pwf.yangfankeji.com

Ruby: arr.include?(x)
来源：http://ujh.yonumen.top

C#:   list.Contains(x)
来源：http://hkr.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://rtf.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ejp.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bkj.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ujb.feifeiyinyue.top

TS:   [...arr];
来源：http://dps.hcnkem.com

Java: new ArrayList<>(list);
来源：http://zwv.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://opv.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://ifl.chenzaomai.com

C#:   new List<int>(list);
来源：http://tdd.gogol.net.cn

[D23] reduce 累积计算
来源：http://sfc.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fnh.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mci.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhn.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rzz.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wky.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://uqe.nanxuanxn.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://guo.aibaodan.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oxe.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://wpe.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hse.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xbv.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nlq.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kvr.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dru.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qfp.nanxinkj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://haf.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://usd.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://uyu.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lnf.hesvh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gxw.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zku.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ihg.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://emo.chenjidiqi.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ctw.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jpi.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xha.gogol.net.cn

[D26] 数组转字符串
来源：http://cyf.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://vsd.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://jqy.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://hto.sysykeji.top

TS:   arr.join(", ")
来源：http://ieg.sxryk.cn

Java: String.join(", ", list)
来源：http://btx.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://olu.cdnleiting.top

Ruby: arr.join(", ")
来源：http://fry.hcnkem.com

C#:   string.Join(", ", list)
来源：http://wbs.havefunace.top

================================================================================
来源：http://lvk.c1oappe.top

E. 字符串处理
来源：http://hyz.shangyingyoupin.top

================================================================================
来源：http://zri.fktsv.cn

[E01] 拼接字符串
来源：http://cfw.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xac.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gzu.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jde.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dno.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfm.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fgx.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bli.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iyl.daria6918.cn

[E02] 重复字符串
来源：http://awc.jiagoushi.top

Py:   "ab" * 3
来源：http://clx.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://ezu.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://rbl.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://blg.aizwys.cn

Java: "ab".repeat(3)
来源：http://zcj.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://cmu.jianghu66.top

Ruby: "ab" * 3
来源：http://idr.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kfh.jiagoushi.top

[E03] 截取子串
来源：http://cht.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gwi.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ugq.pycfn.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yqb.havefunace.top

TS:   s.slice(1, 4)
来源：http://fnz.pycfn.com

Java: s.substring(1, 4)
来源：http://tlt.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hey.zhengqikj.top

Ruby: s[1, 3];  s[1..3]
来源：http://vww.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://apg.cqqwz.cn

[E04] 查找子串位置
来源：http://mtr.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://rzz.yangfankeji.com

PHP:  strpos($s, "x");
来源：http://cpe.smart0.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://evz.ivvv.top

TS:   s.indexOf("x")
来源：http://lcj.mhx1999.top

Java: s.indexOf("x")
来源：http://fhp.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://jhx.snrcjt.cn

Ruby: s.index("x")
来源：http://ckj.yonumen.top

C#:   s.IndexOf("x")
来源：http://dot.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://pus.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ntr.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bpt.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ieu.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nvp.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cpg.hywenlv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uzd.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lqo.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://usm.0kj1m.cn

[E06] 替换子串
来源：http://gxp.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://spg.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://bff.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yre.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://udw.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfm.xuanzx.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hfe.jiagoushi.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://alz.birdmap.top

C#:   s.Replace("a", "b")
来源：http://ykb.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://hcn.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yjp.bjfxy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cfm.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hml.birdmap.top

TS:   s.split(",")
来源：http://onw.yuxming.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wpd.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://daq.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://vef.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ago.ybcxt.top

[E08] 数组按分隔符合并
来源：http://hyi.dianchejie.cn

Py:   ",".join(items)
来源：http://ppf.xziqi.cn

PHP:  implode(",", $items);
来源：http://jqq.jinqigfzy.top

JS:   items.join(",")
来源：http://vrm.jianghu66.top

TS:   items.join(",")
来源：http://tmc.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://ntd.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://sog.andypj.xyz

Ruby: items.join(",")
来源：http://vnh.svipenyu.cn

C#:   string.Join(",", items)
来源：http://whi.sweek.top

[E09] 去除所有空白字符
来源：http://mxb.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fcx.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nbs.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://mao.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ppe.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://vyu.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bpi.mhx1999.top

Ruby: s.gsub(/\s+/, "")
来源：http://qod.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rli.hnxiangtu.top


<!-- 参考信息 -->