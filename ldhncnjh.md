代发 wailian999

Py:   len(arr)
来源：http://xde.cheryme.top

PHP:  count($arr);
来源：http://xfb.fengsongda.top

JS:   arr.length
来源：http://fzf.yj202588.top

TS:   arr.length
来源：http://nqm.hysaishi.cn

Java: list.size();
来源：http://nvo.mhx1999.top

Go:   len(arr)
来源：http://vdr.cheryme.top

Ruby: arr.length; arr.size
来源：http://avx.birdmap.top

C#:   list.Count;
来源：http://xal.yj202588.top

[D07] 切片 / 取子数组
来源：http://eau.gogol.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gil.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://fkq.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://kni.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://zis.yongpay.top

Java: list.subList(1, 4);
来源：http://etk.yfazqb.com

Go:   arr[1:4]
来源：http://rnv.yueranfly.top

Ruby: arr[1, 3]
来源：http://qyk.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://jck.tianlin.xyz

[D08] 合并两个数组
来源：http://hxi.mhx1999.top

Py:   a + b;  a.extend(b)
来源：http://mmt.yvedp.cn

PHP:  array_merge($a, $b);
来源：http://ywj.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yev.hnqzz.top

TS:   [...a, ...b];
来源：http://wmk.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://roc.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://rvg.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://fac.wangdashe.top

C#:   a.Concat(b).ToList()
来源：http://lec.316326.xyz

[D09] 排序（升序）
来源：http://ssa.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://wpf.ppjwa.cn

PHP:  sort($arr);
来源：http://nvy.nwbrower.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fzq.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://pqi.hongshengwenyu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vym.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lrg.bbcook.cn

Ruby: arr.sort
来源：http://dpz.havefunace.top

C#:   list.Sort();
来源：http://jkp.mhx1999.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://iye.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hul.chenlongwang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gui.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hcg.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://sep.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jmt.guowangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://egg.9152youxi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qox.smart0.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qvi.andypj.xyz

[D11] 反转数组
来源：http://lmp.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://bur.fktsv.cn

PHP:  array_reverse($arr);
来源：http://bed.chenzaomai.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dfh.cdnleiting.top

TS:   [...arr].reverse();
来源：http://jci.tianlin.xyz

Java: Collections.reverse(list);
来源：http://yvx.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://mxd.dianchejie.cn

Ruby: arr.reverse
来源：http://ddt.0kj1m.cn

C#:   list.Reverse();
来源：http://ruz.xylfe.cn

[D12] 查找元素下标
来源：http://rzp.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://fur.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fcj.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rcz.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cin.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ryz.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://wrt.fktsv.cn

Ruby: arr.index(x)
来源：http://fss.yuxming.cn

C#:   list.IndexOf(x);
来源：http://dck.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://ufr.shzxlz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yga.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wiq.guowangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://inh.ctjpmb.com

TS:   arr.filter(x => x > 3)
来源：http://hcu.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jlq.jyoumei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zjz.jinqigufen.top

Ruby: arr.select { |x| x > 3 }
来源：http://fuz.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://efa.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://ogh.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jxx.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aok.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://ytf.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://rzl.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lnw.xuetiantiany.cn

Go:   // 手写循环
来源：http://aum.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gzu.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pdl.fzhhl.top

[D15] 去重
来源：http://mgj.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fhr.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://wjv.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://mod.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://sme.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yta.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://swk.meibo888.top

Ruby: arr.uniq
来源：http://avf.daxiang520.top

C#:   list.Distinct().ToList()
来源：http://zpu.xuetiantiany.cn

[D16] 求和与平均值
来源：http://ppi.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://guk.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://chf.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgm.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pbb.jinqigufen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://flz.jqgufenzy.top

Go:   // 手写循环累加
来源：http://zmf.fehbvm.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jgl.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://fra.snrcjt.cn

[D17] 最大值与最小值
来源：http://luv.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://vnh.wangdashe.top

PHP:  max($arr);  min($arr);
来源：http://moc.wangdashe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pfu.pycfn.com

TS:   Math.max(...arr);
来源：http://rds.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://syb.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xtg.yonumen.top

Ruby: arr.max;  arr.min
来源：http://hmw.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://hbg.xziqi.cn

[D18] 扁平化嵌套数组
来源：http://ypc.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yka.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://yrw.yuxming.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://czy.chenzaomai.com

TS:   nested.flat();
来源：http://aip.fehbvm.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://drq.cqqwz.cn

Go:   // 手写双层循环
来源：http://ask.jinqigfzy.top

Ruby: nested.flatten
来源：http://prc.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kgz.vqdsnc.cn

[D19] 按字段分组
来源：http://hya.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hvx.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bol.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bog.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://xzn.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cbq.sweek.top

Go:   // 手写 map[string][]T
来源：http://vew.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yew.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wgw.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://byv.hcnkem.com

Py:   Counter(arr)
来源：http://laj.52xcode.cn

PHP:  array_count_values($arr);
来源：http://iys.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bat.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nvz.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://irb.ydzc1.top

Go:   // 手写 map[T]int
来源：http://xaa.birdmap.top

Ruby: arr.tally
来源：http://nzt.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lbz.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://oss.yj20258888.top

Py:   x in arr
来源：http://wyc.uphjek.com

PHP:  in_array($x, $arr, true);
来源：http://akj.zdbjq.cn

JS:   arr.includes(x)
来源：http://hro.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://wik.tian-w.cn

