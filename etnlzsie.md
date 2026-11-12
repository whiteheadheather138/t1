代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uqf.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://wor.cheryme.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kem.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mar.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://avp.chenzaomai.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fva.ydzc1.top

[D05] 访问与修改元素
来源：http://joe.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xsi.yvedp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ypq.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uyh.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://hll.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://mzd.hysaishi.cn

Go:   arr[0]; arr[0] = 9
来源：http://mam.daxiang520.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nqb.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gju.sufxvd.cn

[D06] 数组长度
来源：http://ziz.vqdsnc.cn

Py:   len(arr)
来源：http://akk.jlsjyb.cn

PHP:  count($arr);
来源：http://ktr.cdnleiting.top

JS:   arr.length
来源：http://fph.ydjk.org.cn

TS:   arr.length
来源：http://ekx.chenjidiqi.icu

Java: list.size();
来源：http://mgl.uphjek.com

Go:   len(arr)
来源：http://atz.tanke756.top

Ruby: arr.length; arr.size
来源：http://vtj.xuetiantiany.cn

C#:   list.Count;
来源：http://jqs.nwbrower.top

[D07] 切片 / 取子数组
来源：http://ule.yongpay.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ujp.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://slv.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://itz.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://bse.chenzaomai.com

Java: list.subList(1, 4);
来源：http://lay.xziqi.cn

Go:   arr[1:4]
来源：http://hls.jqgfzy.top

Ruby: arr[1, 3]
来源：http://xna.fehbvm.com

C#:   list.GetRange(1, 3);
来源：http://xvo.zhixingplan.top

[D08] 合并两个数组
来源：http://uce.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://mdb.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://gbh.nanxuanxn.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bmn.gotoacloud.top

TS:   [...a, ...b];
来源：http://klz.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tcx.zhaomingkeji.xyz

Go:   append(a, b...)
来源：http://qjv.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://pky.jyoumei.cn

C#:   a.Concat(b).ToList()
来源：http://lus.ydjk.org.cn

[D09] 排序（升序）
来源：http://ueo.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fcd.kuanghao11.cn

PHP:  sort($arr);
来源：http://cuf.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qlo.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://cmk.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://lpt.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pcv.nanxinkj.top

Ruby: arr.sort
来源：http://hrh.gaohongyu789.top

C#:   list.Sort();
来源：http://tab.zhoulong.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://tcm.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://egs.yangfankeji.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://civ.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jty.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rcu.jlsjyb.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dbv.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://evc.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pwg.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rav.ivvv.top

[D11] 反转数组
来源：http://hky.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://ljc.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://dte.cashguo.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rtm.vqdsnc.cn

TS:   [...arr].reverse();
来源：http://hgm.xinyue.icu

Java: Collections.reverse(list);
来源：http://knm.havefunace.top

Go:   slices.Reverse(arr)
来源：http://pfl.ybcxt.top

Ruby: arr.reverse
来源：http://enj.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://yky.jlsjyb.cn

[D12] 查找元素下标
来源：http://ebd.zhiwuduotai.top

Py:   arr.index(x);  x in arr
来源：http://cwr.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hdy.xingfuxueyuan.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xei.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ehf.52xcode.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nzz.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://out.birdmap.top

Ruby: arr.index(x)
来源：http://xlw.52xcode.cn

C#:   list.IndexOf(x);
来源：http://zso.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://aqr.52xcode.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uqm.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cjd.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://vwm.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://fzf.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dzc.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nyv.hnxiangtu.top

Ruby: arr.select { |x| x > 3 }
来源：http://oul.zhengqikj.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xti.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://iiv.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xfp.xinyue.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yzx.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://ten.sweek.top

TS:   arr.map(x => x * 2)
来源：http://snz.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://khs.jinghuilouyu.cn

Go:   // 手写循环
来源：http://hxe.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://och.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://zjz.hammf.cn

[D15] 去重
来源：http://tdk.zhiwuduotai.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yly.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://zsa.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://ifr.jianghu66.top

TS:   [...new Set(arr)]
来源：http://rfc.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://esu.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://ete.zhijiandao.cn

Ruby: arr.uniq
来源：http://ery.yonumen.top

C#:   list.Distinct().ToList()
来源：http://ksx.shuidangran.top

[D16] 求和与平均值
来源：http://blx.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pnm.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lqj.jianghu66.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oek.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bqq.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kwi.cucudq.cn

Go:   // 手写循环累加
来源：http://xmd.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://unz.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://krn.havefunace.top

[D17] 最大值与最小值
来源：http://cse.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://wtn.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://iwm.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nzx.pengpengdd.cyou

TS:   Math.max(...arr);
来源：http://avg.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://who.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ahn.meibo888.top

Ruby: arr.max;  arr.min
来源：http://flq.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://ele.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://dfu.wangshuangyany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bbm.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://cdi.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vem.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://icg.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hnz.shangyingyoupin.top

Go:   // 手写双层循环
来源：http://sng.zhijiandao.cn

Ruby: nested.flatten
来源：http://vmg.tanke756.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xew.fengsongda.top

[D19] 按字段分组
来源：http://nve.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xtu.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://alp.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hel.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lvu.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qbm.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://iyf.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tfw.shanyushiyangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cqh.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://lpr.zdbjq.cn

Py:   Counter(arr)
来源：http://rqz.smart0.xyz

