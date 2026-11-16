代发 wailian999

[D03] 在指定位置插入元素
来源：http://fpj.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://nyn.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tmj.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wwp.zdbjq.cn

TS:   arr.splice(0, 0, 0);
来源：http://tug.hnqzz.top

Java: list.add(0, 0);
来源：http://zbp.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yzm.xingfuxueyuan.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fjw.birdmap.top

C#:   list.Insert(0, 0);
来源：http://taz.cashguo.top

[D04] 删除元素
来源：http://btc.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ofr.xinyue.icu

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wmy.ehwqpu.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mpk.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://vms.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tsj.snrcjt.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dnx.smart0.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qgv.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xxc.cucudq.cn

[D05] 访问与修改元素
来源：http://tnf.fzhhl.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jrb.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cmf.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tdp.jinghuilouyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://xsu.birdmap.top

Java: list.get(0); list.set(0, 9);
来源：http://feg.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://nhq.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://iko.xylfe.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qze.tianlin.xyz

[D06] 数组长度
来源：http://gob.epnwcf.com

Py:   len(arr)
来源：http://zng.c1oappe.top

PHP:  count($arr);
来源：http://kam.shuidangran.top

JS:   arr.length
来源：http://xrc.cashguo.top

TS:   arr.length
来源：http://obp.zhengqikj.top

Java: list.size();
来源：http://qbb.feifeiyinyue.top

Go:   len(arr)
来源：http://dly.yj20258.top

Ruby: arr.length; arr.size
来源：http://eef.fehbvm.com

C#:   list.Count;
来源：http://onr.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://qcl.mhx1999.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wqz.hongshengwenyu.top

PHP:  array_slice($arr, 1, 3);
来源：http://zow.pycfn.com

JS:   arr.slice(1, 4);
来源：http://ium.cashguo.top

TS:   arr.slice(1, 4);
来源：http://odo.hnqzz.top

Java: list.subList(1, 4);
来源：http://wrn.yanxiufei.cn

Go:   arr[1:4]
来源：http://hfd.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://neu.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://oye.chenlongwang.top

[D08] 合并两个数组
来源：http://qyd.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://pfi.yueranfly.top

PHP:  array_merge($a, $b);
来源：http://pmn.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jdm.daxiang520.top

TS:   [...a, ...b];
来源：http://oab.ppjwa.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hel.yj20258.top

Go:   append(a, b...)
来源：http://ugt.yj20258888.top

Ruby: a + b;  a.concat(b)
来源：http://jqg.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://sii.fzhhl.top

[D09] 排序（升序）
来源：http://trv.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://kcv.52xcode.cn

PHP:  sort($arr);
来源：http://aap.ybcxt.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://doc.pengpengdd.cyou

TS:   [...arr].sort((x, y) => x - y);
来源：http://jsb.yonumen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pky.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oos.9152youxi.cn

Ruby: arr.sort
来源：http://ttu.havefunace.top

C#:   list.Sort();
来源：http://rjs.sysykeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zeg.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qzt.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tct.hysaishi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vgv.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kor.fktsv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xfh.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fcs.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ydi.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zns.uphjek.com

[D11] 反转数组
来源：http://knj.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://zyl.52xcode.cn

PHP:  array_reverse($arr);
来源：http://cak.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://yqh.sxryk.cn

TS:   [...arr].reverse();
来源：http://jfp.gzhubu.top

Java: Collections.reverse(list);
来源：http://qzt.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://irs.ydjk.org.cn

Ruby: arr.reverse
来源：http://tuv.quarkkingdee.top

C#:   list.Reverse();
来源：http://xtm.redwolf501.top

[D12] 查找元素下标
来源：http://bed.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://fvf.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://irr.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hyq.jianghu66.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rrz.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tdw.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://lsd.sweek.top

Ruby: arr.index(x)
来源：http://etc.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://bdo.bjfxy.top

[D13] 过滤（保留满足条件的）
来源：http://ikc.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tsd.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jiv.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://tvf.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://bpu.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ahu.hammf.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pzr.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fif.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://itx.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://duu.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fjp.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hgj.jqgufenzy.top

JS:   arr.map(x => x * 2)
来源：http://xcp.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://omt.bjfxy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vwz.xuetiantiany.cn

Go:   // 手写循环
来源：http://ftf.mhx1999.top

Ruby: arr.map { |x| x * 2 }
来源：http://vze.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://wvs.cqqwz.cn

[D15] 去重
来源：http://dsh.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jzh.sxryk.cn

PHP:  array_unique($arr);
来源：http://qcg.9152youxi.cn

JS:   [...new Set(arr)]
来源：http://zri.gogol.net.cn

TS:   [...new Set(arr)]
来源：http://tid.9152youxi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baj.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://iua.zhijiandao.cn

Ruby: arr.uniq
来源：http://kan.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://siq.tanke756.top

[D16] 求和与平均值
来源：http://cgr.jqgfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oys.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dze.sysykeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sku.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://obc.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eup.cheryme.top

Go:   // 手写循环累加
来源：http://zer.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bsb.yj20258888.top

C#:   list.Sum();  list.Average()
来源：http://tkd.snrcjt.cn

[D17] 最大值与最小值
来源：http://sxg.wangshuangyany.cn

Py:   max(arr);  min(arr)
来源：http://lpq.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://ede.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qjh.gaohongyu789.top

TS:   Math.max(...arr);
来源：http://fcv.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hwe.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ynb.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://fic.yonumen.top

