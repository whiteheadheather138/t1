代发 wailian999

Java: list.size();
来源：http://ghu.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://ihq.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://yqm.zhijiandao.cn

C#:   list.Count;
来源：http://sdz.yueranfly.top

[D07] 切片 / 取子数组
来源：http://txh.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ndj.hnxiangtu.top

PHP:  array_slice($arr, 1, 3);
来源：http://fgv.aizwys.cn

JS:   arr.slice(1, 4);
来源：http://leu.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://swd.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://tof.hfpthk.cn

Go:   arr[1:4]
来源：http://hxx.iojbl.cn

Ruby: arr[1, 3]
来源：http://mnn.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://faa.hysaishi.cn

[D08] 合并两个数组
来源：http://thq.iojbl.cn

Py:   a + b;  a.extend(b)
来源：http://cch.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://ngx.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tvv.nanxuanxn.top

TS:   [...a, ...b];
来源：http://jmh.jinghuilouyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://stv.aizwys.cn

Go:   append(a, b...)
来源：http://xdh.ywan-chungtsiang.top

Ruby: a + b;  a.concat(b)
来源：http://woe.xingfuxueyuan.xyz

C#:   a.Concat(b).ToList()
来源：http://cnr.sysykeji.top

[D09] 排序（升序）
来源：http://rri.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://nrc.yueranfly.top

PHP:  sort($arr);
来源：http://dsu.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vwb.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://adi.aibaodan.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ecj.haohaochexian.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gmy.52xcode.cn

Ruby: arr.sort
来源：http://thv.zdbjq.cn

C#:   list.Sort();
来源：http://tie.sxryk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://dbb.chenzaomai.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ydx.aizwys.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aen.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zhp.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ggi.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qjx.hammf.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://var.birdmap.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://obi.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xkp.fengsongda.top

[D11] 反转数组
来源：http://oyf.feifeiyinyue.top

Py:   arr[::-1];  arr.reverse()
来源：http://oxq.316326.xyz

PHP:  array_reverse($arr);
来源：http://wmw.sxryk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://odu.fengsongda.top

TS:   [...arr].reverse();
来源：http://axs.fengsongda.top

Java: Collections.reverse(list);
来源：http://rnr.hammf.cn

Go:   slices.Reverse(arr)
来源：http://nqu.zhijiandao.cn

Ruby: arr.reverse
来源：http://onz.cashguo.top

C#:   list.Reverse();
来源：http://fvu.0kj1m.cn

[D12] 查找元素下标
来源：http://hhj.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://zxr.zycfv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mnn.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikj.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nsa.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sfv.52xcode.cn

Go:   slices.Index(arr, x)
来源：http://pis.jiagoushi.top

Ruby: arr.index(x)
来源：http://scm.wangdashe.top

C#:   list.IndexOf(x);
来源：http://ykk.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://mba.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qbn.jlsjyb.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tew.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://wni.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://hvw.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oaz.jiagoushi.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mrr.hnqzz.top

Ruby: arr.select { |x| x > 3 }
来源：http://ivf.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ywh.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://rfq.52xcode.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pqr.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ric.gogol.net.cn

JS:   arr.map(x => x * 2)
来源：http://rxb.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://efa.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xmz.gaohongyu789.top

Go:   // 手写循环
来源：http://lww.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://olr.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://guc.tanke756.top

[D15] 去重
来源：http://gnn.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mtw.hcnkem.com

PHP:  array_unique($arr);
来源：http://dyx.bbcook.cn

JS:   [...new Set(arr)]
来源：http://kcu.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://bim.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ahj.smart0.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://rzd.bjfxy.top

Ruby: arr.uniq
来源：http://cnj.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://psg.cashguo.top

[D16] 求和与平均值
来源：http://mdk.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jeu.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qkf.jlsjyb.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rdu.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zzn.fehbvm.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://flw.yj202588.top

Go:   // 手写循环累加
来源：http://xzo.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://irj.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://ylo.fehbvm.com

[D17] 最大值与最小值
来源：http://yok.jinqigfzy.top

Py:   max(arr);  min(arr)
来源：http://lft.hesvh.cn

PHP:  max($arr);  min($arr);
来源：http://zdm.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nwe.tarul.cn

TS:   Math.max(...arr);
来源：http://jkg.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wbv.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://noy.yj202588.top

Ruby: arr.max;  arr.min
来源：http://yyd.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://yew.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://ryp.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hce.ivvv.top

PHP:  array_merge(...$nested);
来源：http://qnq.daria6918.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gkp.chenjidiqi.icu

TS:   nested.flat();
来源：http://sef.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zmn.tanke756.top

Go:   // 手写双层循环
来源：http://olt.kuanghao11.cn

Ruby: nested.flatten
来源：http://zcw.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://drw.yanxiufei.cn

[D19] 按字段分组
来源：http://pwr.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vxh.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nca.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gnp.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eqe.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wfa.tanke756.top

Go:   // 手写 map[string][]T
来源：http://thy.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kjj.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zod.tanke756.top

[D20] 统计每个元素出现次数
来源：http://nhp.zdbjq.cn

Py:   Counter(arr)
来源：http://gew.sweek.top

PHP:  array_count_values($arr);
来源：http://snu.guowangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whq.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsh.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tob.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://iwj.fanxiaobao.xyz

Ruby: arr.tally
来源：http://dnp.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nna.sufxvd.cn