PHP:  array_count_values($arr);
来源：http://zrz.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxb.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://clm.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kxm.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://nny.316326.xyz

Ruby: arr.tally
来源：http://mff.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wnb.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://oed.gotoacloud.top

Py:   x in arr
来源：http://xia.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://oix.jianghu66.top

JS:   arr.includes(x)
来源：http://unu.zhijiandao.cn

TS:   arr.includes(x)
来源：http://sno.chenzaomai.com

Java: list.contains(x)
来源：http://gst.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://pis.nanxinkj.top

Ruby: arr.include?(x)
来源：http://wnp.dashuyun.cn

C#:   list.Contains(x)
来源：http://csf.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://pqd.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mgg.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xvj.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eel.hnxiangtu.top

TS:   [...arr];
来源：http://yva.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://ame.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://uvp.52xcode.cn

Ruby: arr.dup;  arr.clone
来源：http://rpo.cheryme.top

C#:   new List<int>(list);
来源：http://ozm.xylfe.cn

[D23] reduce 累积计算
来源：http://bhq.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vuk.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://too.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iry.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dfg.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eeq.xziqi.cn

Go:   // 手写循环
来源：http://ahr.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qtb.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://our.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://gnf.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ksw.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uzd.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qdv.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aol.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xks.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hce.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vae.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zgf.bbcook.cn

[D25] Set 集合去重与交并差
来源：http://wyc.yueranfly.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qie.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://evd.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ecr.jianghu66.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hln.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rsm.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://upq.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yze.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fik.hnqzz.top

[D26] 数组转字符串
来源：http://lif.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://vpe.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://unr.ydzc1.top

JS:   arr.join(", ")
来源：http://kzq.andypj.xyz

TS:   arr.join(", ")
来源：http://rgm.fehbvm.com

Java: String.join(", ", list)
来源：http://qfl.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://aya.zdbjq.cn

Ruby: arr.join(", ")
来源：http://eed.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://tod.dianchejie.cn

================================================================================
来源：http://ytc.nwbrower.top

E. 字符串处理
来源：http://uto.sweek.top

================================================================================
来源：http://xng.nwbrower.top

[E01] 拼接字符串
来源：http://wqv.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dci.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kwm.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyy.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ycy.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gfs.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qci.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bbi.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://frm.wangdashe.top

[E02] 重复字符串
来源：http://hnk.yj20258.top

Py:   "ab" * 3
来源：http://xaf.chenjidiqi.icu

PHP:  str_repeat("ab", 3);
来源：http://los.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://lcy.meibo888.top

TS:   "ab".repeat(3)
来源：http://ovs.shuidangran.top

Java: "ab".repeat(3)
来源：http://xwg.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://flz.cucudq.cn

Ruby: "ab" * 3
来源：http://gec.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dok.kuanghao11.cn

[E03] 截取子串
来源：http://otn.tianlin.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://utf.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sye.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kmq.aizwys.cn

TS:   s.slice(1, 4)
来源：http://lpp.jinqigufen.top

Java: s.substring(1, 4)
来源：http://vzc.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zzv.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://lck.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://ngi.ppjwa.cn

[E04] 查找子串位置
来源：http://umc.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://eku.bjfxy.top

PHP:  strpos($s, "x");
来源：http://fir.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ycb.mhx1999.top

TS:   s.indexOf("x")
来源：http://beh.xziqi.cn

Java: s.indexOf("x")
来源：http://zwh.chenjidiqi.icu

Go:   strings.Index(s, "x")
来源：http://mxj.hywenlv.cn

Ruby: s.index("x")
来源：http://avd.yonumen.top

C#:   s.IndexOf("x")
来源：http://tuz.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bqw.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dqd.guowangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rvi.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gdj.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tsj.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ylm.shanyushiyangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://epv.xingfuxueyuan.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://naj.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uss.chenlongwang.top

[E06] 替换子串
来源：http://yuw.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bap.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ixz.gotoacloud.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vwy.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://nqx.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ndu.yuanzhike.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ayz.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hpy.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://bwq.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://knq.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lov.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uwx.jlsjyb.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fpv.havefunace.top

TS:   s.split(",")
来源：http://wio.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jkd.cheryme.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://obj.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://rvu.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dea.shanyushiyangtech.top

[E08] 数组按分隔符合并
来源：http://gmq.kuanghao11.cn

Py:   ",".join(items)
来源：http://ves.hcnkem.com

PHP:  implode(",", $items);
来源：http://adf.bbcook.cn

JS:   items.join(",")
来源：http://btz.chenjidiqi.icu

TS:   items.join(",")
来源：http://zgc.chenlongwang.top

Java: String.join(",", items)
来源：http://lkn.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://smt.zhoulong.xyz

Ruby: items.join(",")
来源：http://pcz.sweek.top

C#:   string.Join(",", items)
来源：http://ewc.cucudq.cn

[E09] 去除所有空白字符
来源：http://fha.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fae.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wcp.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://frx.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://tqs.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://nzb.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eug.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://xjs.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oeu.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://cvs.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uje.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mrz.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://vln.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://xfu.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://gfu.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qkb.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://omt.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ktp.shuidangran.top

[E11] 反转字符串
来源：http://xpr.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://awl.zhengqikj.top

PHP:  strrev($s);
来源：http://upl.cdnleiting.top


<!-- 参考信息 -->