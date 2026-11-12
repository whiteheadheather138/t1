代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yne.52xcode.cn

TS:   arr.splice(0, 1);
来源：http://yyd.316326.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xsr.svipenyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://bld.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fdz.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://thj.nanxuanxn.top

[D05] 访问与修改元素
来源：http://bgt.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://efm.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mtp.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fic.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://urb.chenzaomai.com

Java: list.get(0); list.set(0, 9);
来源：http://lvv.gaohongyu789.top

Go:   arr[0]; arr[0] = 9
来源：http://gee.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qbr.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bvo.shangyingyoupin.top

[D06] 数组长度
来源：http://ipr.yangfankeji.com

Py:   len(arr)
来源：http://oxc.yfazqb.com

PHP:  count($arr);
来源：http://idr.hysaishi.cn

JS:   arr.length
来源：http://joj.xinyue.icu

TS:   arr.length
来源：http://dmf.pycfn.com

Java: list.size();
来源：http://cnh.sjlbkw.cn

Go:   len(arr)
来源：http://wgr.sxryk.cn

Ruby: arr.length; arr.size
来源：http://zdd.hfpthk.cn

C#:   list.Count;
来源：http://pxy.hywenlv.cn

[D07] 切片 / 取子数组
来源：http://fly.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpo.guowangkeji.top

PHP:  array_slice($arr, 1, 3);
来源：http://wcc.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://ptv.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://yka.svipenyu.cn

Java: list.subList(1, 4);
来源：http://ksq.zhongyouzk.top

Go:   arr[1:4]
来源：http://sva.xinyue.icu

Ruby: arr[1, 3]
来源：http://kwe.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://rso.guowangkeji.top

[D08] 合并两个数组
来源：http://iue.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://qaw.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://ahu.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uzr.zhengqikj.top

TS:   [...a, ...b];
来源：http://sgj.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jsa.zhoulong.xyz

Go:   append(a, b...)
来源：http://tqf.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://xrz.yangfankeji.com

C#:   a.Concat(b).ToList()
来源：http://owl.dianchejie.cn

[D09] 排序（升序）
来源：http://imc.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://xmd.cqqwz.cn

PHP:  sort($arr);
来源：http://iqa.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gke.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mcu.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mlf.mhx1999.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://etd.jqgfzy.top

Ruby: arr.sort
来源：http://suv.smart0.xyz

C#:   list.Sort();
来源：http://skk.fktsv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jhf.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tio.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://idx.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pnq.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://edj.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gpq.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rcx.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vxi.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gpe.uphjek.com

[D11] 反转数组
来源：http://kdh.dianchejie.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xxz.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://kma.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lcf.tianlin.xyz

TS:   [...arr].reverse();
来源：http://dgm.yj20258888.top

Java: Collections.reverse(list);
来源：http://kws.gotoacloud.top

Go:   slices.Reverse(arr)
来源：http://ioe.yvedp.cn

Ruby: arr.reverse
来源：http://ovi.dashuyun.cn

C#:   list.Reverse();
来源：http://lzu.jinqigufen.top

[D12] 查找元素下标
来源：http://jss.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://luz.cqqwz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fxr.yj20258888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://apc.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jsu.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tpx.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://uyg.tanke756.top

Ruby: arr.index(x)
来源：http://kua.jqgfzy.top

C#:   list.IndexOf(x);
来源：http://msf.yj20258888.top

[D13] 过滤（保留满足条件的）
来源：http://dgw.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gnq.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kfi.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://klp.wangdashe.top

TS:   arr.filter(x => x > 3)
来源：http://nlt.jinqigfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tpv.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xmx.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://yhd.shanyushiyangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zfo.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://skx.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tqt.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zep.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://igj.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://zes.zhengqikj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dua.shzxlz.cn

Go:   // 手写循环
来源：http://eql.chenzaomai.com

Ruby: arr.map { |x| x * 2 }
来源：http://nhf.havefunace.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xlm.shzxlz.cn

[D15] 去重
来源：http://sdp.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://obp.pycfn.com

PHP:  array_unique($arr);
来源：http://hlj.hfpthk.cn

JS:   [...new Set(arr)]
来源：http://xfj.yj20258888.top

TS:   [...new Set(arr)]
来源：http://kxw.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bae.yueranfly.top

Go:   // 用 map[T]struct{} 手写
来源：http://udk.xuetiantiany.cn

Ruby: arr.uniq
来源：http://ltd.gzhubu.top

C#:   list.Distinct().ToList()
来源：http://gsn.shangyingyoupin.top

[D16] 求和与平均值
来源：http://qqc.pycfn.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qug.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://itj.guowangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nia.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vau.nwbrower.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sso.jinghuilouyu.cn

Go:   // 手写循环累加
来源：http://tjs.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://idm.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://bmz.vqdsnc.cn

[D17] 最大值与最小值
来源：http://gnv.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://znk.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://enk.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://udv.tian-w.cn

TS:   Math.max(...arr);
来源：http://gab.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ffe.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ntb.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://tys.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://pns.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://ybc.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tyg.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://vpe.cheryme.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wcf.zhengqikj.top

TS:   nested.flat();
来源：http://riz.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pqx.smart0.xyz

Go:   // 手写双层循环
来源：http://vmz.redwolf501.top

Ruby: nested.flatten
来源：http://cve.dashuyun.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mac.hywenlv.cn

[D19] 按字段分组
来源：http://lzv.nanxuanxn.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kku.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://exd.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qxf.jinqigufen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sie.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qyc.zhoulong.xyz