Java: list.contains(x)
来源：http://qai.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://yom.chenzaomai.com

Ruby: arr.include?(x)
来源：http://rnz.vqdsnc.cn

C#:   list.Contains(x)
来源：http://ryu.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://dcv.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://woq.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qgi.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cwu.xuanzx.com

TS:   [...arr];
来源：http://uvb.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://qul.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://pyo.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://xnp.ivvv.top

C#:   new List<int>(list);
来源：http://ttz.hcnkem.com

[D23] reduce 累积计算
来源：http://qgr.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fgd.jinqigufen.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gci.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mub.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fxd.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oqa.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://svw.zhoulong.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wkq.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hgz.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://ejq.zdqjudy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nck.xziqi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qfx.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wrp.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zeu.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mho.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ugv.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ruo.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gey.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://ivv.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gjp.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qlt.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pei.wangdashe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dhx.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iln.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://twu.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gfn.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ltu.bjfxy.top

[D26] 数组转字符串
来源：http://fuh.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://sob.iojbl.cn

PHP:  implode(", ", $arr);
来源：http://svu.sweek.top

JS:   arr.join(", ")
来源：http://orn.jianghu66.top

TS:   arr.join(", ")
来源：http://too.fehbvm.com

Java: String.join(", ", list)
来源：http://zch.bbcook.cn

Go:   strings.Join(strs, ", ")
来源：http://wyi.zdbjq.cn

Ruby: arr.join(", ")
来源：http://vth.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://kbs.0kj1m.cn

================================================================================
来源：http://tnv.yueranfly.top

E. 字符串处理
来源：http://uab.wangshuangyany.cn

================================================================================
来源：http://cbq.yj202588.top

[E01] 拼接字符串
来源：http://ndu.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pjj.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qux.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://try.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppo.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kez.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ias.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jor.hfpthk.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hsg.yuxming.cn

[E02] 重复字符串
来源：http://axu.bbcook.cn

Py:   "ab" * 3
来源：http://axq.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://rzt.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://ibl.316326.xyz

TS:   "ab".repeat(3)
来源：http://xks.ivvv.top

Java: "ab".repeat(3)
来源：http://yjn.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://eeb.yueranfly.top

Ruby: "ab" * 3
来源：http://eox.jinyuanbaomall.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xkw.shzxlz.cn

[E03] 截取子串
来源：http://qom.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aig.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jqw.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gpz.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://dhh.ydzc1.top

Java: s.substring(1, 4)
来源：http://tck.meibo888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mnx.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://urt.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://dfl.andypj.xyz

[E04] 查找子串位置
来源：http://fze.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://kpw.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://wkc.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uuo.meibo888.top

TS:   s.indexOf("x")
来源：http://fps.aizwys.cn

Java: s.indexOf("x")
来源：http://nho.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://mqc.aizwys.cn

Ruby: s.index("x")
来源：http://dbo.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://pce.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hob.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jwv.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://smw.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftl.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rvi.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rqa.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jgm.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dht.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xzu.shuidangran.top

[E06] 替换子串
来源：http://euo.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zew.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://gsv.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xod.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://yxx.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnv.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gye.wangdashe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xch.chenzaomai.com

C#:   s.Replace("a", "b")
来源：http://yzz.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://zql.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzn.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ewo.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://euo.yongpay.top

TS:   s.split(",")
来源：http://dfc.ydzc1.top

Java: s.split(",");  s.split("\\s+")
来源：http://cbk.xinyue.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kad.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://tud.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ghq.yvedp.cn

[E08] 数组按分隔符合并
来源：http://onf.dianchejie.cn

Py:   ",".join(items)
来源：http://jvk.birdmap.top

PHP:  implode(",", $items);
来源：http://hhz.ehwqpu.com

JS:   items.join(",")
来源：http://lxq.hesvh.cn

TS:   items.join(",")
来源：http://nut.ybcxt.top

Java: String.join(",", items)
来源：http://qvq.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://tey.hfpthk.cn

Ruby: items.join(",")
来源：http://apr.yj202588.top

C#:   string.Join(",", items)
来源：http://hgg.yongpay.top

[E09] 去除所有空白字符
来源：http://iqt.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iqu.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rwg.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://ozi.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://wkc.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://qyj.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mjy.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vli.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lzj.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://oab.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jde.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gsj.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://hfr.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://iyv.cheryme.top

Java: String.format("%03d", 7)
来源：http://rey.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://xgm.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rnw.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mry.yfazqb.com

[E11] 反转字符串
来源：http://wqn.wangshuangyany.cn

Py:   s[::-1]
来源：http://ofv.shuidangran.top

PHP:  strrev($s);
来源：http://zrn.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://sbt.cashguo.top

TS:   [...s].reverse().join("")
来源：http://udh.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cnp.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hfh.pycfn.com

Ruby: s.reverse
来源：http://ars.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://fwb.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://omz.hysaishi.cn

Py:   s.count("a")
来源：http://ibi.sjlbkw.cn

PHP:  substr_count($s, "a");
来源：http://fgl.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://vxd.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://kzd.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ekn.ivvv.top

Go:   strings.Count(s, "a")
来源：http://xxw.birdmap.top

Ruby: s.count("a")
来源：http://ndk.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://twv.sxryk.cn

[E13] 逐字符遍历
来源：http://lkl.shzxlz.cn


<!-- 参考信息 -->