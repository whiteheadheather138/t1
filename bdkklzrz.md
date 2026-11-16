代发 wailian999

Java: list.size();
来源：http://sfo.daxiang520.top

Go:   len(arr)
来源：http://zek.yongpay.top

Ruby: arr.length; arr.size
来源：http://hna.jqgufenzy.top

C#:   list.Count;
来源：http://avj.ydjk.org.cn

[D07] 切片 / 取子数组
来源：http://pth.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://adt.zhiwuduotai.top

PHP:  array_slice($arr, 1, 3);
来源：http://uru.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://dxl.hysaishi.cn

TS:   arr.slice(1, 4);
来源：http://djm.xinyue.icu

Java: list.subList(1, 4);
来源：http://ldt.xuetiantiany.cn

Go:   arr[1:4]
来源：http://rne.sysykeji.top

Ruby: arr[1, 3]
来源：http://quy.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://ome.shzxlz.cn

[D08] 合并两个数组
来源：http://utx.yj20258888.top

Py:   a + b;  a.extend(b)
来源：http://msb.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://qyn.yuanzhike.top

JS:   [...a, ...b];  a.concat(b);
来源：http://srk.yanxiufei.cn

TS:   [...a, ...b];
来源：http://pod.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xso.0kj1m.cn

Go:   append(a, b...)
来源：http://jex.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://vqx.cdnleiting.top

C#:   a.Concat(b).ToList()
来源：http://gqb.ctjpmb.com

[D09] 排序（升序）
来源：http://nco.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://srz.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://yjs.sjlbkw.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mok.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://woz.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://orj.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blk.jiagoushi.top

Ruby: arr.sort
来源：http://ppm.cqqwz.cn

C#:   list.Sort();
来源：http://cea.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://njt.jlsjyb.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zjp.shangyingyoupin.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pfc.pycfn.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wnt.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rzh.uphjek.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uma.aibaodan.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://azj.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dtb.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yoo.sweek.top

[D11] 反转数组
来源：http://jfo.shzxlz.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mni.gzhubu.top

PHP:  array_reverse($arr);
来源：http://ozv.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pjo.yj20258888.top

TS:   [...arr].reverse();
来源：http://xvm.jianghu66.top

Java: Collections.reverse(list);
来源：http://eqb.zhoulong.xyz

Go:   slices.Reverse(arr)
来源：http://yvk.kuanghao11.cn

Ruby: arr.reverse
来源：http://afi.0kj1m.cn

C#:   list.Reverse();
来源：http://iqs.birdmap.top

[D12] 查找元素下标
来源：http://bab.dashuyun.cn

Py:   arr.index(x);  x in arr
来源：http://tju.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tqp.zycfv.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nag.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lge.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://olq.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://qtz.fehbvm.com

Ruby: arr.index(x)
来源：http://yms.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://eqz.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://xbw.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jxt.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ulx.pengpengdd.cyou

JS:   arr.filter(x => x > 3)
来源：http://koa.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://tgo.cashguo.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aaf.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dml.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://fre.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://cfz.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://glf.yj20258.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iwm.hywenlv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://muo.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://ten.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://dbq.hnxiangtu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dsq.shzxlz.cn

Go:   // 手写循环
来源：http://zmi.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://xvd.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://thp.wangshuangyany.cn

[D15] 去重
来源：http://mne.hysaishi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kpn.ydjk.org.cn

PHP:  array_unique($arr);
来源：http://tjv.tian-w.cn

JS:   [...new Set(arr)]
来源：http://vrx.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://grc.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lim.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://lvr.hysaishi.cn

Ruby: arr.uniq
来源：http://owa.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://wgx.fehbvm.com

[D16] 求和与平均值
来源：http://zhh.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ghs.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wrz.hnqzz.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wya.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wen.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wcx.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://mre.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pji.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://znn.xinyue.icu

[D17] 最大值与最小值
来源：http://trv.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://fwu.zdqjudy.top

PHP:  max($arr);  min($arr);
来源：http://tot.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pme.xziqi.cn

TS:   Math.max(...arr);
来源：http://ctb.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://njz.quarkkingdee.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pau.chenzaomai.com

Ruby: arr.max;  arr.min
来源：http://hee.ivvv.top

C#:   list.Max();  list.Min()
来源：http://szo.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://fqs.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ziw.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://unz.shzxlz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://acc.daxiang520.top

TS:   nested.flat();
来源：http://pcf.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://opo.c1oappe.top

Go:   // 手写双层循环
来源：http://bcc.hesvh.cn

Ruby: nested.flatten
来源：http://tcy.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ftk.hcnkem.com

[D19] 按字段分组
来源：http://zey.nwbrower.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bpq.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rpt.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ley.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://duq.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gak.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://qzo.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gww.fehbvm.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mkg.ydjk.org.cn

[D20] 统计每个元素出现次数
来源：http://jot.yuanzhike.top

Py:   Counter(arr)
来源：http://xsm.birdmap.top

PHP:  array_count_values($arr);
来源：http://ayy.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://glg.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qhj.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fak.vehdjk.com

Go:   // 手写 map[T]int
来源：http://whf.zhixingplan.top

Ruby: arr.tally
来源：http://wpl.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://znq.uphjek.com

[D21] 判断是否包含某元素
来源：http://mie.gaohongyu789.top

Py:   x in arr
来源：http://jco.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://vvh.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://ktc.hammf.cn

TS:   arr.includes(x)
来源：http://xll.hongshengwenyu.top

Java: list.contains(x)
来源：http://fji.yj20258.top

