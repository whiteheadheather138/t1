代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cme.tarul.cn

TS:   arr.splice(0, 1);
来源：http://gtb.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://uzs.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jnd.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nts.zhixingplan.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kco.yonumen.top

[D05] 访问与修改元素
来源：http://xsu.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kxr.vehdjk.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yej.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xuo.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://tfk.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://nph.ivvv.top

Go:   arr[0]; arr[0] = 9
来源：http://hii.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xlg.nanxinkj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ogm.shanyushiyangtech.top

[D06] 数组长度
来源：http://usb.bjfxy.top

Py:   len(arr)
来源：http://dqt.hammf.cn

PHP:  count($arr);
来源：http://ffa.c1oappe.top

JS:   arr.length
来源：http://tvf.yanxiufei.cn

TS:   arr.length
来源：http://wwz.fktsv.cn

Java: list.size();
来源：http://kgn.cdnleiting.top

Go:   len(arr)
来源：http://tra.chenlongwang.top

Ruby: arr.length; arr.size
来源：http://urf.yongpay.top

C#:   list.Count;
来源：http://oub.hesvh.cn

[D07] 切片 / 取子数组
来源：http://iac.vqdsnc.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dhy.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://flf.yj20258.top

JS:   arr.slice(1, 4);
来源：http://akz.meibo888.top

TS:   arr.slice(1, 4);
来源：http://lty.xuanzx.com

Java: list.subList(1, 4);
来源：http://xrp.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://yoq.hywenlv.cn

Ruby: arr[1, 3]
来源：http://bas.hcnkem.com

C#:   list.GetRange(1, 3);
来源：http://rtt.tian-w.cn

[D08] 合并两个数组
来源：http://ncx.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://kre.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://qvd.chenjidiqi.icu

JS:   [...a, ...b];  a.concat(b);
来源：http://bnt.cdnleiting.top

TS:   [...a, ...b];
来源：http://arn.zhengqikj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gde.zycfv.cn

Go:   append(a, b...)
来源：http://gsq.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://hoo.xuanzx.com

C#:   a.Concat(b).ToList()
来源：http://wfw.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://avi.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://ruz.bjfxy.top

PHP:  sort($arr);
来源：http://zdm.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rra.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mvm.shanyushiyangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bgs.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yeb.havefunace.top

Ruby: arr.sort
来源：http://lor.fanxiaobao.xyz

C#:   list.Sort();
来源：http://xvr.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://nyb.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://trm.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://duo.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uqf.haohaochexian.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pvb.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xwt.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nxg.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vcg.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xrz.chenjidiqi.icu

[D11] 反转数组
来源：http://hne.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://ykf.daria6918.cn

PHP:  array_reverse($arr);
来源：http://zzu.sufxvd.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nip.cheryme.top

TS:   [...arr].reverse();
来源：http://trv.shanyushiyangtech.top

Java: Collections.reverse(list);
来源：http://tfk.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://sdf.jiagoushi.top

Ruby: arr.reverse
来源：http://beu.chenzaomai.com

C#:   list.Reverse();
来源：http://tzd.yueranfly.top

[D12] 查找元素下标
来源：http://xjw.yueranfly.top

Py:   arr.index(x);  x in arr
来源：http://yqx.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kay.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eyg.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yrk.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://igv.ywan-chungtsiang.top

Go:   slices.Index(arr, x)
来源：http://zxg.nwbrower.top

Ruby: arr.index(x)
来源：http://zxn.yuxming.cn

C#:   list.IndexOf(x);
来源：http://nxx.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://sdw.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mwq.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jpv.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://qbn.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://oxi.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://akj.aizwys.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jjc.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://wut.iojbl.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kvd.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://gaz.hnxiangtu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nuw.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dwu.aibaodan.cn

JS:   arr.map(x => x * 2)
来源：http://uvg.smart0.xyz

TS:   arr.map(x => x * 2)
来源：http://ssb.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zmh.zhijiandao.cn

Go:   // 手写循环
来源：http://irt.fzhhl.top

Ruby: arr.map { |x| x * 2 }
来源：http://kun.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://udo.redwolf501.top

[D15] 去重
来源：http://dny.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xrt.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://dxy.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://ynz.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://ihx.sjlbkw.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tdl.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fsc.zhijiandao.cn

Ruby: arr.uniq
来源：http://xlh.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://qqd.chenzaomai.com

[D16] 求和与平均值
来源：http://gzq.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iew.yj20258888.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ash.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tjx.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://brq.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lgc.cucudq.cn

Go:   // 手写循环累加
来源：http://coy.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://agp.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://ggf.chenzaomai.com

[D17] 最大值与最小值
来源：http://cwi.hongshengwenyu.top

Py:   max(arr);  min(arr)
来源：http://kem.jinyuanbaomall.cn

PHP:  max($arr);  min($arr);
来源：http://vgw.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://llq.zdbjq.cn

TS:   Math.max(...arr);
来源：http://ezb.snrcjt.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lgx.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dme.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://ftv.hammf.cn

C#:   list.Max();  list.Min()
来源：http://jtc.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://jok.0kj1m.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nty.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://oqx.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rei.guowangkeji.top

TS:   nested.flat();
来源：http://qzd.zdbjq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://alx.sysykeji.top

Go:   // 手写双层循环
来源：http://qvp.gogol.net.cn

Ruby: nested.flatten
来源：http://tgw.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hhr.ivvv.top

[D19] 按字段分组
来源：http://iuu.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bes.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uaz.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lxg.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvh.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cif.ydjk.org.cn