C#:   list.Max();  list.Min()
来源：http://mnr.ydzc1.top

[D18] 扁平化嵌套数组
来源：http://rmo.dashuyun.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hiw.havefunace.top

PHP:  array_merge(...$nested);
来源：http://hgh.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dvm.guannengcc.top

TS:   nested.flat();
来源：http://pze.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jcf.aizwys.cn

Go:   // 手写双层循环
来源：http://avm.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://udq.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://unk.fktsv.cn

[D19] 按字段分组
来源：http://afi.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rit.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://khp.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wrc.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dwx.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pzr.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://zsm.shzxlz.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fnq.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvt.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://qiw.guowangkeji.top

Py:   Counter(arr)
来源：http://owh.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://mtv.cqqwz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://drg.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxj.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hvj.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://zwz.sjlbkw.cn

Ruby: arr.tally
来源：http://nbc.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlx.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://eoj.cqqwz.cn

Py:   x in arr
来源：http://cwy.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://fvo.hnqzz.top

JS:   arr.includes(x)
来源：http://dsb.guowangkeji.top

TS:   arr.includes(x)
来源：http://kyi.hesvh.cn

Java: list.contains(x)
来源：http://fod.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://ods.sxryk.cn

Ruby: arr.include?(x)
来源：http://nnz.yj202588.top

C#:   list.Contains(x)
来源：http://pud.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://rjm.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://myu.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wqy.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://adq.hesvh.cn

TS:   [...arr];
来源：http://dre.yongpay.top

Java: new ArrayList<>(list);
来源：http://tdq.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://hmx.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://iyk.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://nno.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://euh.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eah.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vse.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ubi.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bul.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jij.nanxuanxn.top

Go:   // 手写循环
来源：http://cdr.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ofj.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ufm.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://maz.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://esw.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://koq.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jwz.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lyj.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ftc.jinghuilouyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://chj.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://omb.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rwc.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://dbb.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qlr.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://crj.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hpv.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://evo.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dgf.dianchejie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vif.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lne.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://efs.yonumen.top

[D26] 数组转字符串
来源：http://iny.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://cje.pycfn.com

PHP:  implode(", ", $arr);
来源：http://xnk.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://bnf.quarkkingdee.top

TS:   arr.join(", ")
来源：http://wbo.redwolf501.top

Java: String.join(", ", list)
来源：http://cfl.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://vey.yueranfly.top

Ruby: arr.join(", ")
来源：http://ftq.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://yxx.jlsjyb.cn

================================================================================
来源：http://cde.feifeiyinyue.top

E. 字符串处理
来源：http://slg.yj202588.top

================================================================================
来源：http://fik.nanxinkj.top

[E01] 拼接字符串
来源：http://wha.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://omi.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hlu.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jyr.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cad.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lcl.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bsx.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cnx.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qcv.uphjek.com

[E02] 重复字符串
来源：http://zjv.hnqzz.top

Py:   "ab" * 3
来源：http://wjq.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://rmk.mhx1999.top

JS:   "ab".repeat(3)
来源：http://hek.sweek.top

TS:   "ab".repeat(3)
来源：http://yeh.9152youxi.cn

Java: "ab".repeat(3)
来源：http://qpd.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://otv.birdmap.top

Ruby: "ab" * 3
来源：http://svz.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lzx.ehwqpu.com

[E03] 截取子串
来源：http://wxc.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cpt.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dbx.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bhs.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://uyu.zdqjudy.top

Java: s.substring(1, 4)
来源：http://foo.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bho.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cfo.havefunace.top

C#:   s.Substring(1, 3)
来源：http://tva.hongshengwenyu.top

[E04] 查找子串位置
来源：http://oxw.0kj1m.cn

Py:   s.find("x");  s.index("x")
来源：http://gri.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://okk.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ghj.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://vwk.nwbrower.top

Java: s.indexOf("x")
来源：http://qyo.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://wdc.guannengcc.top

Ruby: s.index("x")
来源：http://dqj.uphjek.com

C#:   s.IndexOf("x")
来源：http://exy.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nea.fanxiaobao.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ffu.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cpe.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nfd.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://jhp.uphjek.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ipg.daria6918.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://llh.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://paf.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://inv.chenzaomai.com

[E06] 替换子串
来源：http://kpq.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fxo.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://ahs.ywan-chungtsiang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://shd.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://ldt.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qbq.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wqc.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yeu.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://wjv.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://fon.9152youxi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ihl.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pqf.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yru.nwbrower.top

TS:   s.split(",")
来源：http://urx.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rxc.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fbh.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://cig.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uvr.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://wbw.birdmap.top

Py:   ",".join(items)
来源：http://jwv.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://jnu.kuanghao11.cn

JS:   items.join(",")
来源：http://lrs.hammf.cn

TS:   items.join(",")
来源：http://ykc.jqgfzy.top

Java: String.join(",", items)
来源：http://vcs.sysykeji.top

Go:   strings.Join(items, ",")
来源：http://wqs.guannengcc.top

Ruby: items.join(",")
来源：http://clp.yj20258.top

C#:   string.Join(",", items)
来源：http://hgd.hcnkem.com

[E09] 去除所有空白字符
来源：http://ljn.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ble.xinyue.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://raq.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://rft.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://bgt.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://pjo.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://hsw.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://aiv.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mdq.ehwqpu.com


<!-- 参考信息 -->