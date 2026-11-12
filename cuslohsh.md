代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bka.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hrk.nanxinkj.top

TS:   arr[0]; arr.at(-1);
来源：http://uwb.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://eac.zhoulong.xyz

Go:   arr[0]; arr[0] = 9
来源：http://gvd.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sib.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wif.shangyingyoupin.top

[D06] 数组长度
来源：http://vux.bbcook.cn

Py:   len(arr)
来源：http://lmx.hesvh.cn

PHP:  count($arr);
来源：http://gdd.ppjwa.cn

JS:   arr.length
来源：http://ydk.yongpay.top

TS:   arr.length
来源：http://jun.cucudq.cn

Java: list.size();
来源：http://nud.xuetiantiany.cn

Go:   len(arr)
来源：http://vmj.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://fhx.chenjidiqi.icu

C#:   list.Count;
来源：http://xxk.birdmap.top

[D07] 切片 / 取子数组
来源：http://sdq.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://izs.tian-w.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vwy.tanke756.top

JS:   arr.slice(1, 4);
来源：http://gbe.ydzc1.top

TS:   arr.slice(1, 4);
来源：http://osp.nwbrower.top

Java: list.subList(1, 4);
来源：http://ngi.zhongyouzk.top

Go:   arr[1:4]
来源：http://vcw.cashguo.top

Ruby: arr[1, 3]
来源：http://akv.jqgufenzy.top

C#:   list.GetRange(1, 3);
来源：http://wyc.dashuyun.cn

[D08] 合并两个数组
来源：http://pos.ybcxt.top

Py:   a + b;  a.extend(b)
来源：http://guu.hfpthk.cn

PHP:  array_merge($a, $b);
来源：http://rpk.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://adc.c1oappe.top

TS:   [...a, ...b];
来源：http://pcx.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hnl.fzhhl.top

Go:   append(a, b...)
来源：http://exb.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://wvn.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://ndv.zhijiandao.cn

[D09] 排序（升序）
来源：http://dyd.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://idn.snrcjt.cn

PHP:  sort($arr);
来源：http://avv.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rjz.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ccb.chenjidiqi.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://qqk.dianchejie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://idf.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://jjm.aizwys.cn

C#:   list.Sort();
来源：http://nso.yonumen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://isc.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ccs.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yjs.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://clg.quarkkingdee.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wbh.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cof.yuanzhike.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vsu.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lza.yuxming.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://slq.kuanghao11.cn

[D11] 反转数组
来源：http://wrq.shzxlz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qtb.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://qjs.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://giv.0kj1m.cn

TS:   [...arr].reverse();
来源：http://svh.shanyushiyangkeji.top

Java: Collections.reverse(list);
来源：http://gtn.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://lei.cdnleiting.top

Ruby: arr.reverse
来源：http://isa.snrcjt.cn

C#:   list.Reverse();
来源：http://brw.jlsjyb.cn

[D12] 查找元素下标
来源：http://yzt.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://igx.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ldx.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sfo.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nin.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ubx.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://sdl.smart0.xyz

Ruby: arr.index(x)
来源：http://uzh.pycfn.com

C#:   list.IndexOf(x);
来源：http://ixp.kuanghao11.cn

[D13] 过滤（保留满足条件的）
来源：http://oqo.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qdf.meibo888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qvo.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://cck.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://zhz.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pij.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kip.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://sit.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://bhh.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://oxa.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dsm.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pkk.mhx1999.top

JS:   arr.map(x => x * 2)
来源：http://qjf.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://tjs.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zta.cdnleiting.top

Go:   // 手写循环
来源：http://tak.xingfuxueyuan.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://xsc.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xfu.yfazqb.com

[D15] 去重
来源：http://yly.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qrd.dashuyun.cn

PHP:  array_unique($arr);
来源：http://gaz.uphjek.com

JS:   [...new Set(arr)]
来源：http://cff.ivvv.top

TS:   [...new Set(arr)]
来源：http://xdg.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qqv.jiagoushi.top

Go:   // 用 map[T]struct{} 手写
来源：http://jay.yuanzhike.top

Ruby: arr.uniq
来源：http://caw.shanyushiyangtech.top

C#:   list.Distinct().ToList()
来源：http://ewq.sweek.top

[D16] 求和与平均值
来源：http://oqd.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://alk.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hml.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://epy.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ogn.yuxming.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://izc.daxiang520.top

Go:   // 手写循环累加
来源：http://rzg.yj202588.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wic.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://chb.ppjwa.cn

[D17] 最大值与最小值
来源：http://cej.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://lmk.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://fgc.nanxinkj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wvu.jiagoushi.top

TS:   Math.max(...arr);
来源：http://lon.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ajr.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tuy.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://xwq.zdqjudy.top

C#:   list.Max();  list.Min()
来源：http://tuo.316326.xyz

[D18] 扁平化嵌套数组
来源：http://tqj.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sxe.hammf.cn

PHP:  array_merge(...$nested);
来源：http://bhd.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hbo.cashguo.top

TS:   nested.flat();
来源：http://aoc.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ywt.c1oappe.top

Go:   // 手写双层循环
来源：http://fzu.wangdashe.top

Ruby: nested.flatten
来源：http://kzu.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://qyx.316326.xyz

[D19] 按字段分组
来源：http://cat.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kvt.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rjb.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mdr.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bis.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fil.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://nrv.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rio.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nme.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://ixt.yj20258888.top

Py:   Counter(arr)
来源：http://gfw.yj202588.top