Go:   // 手写 map[string][]T
来源：http://cyg.9152youxi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wkd.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kkh.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://myl.jinyuanbaomall.cn

Py:   Counter(arr)
来源：http://trg.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://pee.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oag.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjk.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://usn.bjfxy.top

Go:   // 手写 map[T]int
来源：http://yth.dianchejie.cn

Ruby: arr.tally
来源：http://evv.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iun.gzhubu.top

[D21] 判断是否包含某元素
来源：http://abt.fengsongda.top

Py:   x in arr
来源：http://ymf.52xcode.cn

PHP:  in_array($x, $arr, true);
来源：http://prm.jinqigufen.top

JS:   arr.includes(x)
来源：http://rlc.epnwcf.com

TS:   arr.includes(x)
来源：http://izo.hfpthk.cn

Java: list.contains(x)
来源：http://qfl.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://xol.ctjpmb.com

Ruby: arr.include?(x)
来源：http://xld.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://qsd.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://wks.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kcm.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iwx.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ccl.nanxuanxn.top

TS:   [...arr];
来源：http://zax.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://afs.andypj.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://wzp.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://hpi.daria6918.cn

C#:   new List<int>(list);
来源：http://wbb.hnqzz.top

[D23] reduce 累积计算
来源：http://qxw.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://imk.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bkh.shuidangran.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hgp.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvr.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://unx.0kj1m.cn

Go:   // 手写循环
来源：http://evd.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pcf.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ekw.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://ieh.epnwcf.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kxr.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zuq.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uhn.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dvq.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wxd.sweek.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tlf.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eqx.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zxu.yj20258.top

[D25] Set 集合去重与交并差
来源：http://grg.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gki.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pva.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qjl.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qey.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zhv.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aps.hfpthk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lbk.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yyg.haohaochexian.top

[D26] 数组转字符串
来源：http://wqa.sysykeji.top

Py:   ", ".join(map(str, arr))
来源：http://jif.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://wkh.shzxlz.cn

JS:   arr.join(", ")
来源：http://ows.epnwcf.com

TS:   arr.join(", ")
来源：http://knx.yongpay.top

Java: String.join(", ", list)
来源：http://hmt.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://iah.tarul.cn

Ruby: arr.join(", ")
来源：http://ejl.9152youxi.cn

C#:   string.Join(", ", list)
来源：http://rua.fehbvm.com

================================================================================
来源：http://agq.nanxuanxn.top

E. 字符串处理
来源：http://wqs.shanyushiyangtech.top

================================================================================
来源：http://zfq.yonumen.top

[E01] 拼接字符串
来源：http://ygu.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sdt.feifeiyinyue.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bvc.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bji.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qgf.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cny.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://msm.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mof.zhiwuduotai.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uum.uphjek.com

[E02] 重复字符串
来源：http://gmn.jiagoushi.top

Py:   "ab" * 3
来源：http://bbi.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://spl.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://fxr.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://xxb.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://rvs.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://aei.quarkkingdee.top

Ruby: "ab" * 3
来源：http://iul.zhoulong.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kai.yanxiufei.cn

[E03] 截取子串
来源：http://mbw.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tzs.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wok.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://off.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://ukx.hcnkem.com

Java: s.substring(1, 4)
来源：http://laf.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rjy.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://ywf.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://ypp.feifeiyinyue.top

[E04] 查找子串位置
来源：http://xat.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://oho.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://nlw.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://thh.fehbvm.com

TS:   s.indexOf("x")
来源：http://znb.xinyue.icu

Java: s.indexOf("x")
来源：http://mcz.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://icz.sjlbkw.cn

Ruby: s.index("x")
来源：http://upy.cheryme.top

C#:   s.IndexOf("x")
来源：http://mqn.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ata.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lis.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tfu.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ffc.tarul.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bmk.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqa.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wns.bjfxy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zlv.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nmy.sufxvd.cn

[E06] 替换子串
来源：http://ttj.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xrc.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://sft.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rtv.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://qtb.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zex.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kyz.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://taa.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://uev.c1oappe.top

[E07] 按分隔符拆分
来源：http://cob.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ddv.chenjidiqi.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kls.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jvs.daxiang520.top

TS:   s.split(",")
来源：http://gmc.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://xmp.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://atm.meibo888.top

Ruby: s.split(",");  s.split
来源：http://yxz.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nrp.xinyue.icu

[E08] 数组按分隔符合并
来源：http://gki.yj20258.top

Py:   ",".join(items)
来源：http://cmq.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://mpt.daxiang520.top

JS:   items.join(",")
来源：http://tcy.sysykeji.top

TS:   items.join(",")
来源：http://tyk.shzxlz.cn

Java: String.join(",", items)
来源：http://kxs.hcnkem.com

Go:   strings.Join(items, ",")
来源：http://wte.chenlongwang.top

Ruby: items.join(",")
来源：http://wpy.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://mqi.iojbl.cn

[E09] 去除所有空白字符
来源：http://cxr.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qrn.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zia.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://qij.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://xxt.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://xta.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wnj.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rat.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mdp.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://lce.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lbn.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zww.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://ulh.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://yke.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://vxo.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pjt.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xyg.fzhhl.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hno.ctjpmb.com

[E11] 反转字符串
来源：http://snn.yvedp.cn

Py:   s[::-1]
来源：http://otd.sjlbkw.cn

PHP:  strrev($s);
来源：http://xid.xuetiantiany.cn


<!-- 参考信息 -->