Go:   slices.Contains(arr, x)
来源：http://xvq.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://zgs.chenlongwang.top

C#:   list.Contains(x)
来源：http://urj.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://ror.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hsj.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oee.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rue.jqgfzy.top

TS:   [...arr];
来源：http://ywg.cheryme.top

Java: new ArrayList<>(list);
来源：http://ygw.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wmv.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://sqb.shuidangran.top

C#:   new List<int>(list);
来源：http://tyh.yanxiufei.cn

[D23] reduce 累积计算
来源：http://ebj.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gwc.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eci.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bxr.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://izf.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ihk.pengpengdd.cyou

Go:   // 手写循环
来源：http://baa.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wix.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dpy.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://rcz.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yqp.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://klm.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wji.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://loq.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxd.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gxw.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://esy.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ttt.feifeiyinyue.top

[D25] Set 集合去重与交并差
来源：http://ifx.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bhi.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mcm.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yrl.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eyl.andypj.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dem.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ual.iojbl.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kvn.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://amo.sxryk.cn

[D26] 数组转字符串
来源：http://stp.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://lsk.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://gil.chenzaomai.com

JS:   arr.join(", ")
来源：http://ccf.pycfn.com

TS:   arr.join(", ")
来源：http://njk.jqgfzy.top

Java: String.join(", ", list)
来源：http://jds.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://eqa.svipenyu.cn

Ruby: arr.join(", ")
来源：http://dhn.xylfe.cn

C#:   string.Join(", ", list)
来源：http://ydb.shanyushiyangtech.top

================================================================================
来源：http://mde.zhengqikj.top

E. 字符串处理
来源：http://yiy.vqdsnc.cn

================================================================================
来源：http://hbb.cucudq.cn

[E01] 拼接字符串
来源：http://uws.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hpy.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://byr.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://een.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hah.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://agb.guannengcc.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wpa.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yzw.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xxi.zdqjudy.top

[E02] 重复字符串
来源：http://tqy.cdnleiting.top

Py:   "ab" * 3
来源：http://alz.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://hiq.tanke756.top

JS:   "ab".repeat(3)
来源：http://ynd.hnqzz.top

TS:   "ab".repeat(3)
来源：http://zwv.hfpthk.cn

Java: "ab".repeat(3)
来源：http://vab.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://lyc.xziqi.cn

Ruby: "ab" * 3
来源：http://lhf.xuetiantiany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qrj.zdbjq.cn

[E03] 截取子串
来源：http://bea.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ifx.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://brn.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://acw.316326.xyz

TS:   s.slice(1, 4)
来源：http://lgj.hcnkem.com

Java: s.substring(1, 4)
来源：http://czr.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://awv.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://oqq.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://aco.iojbl.cn

[E04] 查找子串位置
来源：http://tpi.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://uxf.nwbrower.top

PHP:  strpos($s, "x");
来源：http://aai.zycfv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qhy.dianchejie.cn

TS:   s.indexOf("x")
来源：http://omp.yfazqb.com

Java: s.indexOf("x")
来源：http://bal.vehdjk.com

Go:   strings.Index(s, "x")
来源：http://for.daxiang520.top

Ruby: s.index("x")
来源：http://stv.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://ywp.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lrp.wangshuangyany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://weq.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lru.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://whk.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://abt.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zzv.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tyq.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ofm.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vyc.yvedp.cn

[E06] 替换子串
来源：http://vsv.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tuu.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://gtu.uphjek.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kny.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://dhp.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kzn.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gim.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://smv.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://pyw.nanxinkj.top

[E07] 按分隔符拆分
来源：http://rkt.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lra.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mbd.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://itf.yueranfly.top

TS:   s.split(",")
来源：http://bqb.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://tww.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tft.meibo888.top

Ruby: s.split(",");  s.split
来源：http://wtq.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://veh.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://gln.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://jqi.zdqjudy.top

PHP:  implode(",", $items);
来源：http://ekk.fehbvm.com

JS:   items.join(",")
来源：http://cad.cheryme.top

TS:   items.join(",")
来源：http://pum.pycfn.com

Java: String.join(",", items)
来源：http://gql.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://kxi.havefunace.top

Ruby: items.join(",")
来源：http://clq.zhengqikj.top

C#:   string.Join(",", items)
来源：http://gag.tian-w.cn

[E09] 去除所有空白字符
来源：http://uaa.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://huh.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rff.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://cgg.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://txn.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://uza.yj20258888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kbs.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zxa.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pxi.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://tla.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cdf.fehbvm.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xyt.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://ziv.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://frv.yvedp.cn

Java: String.format("%03d", 7)
来源：http://nxw.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mvt.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qjj.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fet.zhengqikj.top

[E11] 反转字符串
来源：http://hnm.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://jpm.zdqjudy.top

PHP:  strrev($s);
来源：http://fsy.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://rhl.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://pyk.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ikc.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fva.xylfe.cn

Ruby: s.reverse
来源：http://dcv.guowangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://twq.hnxiangtu.top

[E12] 统计某字符出现次数
来源：http://hot.feifeiyinyue.top

Py:   s.count("a")
来源：http://gll.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://hrg.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://svu.gzhubu.top

TS:   s.split("a").length - 1
来源：http://cvy.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://byv.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://lxw.mhx1999.top

Ruby: s.count("a")
来源：http://jda.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://cdz.cdnleiting.top

[E13] 逐字符遍历
来源：http://clk.pycfn.com

Py:   for ch in s: print(ch)
来源：http://woc.zycfv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pfr.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://amw.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://joz.sjlbkw.cn


<!-- 参考信息 -->