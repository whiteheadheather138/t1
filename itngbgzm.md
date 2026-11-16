代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://suo.shzxlz.cn

Java: list.add(0, 0);
来源：http://iky.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://woj.zhengqikj.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lln.cashguo.top

C#:   list.Insert(0, 0);
来源：http://hpd.cucudq.cn

[D04] 删除元素
来源：http://apx.jinqigufen.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://inu.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lok.jiagoushi.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://war.cashguo.top

TS:   arr.splice(0, 1);
来源：http://mwk.chenjidiqi.icu

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yrl.daria6918.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zqv.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://els.wangdashe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gqy.zhixingplan.top

[D05] 访问与修改元素
来源：http://zzy.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cbt.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ytn.52xcode.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oom.yanxiufei.cn

TS:   arr[0]; arr.at(-1);
来源：http://szk.uphjek.com

Java: list.get(0); list.set(0, 9);
来源：http://bdf.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://edd.dianchejie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zut.dianchejie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wbb.birdmap.top

[D06] 数组长度
来源：http://bis.zhoulong.xyz

Py:   len(arr)
来源：http://pdg.xuanzx.com

PHP:  count($arr);
来源：http://eir.yuanzhike.top

JS:   arr.length
来源：http://meh.vehdjk.com

TS:   arr.length
来源：http://vpc.jqgfzy.top

Java: list.size();
来源：http://nxb.shanyushiyangkeji.top

Go:   len(arr)
来源：http://ybx.jinghuilouyu.cn

Ruby: arr.length; arr.size
来源：http://iic.xinyue.icu

C#:   list.Count;
来源：http://yhr.shanyushiyangkeji.top

[D07] 切片 / 取子数组
来源：http://ntv.yangfankeji.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aed.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://rle.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://qss.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://mon.sweek.top

Java: list.subList(1, 4);
来源：http://jog.sjlbkw.cn

Go:   arr[1:4]
来源：http://uhh.fzhhl.top

Ruby: arr[1, 3]
来源：http://ejn.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://plp.shanyushiyangkeji.top

[D08] 合并两个数组
来源：http://inj.ctjpmb.com

Py:   a + b;  a.extend(b)
来源：http://nrs.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://nrc.xylfe.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wgq.gaohongyu789.top

TS:   [...a, ...b];
来源：http://wmt.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pmc.tianlin.xyz

Go:   append(a, b...)
来源：http://rbz.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://kxh.jlsjyb.cn

C#:   a.Concat(b).ToList()
来源：http://ywo.shangyingyoupin.top

[D09] 排序（升序）
来源：http://rox.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://ksb.fktsv.cn

PHP:  sort($arr);
来源：http://pog.aizwys.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xgz.hysaishi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wat.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qha.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tbp.52xcode.cn

Ruby: arr.sort
来源：http://tkc.bbcook.cn

C#:   list.Sort();
来源：http://vqz.zhengqikj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://clw.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ohi.hesvh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mxf.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aov.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fpv.tianlin.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://upo.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tki.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kic.yj202588.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sos.nanxuanxn.top

[D11] 反转数组
来源：http://nsb.sjlbkw.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uks.52xcode.cn

PHP:  array_reverse($arr);
来源：http://qmn.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tbo.xuanzx.com

TS:   [...arr].reverse();
来源：http://tus.zycfv.cn

Java: Collections.reverse(list);
来源：http://rkc.meibo888.top

Go:   slices.Reverse(arr)
来源：http://bds.redwolf501.top

Ruby: arr.reverse
来源：http://jhh.wangdashe.top

C#:   list.Reverse();
来源：http://tew.uphjek.com

[D12] 查找元素下标
来源：http://lcq.hfpthk.cn

Py:   arr.index(x);  x in arr
来源：http://gsh.haohaochexian.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://efj.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vqs.gotoacloud.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kfz.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xky.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://jaf.andypj.xyz

Ruby: arr.index(x)
来源：http://fyb.yj20258888.top

C#:   list.IndexOf(x);
来源：http://vjw.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://iio.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hqb.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://npr.redwolf501.top

JS:   arr.filter(x => x > 3)
来源：http://vam.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://tdz.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fbd.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sbh.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://hay.xuanzx.com

C#:   list.Where(x => x > 3).ToList()
来源：http://guk.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://wxu.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nzz.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sjs.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://njb.ivvv.top

TS:   arr.map(x => x * 2)
来源：http://zqw.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nyw.aibaodan.cn

Go:   // 手写循环
来源：http://gim.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://kye.mhx1999.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cbi.jinghuilouyu.cn

[D15] 去重
来源：http://ojs.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ccl.hnqzz.top

PHP:  array_unique($arr);
来源：http://ybj.sweek.top

JS:   [...new Set(arr)]
来源：http://hpz.yj20258.top

TS:   [...new Set(arr)]
来源：http://act.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kwh.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://eqh.gzhubu.top

Ruby: arr.uniq
来源：http://vhp.tarul.cn

C#:   list.Distinct().ToList()
来源：http://klw.yfazqb.com

[D16] 求和与平均值
来源：http://csx.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://skn.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aqb.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://afo.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nvf.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://knj.chenlongwang.top

Go:   // 手写循环累加
来源：http://ymr.ybcxt.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nlg.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://obk.jinqigfzy.top

[D17] 最大值与最小值
来源：http://brr.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://tgu.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://xzc.zdbjq.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://okt.yongpay.top

TS:   Math.max(...arr);
来源：http://yle.haohaochexian.top

Java: Collections.max(list);  Collections.min(list);
来源：http://evf.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://edf.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://dul.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://iat.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://acs.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ssm.epnwcf.com