[D21] 判断是否包含某元素
来源：http://cyz.hysaishi.cn

Py:   x in arr
来源：http://kvg.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://bgz.hesvh.cn

JS:   arr.includes(x)
来源：http://cvu.epnwcf.com

TS:   arr.includes(x)
来源：http://wdz.sweek.top

Java: list.contains(x)
来源：http://kib.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://ghh.fktsv.cn

Ruby: arr.include?(x)
来源：http://uzs.ivvv.top

C#:   list.Contains(x)
来源：http://etw.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://thj.jianghu66.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rjz.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://osf.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://arx.sjlbkw.cn

TS:   [...arr];
来源：http://cux.ydzc1.top

Java: new ArrayList<>(list);
来源：http://rbi.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dsd.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://ngm.fktsv.cn

C#:   new List<int>(list);
来源：http://hmo.ydzc1.top

[D23] reduce 累积计算
来源：http://bhd.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wlu.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mod.tian-w.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eaa.316326.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dxj.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://izr.smart0.xyz

Go:   // 手写循环
来源：http://jpg.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bnn.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://igz.yfazqb.com

[D24] 字典 / Map 基本操作
来源：http://dka.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dsr.shuidangran.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lhx.hnqzz.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://faa.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://euk.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qhy.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hmc.fanxiaobao.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zow.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gzh.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://vvd.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qpi.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rhq.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lvy.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kof.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mov.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pns.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jxk.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pfz.zhengqikj.top

[D26] 数组转字符串
来源：http://vpt.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://geh.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://ito.cqqwz.cn

JS:   arr.join(", ")
来源：http://juo.wangdashe.top

TS:   arr.join(", ")
来源：http://uug.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://blv.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://hri.bjfxy.top

Ruby: arr.join(", ")
来源：http://ftt.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://sei.tanke756.top

================================================================================
来源：http://ddx.sjlbkw.cn

E. 字符串处理
来源：http://rkp.ehwqpu.com

================================================================================
来源：http://xeq.sweek.top

[E01] 拼接字符串
来源：http://pju.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ulg.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jae.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ppq.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bkj.zycfv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bcm.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://thq.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://frf.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lft.xuanzx.com

[E02] 重复字符串
来源：http://rhk.tanke756.top

Py:   "ab" * 3
来源：http://fqx.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://tfu.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://ijc.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://zjm.fzhhl.top

Java: "ab".repeat(3)
来源：http://eza.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://zrj.svipenyu.cn

Ruby: "ab" * 3
来源：http://tkj.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jcl.chenzaomai.com

[E03] 截取子串
来源：http://blq.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sgl.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iac.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yno.52xcode.cn

TS:   s.slice(1, 4)
来源：http://bhm.jyoumei.cn

Java: s.substring(1, 4)
来源：http://sau.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ezt.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://dkr.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://thf.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://tle.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://xus.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://blf.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rew.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://ruv.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://kjf.yongpay.top

Go:   strings.Index(s, "x")
来源：http://ubd.yj20258888.top

Ruby: s.index("x")
来源：http://ksh.yj20258888.top

C#:   s.IndexOf("x")
来源：http://uae.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hvl.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tfa.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mbp.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sch.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hbm.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gia.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nbc.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://knq.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qzb.zycfv.cn

[E06] 替换子串
来源：http://tng.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gmn.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://psa.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bab.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://abg.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yon.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gqd.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zhj.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://rcz.gogol.net.cn

[E07] 按分隔符拆分
来源：http://byx.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ofw.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qty.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ztx.ydjk.org.cn

TS:   s.split(",")
来源：http://qad.ydjk.org.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uxe.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hjz.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://gfh.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hlv.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://lje.yonumen.top

Py:   ",".join(items)
来源：http://nzp.tanke756.top

PHP:  implode(",", $items);
来源：http://sef.xinyue.icu

JS:   items.join(",")
来源：http://reh.snrcjt.cn

TS:   items.join(",")
来源：http://zlj.gaohongyu789.top

Java: String.join(",", items)
来源：http://lkk.52xcode.cn

Go:   strings.Join(items, ",")
来源：http://sxo.xuanzx.com

Ruby: items.join(",")
来源：http://kwt.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://yus.ydzc1.top

[E09] 去除所有空白字符
来源：http://caq.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://djf.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rvl.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://utk.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://ukz.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://liv.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bbm.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://dkf.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gnq.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://qet.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ioy.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sbs.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://mfg.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://qlj.xziqi.cn

Java: String.format("%03d", 7)
来源：http://ept.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://vnb.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://smq.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cwy.zhixingplan.top

[E11] 反转字符串
来源：http://mrj.jqgufenzy.top

Py:   s[::-1]
来源：http://fal.zdbjq.cn

PHP:  strrev($s);
来源：http://civ.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://qtt.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://arq.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jwb.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hko.epnwcf.com

Ruby: s.reverse
来源：http://xyd.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://byt.fengsongda.top

[E12] 统计某字符出现次数
来源：http://rvm.yongpay.top

Py:   s.count("a")
来源：http://ubh.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://vhr.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://stn.bbcook.cn

TS:   s.split("a").length - 1
来源：http://psw.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cpj.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://yfp.ydzc1.top

Ruby: s.count("a")
来源：http://kxg.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://xyx.ctjpmb.com

[E13] 逐字符遍历
来源：http://qpc.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://gto.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://plz.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ohv.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ptv.zhijiandao.cn


<!-- 参考信息 -->