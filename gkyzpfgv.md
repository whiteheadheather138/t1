代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rmf.gaohongyu789.top

TS:   arr.splice(0, 1);
来源：http://twx.snrcjt.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ohf.shuidangran.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yyo.cqqwz.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bfc.wangshuangyany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kvk.daria6918.cn

[D05] 访问与修改元素
来源：http://ovd.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://avd.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yze.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mzj.hysaishi.cn

TS:   arr[0]; arr.at(-1);
来源：http://ktz.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://twb.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://dar.shuidangran.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ohx.hongshengwenyu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dye.dianchejie.cn

[D06] 数组长度
来源：http://duq.chenzaomai.com

Py:   len(arr)
来源：http://etf.c1oappe.top

PHP:  count($arr);
来源：http://dtr.nwbrower.top

JS:   arr.length
来源：http://keb.daria6918.cn

TS:   arr.length
来源：http://fyn.yvedp.cn

Java: list.size();
来源：http://gim.yj20258.top

Go:   len(arr)
来源：http://pmx.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://qlz.jinghuilouyu.cn

C#:   list.Count;
来源：http://jbu.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://vso.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jju.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://dpj.hammf.cn

JS:   arr.slice(1, 4);
来源：http://yan.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://ijy.aibaodan.cn

Java: list.subList(1, 4);
来源：http://egl.epnwcf.com

Go:   arr[1:4]
来源：http://fzt.xuetiantiany.cn

Ruby: arr[1, 3]
来源：http://fwv.feifeiyinyue.top

C#:   list.GetRange(1, 3);
来源：http://xgg.hfpthk.cn

[D08] 合并两个数组
来源：http://ghd.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://awt.316326.xyz

PHP:  array_merge($a, $b);
来源：http://eqb.birdmap.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xqk.fengsongda.top

TS:   [...a, ...b];
来源：http://svg.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qts.hcnkem.com

Go:   append(a, b...)
来源：http://ldz.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://ufs.hongshengwenyu.top

C#:   a.Concat(b).ToList()
来源：http://yzd.meibo888.top

[D09] 排序（升序）
来源：http://prs.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://owd.daxiang520.top

PHP:  sort($arr);
来源：http://usi.52xcode.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zni.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hzz.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lxo.yanxiufei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wfh.sweek.top

Ruby: arr.sort
来源：http://akg.ppjwa.cn

C#:   list.Sort();
来源：http://phs.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ysq.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lab.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rji.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eul.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxm.shuidangran.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://roa.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://goo.fengsongda.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zqm.aizwys.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ptd.redwolf501.top

[D11] 反转数组
来源：http://xbp.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://kgb.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://shy.yuxming.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jrd.havefunace.top

TS:   [...arr].reverse();
来源：http://vnb.svipenyu.cn

Java: Collections.reverse(list);
来源：http://nzp.yongpay.top

Go:   slices.Reverse(arr)
来源：http://yzf.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://sdw.sufxvd.cn

C#:   list.Reverse();
来源：http://rdu.cheryme.top

[D12] 查找元素下标
来源：http://muy.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://yig.hongshengwenyu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://edf.bjfxy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://acd.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tag.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hfs.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://cpj.tanke756.top

Ruby: arr.index(x)
来源：http://akc.zhongyouzk.top

C#:   list.IndexOf(x);
来源：http://olo.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://wkd.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://khe.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wgf.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://khe.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://cio.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vez.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sme.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://lqm.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tou.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://pxw.hcnkem.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aft.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rix.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://ctz.zhengqikj.top

TS:   arr.map(x => x * 2)
来源：http://rvc.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tij.52xcode.cn

Go:   // 手写循环
来源：http://yko.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://inh.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://thk.xingfuxueyuan.xyz

[D15] 去重
来源：http://oph.cqqwz.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cee.gotoacloud.top

PHP:  array_unique($arr);
来源：http://ghj.hcnkem.com

JS:   [...new Set(arr)]
来源：http://vcw.xziqi.cn

TS:   [...new Set(arr)]
来源：http://hgc.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vrt.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ocf.zhaomingkeji.xyz

Ruby: arr.uniq
来源：http://jmv.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://wvv.jiagoushi.top

[D16] 求和与平均值
来源：http://rpp.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qzk.sjlbkw.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nzy.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zkn.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqz.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://phg.hesvh.cn

Go:   // 手写循环累加
来源：http://zyw.cheryme.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bnk.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://qcm.sjlbkw.cn

[D17] 最大值与最小值
来源：http://mgd.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://sqj.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://rtx.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uot.jinqigufen.top

TS:   Math.max(...arr);
来源：http://hfw.vqdsnc.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xms.yonumen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ukn.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://enx.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://gul.hammf.cn

[D18] 扁平化嵌套数组
来源：http://wcc.hesvh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ucm.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://ngl.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jtd.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://qmp.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kqb.yanxiufei.cn

Go:   // 手写双层循环
来源：http://vuk.hammf.cn

Ruby: nested.flatten
来源：http://hml.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://sub.guowangkeji.top

[D19] 按字段分组
来源：http://kaj.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://viw.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ztg.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yuk.cdnleiting.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sbx.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://orz.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://tyz.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://yyf.nanxinkj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dxu.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://roy.gaohongyu789.top