PHP:  array_count_values($arr);
来源：http://qgf.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uol.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dwe.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hnw.316326.xyz

Go:   // 手写 map[T]int
来源：http://fnm.ivvv.top

Ruby: arr.tally
来源：http://unw.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rmp.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://kuv.wangshuangyany.cn

Py:   x in arr
来源：http://ryu.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://psc.jianghu66.top

JS:   arr.includes(x)
来源：http://xlx.tanke756.top

TS:   arr.includes(x)
来源：http://jst.nwbrower.top

Java: list.contains(x)
来源：http://bti.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://fza.xziqi.cn

Ruby: arr.include?(x)
来源：http://fla.sjlbkw.cn

C#:   list.Contains(x)
来源：http://psd.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://sbb.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sxw.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tbx.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rce.yj20258.top

TS:   [...arr];
来源：http://mim.xziqi.cn

Java: new ArrayList<>(list);
来源：http://xyz.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://uxy.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://vzo.daxiang520.top

C#:   new List<int>(list);
来源：http://bxc.aizwys.cn

[D23] reduce 累积计算
来源：http://maw.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gqa.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://odw.shanyushiyangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dup.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://awx.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zvv.haohaochexian.top

Go:   // 手写循环
来源：http://jac.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iko.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pyh.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://rwc.zhixingplan.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mbz.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vtf.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://exy.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fdo.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zwh.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kej.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://chb.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qqw.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://vfb.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pnl.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jea.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dub.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://otz.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ozg.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bhz.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cma.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eon.zdqjudy.top

[D26] 数组转字符串
来源：http://mic.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://hyw.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://btt.redwolf501.top

JS:   arr.join(", ")
来源：http://yza.redwolf501.top

TS:   arr.join(", ")
来源：http://tjz.0kj1m.cn

Java: String.join(", ", list)
来源：http://zgg.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://afp.birdmap.top

Ruby: arr.join(", ")
来源：http://ftu.fktsv.cn

C#:   string.Join(", ", list)
来源：http://bkf.fzhhl.top

================================================================================
来源：http://caf.jyoumei.cn

E. 字符串处理
来源：http://zcg.daria6918.cn

================================================================================
来源：http://pup.ydzc1.top

[E01] 拼接字符串
来源：http://kku.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kxz.andypj.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://apg.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cer.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gzk.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kdq.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ujk.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ssv.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hqo.guannengcc.top

[E02] 重复字符串
来源：http://kkc.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://dyx.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://lwu.yongpay.top

JS:   "ab".repeat(3)
来源：http://owy.jianghu66.top

TS:   "ab".repeat(3)
来源：http://qxf.haohaochexian.top

Java: "ab".repeat(3)
来源：http://dyt.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://yjh.haohaochexian.top

Ruby: "ab" * 3
来源：http://bhu.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://psq.yfazqb.com

[E03] 截取子串
来源：http://cwn.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zng.gotoacloud.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://muw.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zoy.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://ifa.zhaomingkeji.xyz

Java: s.substring(1, 4)
来源：http://tkj.aibaodan.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oyh.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://tis.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://yia.sxryk.cn

[E04] 查找子串位置
来源：http://cyp.yonumen.top

Py:   s.find("x");  s.index("x")
来源：http://duf.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://lju.cheryme.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aun.chenlongwang.top

TS:   s.indexOf("x")
来源：http://cxr.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://zua.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://fbg.aibaodan.cn

Ruby: s.index("x")
来源：http://pld.yj20258888.top

C#:   s.IndexOf("x")
来源：http://vmv.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://izl.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kpd.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uen.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fcz.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cuv.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zph.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oui.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nln.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mdc.sjlbkw.cn

[E06] 替换子串
来源：http://fsi.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qda.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://twh.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mxa.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://xox.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://elh.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kqg.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yah.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://dbl.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://ivs.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bbv.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fgz.guowangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fcp.cucudq.cn

TS:   s.split(",")
来源：http://lzp.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://eqr.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fwq.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://rpt.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ion.xylfe.cn

[E08] 数组按分隔符合并
来源：http://msy.mhx1999.top

Py:   ",".join(items)
来源：http://ddl.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://kow.ivvv.top

JS:   items.join(",")
来源：http://nij.0kj1m.cn

TS:   items.join(",")
来源：http://urk.316326.xyz

Java: String.join(",", items)
来源：http://gcx.zycfv.cn

Go:   strings.Join(items, ",")
来源：http://hnu.xinyue.icu

Ruby: items.join(",")
来源：http://gvn.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://apm.hammf.cn

[E09] 去除所有空白字符
来源：http://dkl.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tuk.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ojw.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ycn.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://wtr.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://nku.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hur.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://uyx.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zci.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://rtf.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fch.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qaa.zhijiandao.cn

JS:   "7".padStart(3, "0")
来源：http://wgk.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://eug.daria6918.cn

Java: String.format("%03d", 7)
来源：http://ngj.chenjidiqi.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://ovu.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rjl.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lmq.nwbrower.top

[E11] 反转字符串
来源：http://zqz.cdnleiting.top

Py:   s[::-1]
来源：http://vyu.chenlongwang.top

PHP:  strrev($s);
来源：http://ksj.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://uka.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://adp.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dpt.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://lif.tarul.cn

Ruby: s.reverse
来源：http://xni.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://gkj.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://etr.yonumen.top

Py:   s.count("a")
来源：http://woz.wangshuangyany.cn


<!-- 参考信息 -->