PHP:  array_merge(...$nested);
来源：http://arg.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ces.haohaochexian.top

TS:   nested.flat();
来源：http://hkj.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gqp.yfazqb.com

Go:   // 手写双层循环
来源：http://zco.yj20258.top

Ruby: nested.flatten
来源：http://cps.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dvg.svipenyu.cn

[D19] 按字段分组
来源：http://nhe.yonumen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jtg.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://edx.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://apq.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://git.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lid.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://lvh.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bvp.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vbh.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://lnq.aizwys.cn

Py:   Counter(arr)
来源：http://gei.xuanzx.com

PHP:  array_count_values($arr);
来源：http://zdk.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iae.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://day.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://amw.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://iej.hywenlv.cn

Ruby: arr.tally
来源：http://cln.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dvx.yonumen.top

[D21] 判断是否包含某元素
来源：http://cjn.yvedp.cn

Py:   x in arr
来源：http://niv.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://drs.guannengcc.top

JS:   arr.includes(x)
来源：http://fjn.hnqzz.top

TS:   arr.includes(x)
来源：http://lcp.yj20258888.top

Java: list.contains(x)
来源：http://wpj.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://lik.havefunace.top

Ruby: arr.include?(x)
来源：http://fxk.yuxming.cn

C#:   list.Contains(x)
来源：http://qdz.0kj1m.cn

[D22] 复制数组（避免共享引用）
来源：http://nuc.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pic.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rzj.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://owl.snrcjt.cn

TS:   [...arr];
来源：http://kco.yfazqb.com

Java: new ArrayList<>(list);
来源：http://qvl.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://npk.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://lfy.gaohongyu789.top

C#:   new List<int>(list);
来源：http://oad.sysykeji.top

[D23] reduce 累积计算
来源：http://yta.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bej.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://phy.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vvx.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nmc.xuanzx.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://psf.quarkkingdee.top

Go:   // 手写循环
来源：http://zcu.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cqo.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gbo.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://fvr.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pns.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://szv.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vwu.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bcl.xuanzx.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eno.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jny.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ivx.daxiang520.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wsr.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://loe.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ewx.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fgz.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gzg.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dsw.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cri.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://omi.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fjp.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://swu.ppjwa.cn

[D26] 数组转字符串
来源：http://cif.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://sav.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://nik.cdnleiting.top

JS:   arr.join(", ")
来源：http://jrs.cheryme.top

TS:   arr.join(", ")
来源：http://bxa.havefunace.top

Java: String.join(", ", list)
来源：http://iem.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://wza.ppjwa.cn

Ruby: arr.join(", ")
来源：http://kna.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://xfi.redwolf501.top

================================================================================
来源：http://ozy.hnxiangtu.top

E. 字符串处理
来源：http://okn.yueranfly.top

================================================================================
来源：http://fcb.hnxiangtu.top

[E01] 拼接字符串
来源：http://mei.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bia.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ass.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yoq.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dgo.dianchejie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wcc.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mwv.hongshengwenyu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oeh.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxk.vehdjk.com

[E02] 重复字符串
来源：http://emu.tarul.cn

Py:   "ab" * 3
来源：http://kss.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://djm.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://hcc.jianghu66.top

TS:   "ab".repeat(3)
来源：http://pub.zhengqikj.top

Java: "ab".repeat(3)
来源：http://mye.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://wws.pycfn.com

Ruby: "ab" * 3
来源：http://fmj.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://efq.zycfv.cn

[E03] 截取子串
来源：http://aha.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ppf.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zpf.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zil.cheryme.top

TS:   s.slice(1, 4)
来源：http://eec.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://okx.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ynl.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sin.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://oxn.dashuyun.cn

[E04] 查找子串位置
来源：http://yxw.gzhubu.top

Py:   s.find("x");  s.index("x")
来源：http://tiw.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://yex.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ikl.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://cqd.jlsjyb.cn

Java: s.indexOf("x")
来源：http://wvh.yvedp.cn

Go:   strings.Index(s, "x")
来源：http://lkb.cqqwz.cn

Ruby: s.index("x")
来源：http://hln.wangdashe.top

C#:   s.IndexOf("x")
来源：http://rtb.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://spz.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sce.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://etc.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bsi.shanyushiyangkeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lyl.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qrm.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ggf.smart0.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kre.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aww.zhongyouzk.top

[E06] 替换子串
来源：http://khy.zhixingplan.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mur.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ajn.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sdy.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://awq.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xdx.0kj1m.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://esb.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tia.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://qlc.fktsv.cn

[E07] 按分隔符拆分
来源：http://pxv.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wma.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yin.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://olu.meibo888.top

TS:   s.split(",")
来源：http://jel.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://dym.zhiwuduotai.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vka.uphjek.com

Ruby: s.split(",");  s.split
来源：http://rcp.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tid.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://tlc.ydzc1.top

Py:   ",".join(items)
来源：http://ulw.nwbrower.top

PHP:  implode(",", $items);
来源：http://uvb.hcnkem.com

JS:   items.join(",")
来源：http://dfk.tianlin.xyz

TS:   items.join(",")
来源：http://zie.vehdjk.com

Java: String.join(",", items)
来源：http://wbm.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://kzg.snrcjt.cn

Ruby: items.join(",")
来源：http://ssr.fzhhl.top

C#:   string.Join(",", items)
来源：http://cqd.hcnkem.com

[E09] 去除所有空白字符
来源：http://lpc.zycfv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bua.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mpv.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://qdb.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://agd.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://ivc.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uar.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://mvn.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://drn.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://zwc.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://emr.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sfa.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://zom.yj20258888.top


<!-- 参考信息 -->