代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ckd.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://cek.andypj.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rta.yfazqb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qmf.iojbl.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fxj.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gpu.havefunace.top

[D05] 访问与修改元素
来源：http://elk.zhiwuduotai.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jpc.ivvv.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vod.pengpengdd.cyou

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sgz.yfazqb.com

TS:   arr[0]; arr.at(-1);
来源：http://dyv.yvedp.cn

Java: list.get(0); list.set(0, 9);
来源：http://hwd.tanke756.top

Go:   arr[0]; arr[0] = 9
来源：http://hhs.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lka.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hrr.hywenlv.cn

[D06] 数组长度
来源：http://jim.cdnleiting.top

Py:   len(arr)
来源：http://klf.dashuyun.cn

PHP:  count($arr);
来源：http://svo.xinyue.icu

JS:   arr.length
来源：http://hpe.xingfuxueyuan.xyz

TS:   arr.length
来源：http://dzz.aibaodan.cn

Java: list.size();
来源：http://xhf.aibaodan.cn

Go:   len(arr)
来源：http://fmh.zhixingplan.top

Ruby: arr.length; arr.size
来源：http://iia.sjlbkw.cn

C#:   list.Count;
来源：http://exd.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://uys.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://agt.vehdjk.com

PHP:  array_slice($arr, 1, 3);
来源：http://siu.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://ykm.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://jyf.sufxvd.cn

Java: list.subList(1, 4);
来源：http://yir.cqqwz.cn

Go:   arr[1:4]
来源：http://qxk.ybcxt.top

Ruby: arr[1, 3]
来源：http://cmp.0kj1m.cn

C#:   list.GetRange(1, 3);
来源：http://jmc.cdnleiting.top

[D08] 合并两个数组
来源：http://prm.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://rkr.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://gyl.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gye.52xcode.cn

TS:   [...a, ...b];
来源：http://gaz.jlsjyb.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://scn.shangyingyoupin.top

Go:   append(a, b...)
来源：http://zhq.gogol.net.cn

Ruby: a + b;  a.concat(b)
来源：http://pdu.shzxlz.cn

C#:   a.Concat(b).ToList()
来源：http://zfd.jyoumei.cn

[D09] 排序（升序）
来源：http://ddr.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://aql.uphjek.com

PHP:  sort($arr);
来源：http://tlt.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vrw.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cpo.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tfu.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qgm.xuetiantiany.cn

Ruby: arr.sort
来源：http://urq.cheryme.top

C#:   list.Sort();
来源：http://jgl.hywenlv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://doa.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cfw.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oxl.snrcjt.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpy.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ibc.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://twq.nanxuanxn.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://awg.hysaishi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ozc.snrcjt.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wyj.jianghu66.top

[D11] 反转数组
来源：http://qkv.tian-w.cn

Py:   arr[::-1];  arr.reverse()
来源：http://omz.yj20258.top

PHP:  array_reverse($arr);
来源：http://kiy.yj20258.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sgx.hammf.cn

TS:   [...arr].reverse();
来源：http://yvd.0kj1m.cn

Java: Collections.reverse(list);
来源：http://svj.tanke756.top

Go:   slices.Reverse(arr)
来源：http://lcd.jyoumei.cn

Ruby: arr.reverse
来源：http://lvg.tian-w.cn

C#:   list.Reverse();
来源：http://jpf.chenjidiqi.icu

[D12] 查找元素下标
来源：http://trq.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://lbs.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jfq.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bdj.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gqg.yangfankeji.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gyy.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://dyq.jinqigfzy.top

Ruby: arr.index(x)
来源：http://zju.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://wnz.chenjidiqi.icu

[D13] 过滤（保留满足条件的）
来源：http://vrv.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zjy.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hyl.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://mnd.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://jpv.yj20258.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ynu.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://isp.zycfv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fwl.fzhhl.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fjo.ctjpmb.com

[D14] 映射转换（每个元素变形）
来源：http://arh.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zhq.sufxvd.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fvs.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://fbd.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://vlu.zhoulong.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://kfd.feifeiyinyue.top

Go:   // 手写循环
来源：http://kpb.feifeiyinyue.top

Ruby: arr.map { |x| x * 2 }
来源：http://dtr.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dng.chenjidiqi.icu

[D15] 去重
来源：http://rml.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://omp.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://phr.c1oappe.top

JS:   [...new Set(arr)]
来源：http://xat.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://xmt.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rjw.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://urm.andypj.xyz

Ruby: arr.uniq
来源：http://jby.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://lii.dianchejie.cn

[D16] 求和与平均值
来源：http://wiy.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lxu.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hve.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjs.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hgh.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://umx.zdbjq.cn

Go:   // 手写循环累加
来源：http://bhx.aibaodan.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tap.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://btb.yonumen.top

[D17] 最大值与最小值
来源：http://asl.ydjk.org.cn

Py:   max(arr);  min(arr)
来源：http://zgz.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://lai.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rxu.hcnkem.com

TS:   Math.max(...arr);
来源：http://tju.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xxz.gogol.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kvm.yj20258.top

Ruby: arr.max;  arr.min
来源：http://jty.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://hms.zhiwuduotai.top

[D18] 扁平化嵌套数组
来源：http://lky.hywenlv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://def.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://yba.chenlongwang.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ddw.jinqigufen.top

TS:   nested.flat();
来源：http://yda.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uag.jqgfzy.top

Go:   // 手写双层循环
来源：http://aoq.bjfxy.top