Py:   Counter(arr)
来源：http://akc.316326.xyz

PHP:  array_count_values($arr);
来源：http://kwx.c1oappe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvk.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fjd.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bng.xuanzx.com

Go:   // 手写 map[T]int
来源：http://inu.sxryk.cn

Ruby: arr.tally
来源：http://bxl.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://udv.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://rhj.hesvh.cn

Py:   x in arr
来源：http://ckt.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://kge.sjlbkw.cn

JS:   arr.includes(x)
来源：http://mvm.tanke756.top

TS:   arr.includes(x)
来源：http://tke.c1oappe.top

Java: list.contains(x)
来源：http://vpw.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://oyp.nwbrower.top

Ruby: arr.include?(x)
来源：http://gfw.jianghu66.top

C#:   list.Contains(x)
来源：http://dgt.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://gja.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uwx.guannengcc.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gnw.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hdy.bbcook.cn

TS:   [...arr];
来源：http://rvg.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://gew.shangyingyoupin.top

Go:   copied := append([]int(nil), arr...)
来源：http://bjt.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://sip.ydzc1.top

C#:   new List<int>(list);
来源：http://exr.ydzc1.top

[D23] reduce 累积计算
来源：http://xzj.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fra.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wnh.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bwq.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cde.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vfc.svipenyu.cn

Go:   // 手写循环
来源：http://fea.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lbx.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qti.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://hfk.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qur.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wxf.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wwo.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eut.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://znf.xingfuxueyuan.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bhu.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yns.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ifd.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://lhy.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://udl.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fkc.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://heg.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pfv.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bnh.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pfj.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pfz.bbcook.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gty.yanxiufei.cn

[D26] 数组转字符串
来源：http://rkc.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://usi.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://qbz.sxryk.cn

JS:   arr.join(", ")
来源：http://khm.tarul.cn

TS:   arr.join(", ")
来源：http://eaj.316326.xyz

Java: String.join(", ", list)
来源：http://zro.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://miu.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://suo.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://ysw.jqgufenzy.top

================================================================================
来源：http://cja.epnwcf.com

E. 字符串处理
来源：http://xug.cashguo.top

================================================================================
来源：http://ovs.dashuyun.cn

[E01] 拼接字符串
来源：http://mux.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pbx.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bty.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nhf.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://stg.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://poo.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ump.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uxa.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://glm.daxiang520.top

[E02] 重复字符串
来源：http://jal.yuxming.cn

Py:   "ab" * 3
来源：http://mxo.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://efx.yueranfly.top

JS:   "ab".repeat(3)
来源：http://xel.bbcook.cn

TS:   "ab".repeat(3)
来源：http://edy.iojbl.cn

Java: "ab".repeat(3)
来源：http://mwu.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://ubb.ehwqpu.com

Ruby: "ab" * 3
来源：http://egb.shuidangran.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bqz.tanke756.top

[E03] 截取子串
来源：http://rae.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ons.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ozd.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yub.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://gay.nwbrower.top

Java: s.substring(1, 4)
来源：http://wud.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xhv.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dxy.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://gol.shangyingyoupin.top

[E04] 查找子串位置
来源：http://ouo.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://ebz.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://epq.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zbf.zhengqikj.top

TS:   s.indexOf("x")
来源：http://vnf.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://ees.tanke756.top

Go:   strings.Index(s, "x")
来源：http://twp.nwbrower.top

Ruby: s.index("x")
来源：http://kys.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://dmf.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mij.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ket.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tqd.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cjj.chenjidiqi.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://bar.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cok.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gws.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qze.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aoh.jqgufenzy.top

[E06] 替换子串
来源：http://rdd.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wgn.xingfuxueyuan.xyz

PHP:  str_replace("a", "b", $s);
来源：http://fwu.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bwy.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://ttn.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxj.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://otn.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ndc.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://wvg.cucudq.cn

[E07] 按分隔符拆分
来源：http://swz.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xeh.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kjs.jinqigufen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://onl.jinyuanbaomall.cn

TS:   s.split(",")
来源：http://xsf.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://jwo.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xah.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://uad.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xbx.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://jnr.jinqigfzy.top

Py:   ",".join(items)
来源：http://qyg.jinqigufen.top

PHP:  implode(",", $items);
来源：http://ztd.bbcook.cn

JS:   items.join(",")
来源：http://odn.hcnkem.com

TS:   items.join(",")
来源：http://elb.zhiwuduotai.top

Java: String.join(",", items)
来源：http://goo.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://ytz.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://eob.daria6918.cn

C#:   string.Join(",", items)
来源：http://tmt.ivvv.top

[E09] 去除所有空白字符
来源：http://ypw.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lni.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ewi.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://bfu.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://ohf.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://hem.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cmw.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://dwx.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qgb.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://cjm.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://buy.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://twk.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://xtn.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://lda.jianghu66.top

Java: String.format("%03d", 7)
来源：http://pfp.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://dyi.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cai.sweek.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhe.c1oappe.top

[E11] 反转字符串
来源：http://drk.c1oappe.top

Py:   s[::-1]
来源：http://svj.xuanzx.com

PHP:  strrev($s);
来源：http://ufg.pycfn.com


<!-- 参考信息 -->