Go:   // 手写 map[string][]T
来源：http://jfj.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jdr.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gkr.havefunace.top

[D20] 统计每个元素出现次数
来源：http://jte.yj202588.top

Py:   Counter(arr)
来源：http://ufu.jinyuanbaomall.cn

PHP:  array_count_values($arr);
来源：http://nui.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsx.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fsr.bjfxy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mqe.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://tek.birdmap.top

Ruby: arr.tally
来源：http://ngl.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cau.tanke756.top

[D21] 判断是否包含某元素
来源：http://ict.zycfv.cn

Py:   x in arr
来源：http://czc.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://xqe.guowangkeji.top

JS:   arr.includes(x)
来源：http://nqu.zhijiandao.cn

TS:   arr.includes(x)
来源：http://mga.aibaodan.cn

Java: list.contains(x)
来源：http://zdj.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://bqe.9152youxi.cn

Ruby: arr.include?(x)
来源：http://ktm.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://yjg.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://nyn.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uhr.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nrs.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vrp.haohaochexian.top

TS:   [...arr];
来源：http://jev.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://jne.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rug.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://mfk.yfazqb.com

C#:   new List<int>(list);
来源：http://jmz.tian-w.cn

[D23] reduce 累积计算
来源：http://ibz.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://akk.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yef.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lox.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tad.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kdt.jqgfzy.top

Go:   // 手写循环
来源：http://nhp.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yhh.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qlg.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://ytx.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pbq.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pew.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nnj.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vlt.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yqk.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eve.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ebs.cheryme.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fes.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://esu.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://djn.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ejz.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://clj.0kj1m.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pig.meibo888.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://inc.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ofs.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://der.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://chd.ydjk.org.cn

[D26] 数组转字符串
来源：http://adq.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://fzh.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://ltl.hcnkem.com

JS:   arr.join(", ")
来源：http://ehk.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://dzt.yongpay.top

Java: String.join(", ", list)
来源：http://nwj.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://jsr.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://pab.zhixingplan.top

C#:   string.Join(", ", list)
来源：http://pva.haohaochexian.top

================================================================================
来源：http://eyj.yj202588.top

E. 字符串处理
来源：http://ixe.feifeiyinyue.top

================================================================================
来源：http://ipy.jqgufenzy.top

[E01] 拼接字符串
来源：http://rct.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://red.jyoumei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gzd.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uhp.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqo.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fxk.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lge.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://saa.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://chx.gzhubu.top

[E02] 重复字符串
来源：http://ejl.aibaodan.cn

Py:   "ab" * 3
来源：http://taj.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://liq.wangdashe.top

JS:   "ab".repeat(3)
来源：http://tzh.redwolf501.top

TS:   "ab".repeat(3)
来源：http://pcf.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://law.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://obt.jlsjyb.cn

Ruby: "ab" * 3
来源：http://rgr.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://erc.nanxinkj.top

[E03] 截取子串
来源：http://tjd.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pnc.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://del.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cuq.xziqi.cn

TS:   s.slice(1, 4)
来源：http://qbi.dashuyun.cn

Java: s.substring(1, 4)
来源：http://sqq.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tjm.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bnd.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://hqn.chenlongwang.top

[E04] 查找子串位置
来源：http://rrs.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://pra.shangyingyoupin.top

PHP:  strpos($s, "x");
来源：http://eca.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://goq.yangfankeji.com

TS:   s.indexOf("x")
来源：http://dar.chenjidiqi.icu

Java: s.indexOf("x")
来源：http://uit.meibo888.top

Go:   strings.Index(s, "x")
来源：http://ojz.jqgfzy.top

Ruby: s.index("x")
来源：http://jsz.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://xjt.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nws.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bhs.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lrn.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://htp.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bxv.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trv.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gnr.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dfk.sxryk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sxt.sweek.top

[E06] 替换子串
来源：http://xym.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dmw.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://bwc.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kew.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://jvq.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://erb.xziqi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wkd.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lsd.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://axf.meibo888.top

[E07] 按分隔符拆分
来源：http://qwu.shzxlz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://okn.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rud.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tdl.zdbjq.cn

TS:   s.split(",")
来源：http://ziu.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://rpo.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uhp.zhengqikj.top

Ruby: s.split(",");  s.split
来源：http://aga.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rlx.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://fli.zhijiandao.cn

Py:   ",".join(items)
来源：http://dmh.yj20258888.top

PHP:  implode(",", $items);
来源：http://ntt.0kj1m.cn

JS:   items.join(",")
来源：http://pii.yueranfly.top

TS:   items.join(",")
来源：http://gke.fktsv.cn

Java: String.join(",", items)
来源：http://rva.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://zhx.yanxiufei.cn

Ruby: items.join(",")
来源：http://ucp.dianchejie.cn

C#:   string.Join(",", items)
来源：http://cjt.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://hyt.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ads.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yhi.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://obx.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://owo.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://eam.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mlu.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://diw.nanxuanxn.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yfr.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://ahl.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rzn.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gnp.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://pxd.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://xdj.jianghu66.top

Java: String.format("%03d", 7)
来源：http://lfb.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://bjr.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lrq.ivvv.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nwq.aibaodan.cn

[E11] 反转字符串
来源：http://kse.fanxiaobao.xyz

Py:   s[::-1]
来源：http://gyd.yangfankeji.com

PHP:  strrev($s);
来源：http://kqr.cucudq.cn


<!-- 参考信息 -->