Ruby: nested.flatten
来源：http://yfu.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cny.gogol.net.cn

[D19] 按字段分组
来源：http://sgi.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://akf.haohaochexian.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ipm.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://div.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xjb.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://abt.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://yoz.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bje.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dcw.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://jak.haohaochexian.top

Py:   Counter(arr)
来源：http://glt.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://wpw.yanxiufei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kln.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ius.yanxiufei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://icx.yj202588.top

Go:   // 手写 map[T]int
来源：http://krz.shzxlz.cn

Ruby: arr.tally
来源：http://rgs.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tsk.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://ttt.yj20258888.top

Py:   x in arr
来源：http://rxr.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://ujc.ywan-chungtsiang.top

JS:   arr.includes(x)
来源：http://iwf.redwolf501.top

TS:   arr.includes(x)
来源：http://yzi.yuxming.cn

Java: list.contains(x)
来源：http://ykm.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://twq.xziqi.cn

Ruby: arr.include?(x)
来源：http://cvm.jinyuanbaomall.cn

C#:   list.Contains(x)
来源：http://sap.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://jlz.chenzaomai.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oez.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qky.fzhhl.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zmp.zhaomingkeji.xyz

TS:   [...arr];
来源：http://rjn.hcnkem.com

Java: new ArrayList<>(list);
来源：http://xba.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://utf.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://oup.sjlbkw.cn

C#:   new List<int>(list);
来源：http://irg.guannengcc.top

[D23] reduce 累积计算
来源：http://pwc.shanyushiyangtech.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nqj.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xwo.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ksx.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vlp.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yvf.zhongyouzk.top

Go:   // 手写循环
来源：http://syt.gogol.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://idb.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yao.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://dxe.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ich.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ltj.chenzaomai.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zpr.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://imy.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qyu.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzc.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fbi.fzhhl.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lss.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://jto.yangfankeji.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qiu.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kag.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gcr.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jhd.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://afh.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hml.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://erm.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wbf.chenlongwang.top

[D26] 数组转字符串
来源：http://kzj.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://dnc.yuanzhike.top

PHP:  implode(", ", $arr);
来源：http://spj.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://qvr.chenjidiqi.icu

TS:   arr.join(", ")
来源：http://lvj.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://yiw.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://kfc.9152youxi.cn

Ruby: arr.join(", ")
来源：http://vjk.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://mtc.c1oappe.top

================================================================================
来源：http://nau.jqgfzy.top

E. 字符串处理
来源：http://sgg.yongpay.top

================================================================================
来源：http://ksv.jqgufenzy.top

[E01] 拼接字符串
来源：http://ldt.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ltv.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gss.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qcp.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fvd.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nae.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kaz.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tmu.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://thc.tian-w.cn

[E02] 重复字符串
来源：http://squ.snrcjt.cn

Py:   "ab" * 3
来源：http://hem.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://oky.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://eau.xuanzx.com

TS:   "ab".repeat(3)
来源：http://eps.yueranfly.top

Java: "ab".repeat(3)
来源：http://nqm.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://fgs.0kj1m.cn

Ruby: "ab" * 3
来源：http://tkw.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://doj.iojbl.cn

[E03] 截取子串
来源：http://yba.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qlu.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ayj.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ctc.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://jdr.ydzc1.top

Java: s.substring(1, 4)
来源：http://tgi.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bhz.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://nuz.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://ygh.jqgufenzy.top

[E04] 查找子串位置
来源：http://jug.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://lev.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://mas.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sgd.epnwcf.com

TS:   s.indexOf("x")
来源：http://dll.cucudq.cn

Java: s.indexOf("x")
来源：http://ihx.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://rfk.yj20258888.top

Ruby: s.index("x")
来源：http://dqu.yonumen.top

C#:   s.IndexOf("x")
来源：http://uuh.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://oeg.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://asj.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wwa.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lzh.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uvb.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twl.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nbi.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wbu.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://umv.jqgfzy.top

[E06] 替换子串
来源：http://grn.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vkf.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://ovm.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gas.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://xci.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wxd.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://boq.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rev.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://cjb.yonumen.top

[E07] 按分隔符拆分
来源：http://ibq.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lmm.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pev.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rin.tianlin.xyz

TS:   s.split(",")
来源：http://xtc.zhaomingkeji.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ljw.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pto.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://uyb.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nzj.zycfv.cn

[E08] 数组按分隔符合并
来源：http://lpu.yangfankeji.com

Py:   ",".join(items)
来源：http://rfw.yonumen.top

PHP:  implode(",", $items);
来源：http://igh.tanke756.top

JS:   items.join(",")
来源：http://jeg.xuanzx.com

TS:   items.join(",")
来源：http://jnm.hongshengwenyu.top

Java: String.join(",", items)
来源：http://zmy.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://qau.zhixingplan.top

Ruby: items.join(",")
来源：http://eks.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://ofe.hammf.cn

[E09] 去除所有空白字符
来源：http://iju.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tsd.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kwp.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://npm.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://hss.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://tud.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zpv.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://sbs.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fmj.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://fjz.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://seg.aizwys.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dbs.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://jup.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://she.redwolf501.top

Java: String.format("%03d", 7)
来源：http://flu.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iko.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eqs.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zwu.sxryk.cn

[E11] 反转字符串
来源：http://ftu.yj20258.top

Py:   s[::-1]
来源：http://riz.ctjpmb.com

PHP:  strrev($s);
来源：http://nme.chenzaomai.com


<!-- 参考信息 -->