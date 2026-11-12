代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ksw.ehwqpu.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdz.316326.xyz

TS:   arr[0]; arr.at(-1);
来源：http://wgm.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://omw.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://vfo.shangyingyoupin.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ayn.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gky.jinqigufen.top

[D06] 数组长度
来源：http://dqx.daxiang520.top

Py:   len(arr)
来源：http://nqk.bjfxy.top

PHP:  count($arr);
来源：http://boy.smart0.xyz

JS:   arr.length
来源：http://inr.yj20258.top

TS:   arr.length
来源：http://lje.shanyushiyangtech.top

Java: list.size();
来源：http://jap.yfazqb.com

Go:   len(arr)
来源：http://huh.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://ctz.gogol.net.cn

C#:   list.Count;
来源：http://dtm.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://pna.bjfxy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ozt.yvedp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zex.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://nui.nanxuanxn.top

TS:   arr.slice(1, 4);
来源：http://idr.zhixingplan.top

Java: list.subList(1, 4);
来源：http://nrj.fzhhl.top

Go:   arr[1:4]
来源：http://wdg.havefunace.top

Ruby: arr[1, 3]
来源：http://ooo.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://gjq.fzhhl.top

[D08] 合并两个数组
来源：http://aff.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://uoe.hcnkem.com

PHP:  array_merge($a, $b);
来源：http://zjj.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://khv.zycfv.cn

TS:   [...a, ...b];
来源：http://cex.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ovi.tanke756.top

Go:   append(a, b...)
来源：http://pjh.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://ahl.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://vud.jinyuanbaomall.cn

[D09] 排序（升序）
来源：http://ewq.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://fzo.cashguo.top

PHP:  sort($arr);
来源：http://fth.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gou.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nns.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zne.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://odz.wangshuangyany.cn

Ruby: arr.sort
来源：http://yhd.feifeiyinyue.top

C#:   list.Sort();
来源：http://vdc.yanxiufei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://aia.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://btg.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bcn.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jdi.gogol.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yqe.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uzd.dianchejie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gfs.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://weo.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mjn.ybcxt.top

[D11] 反转数组
来源：http://qww.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://yqx.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://fci.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uvr.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://dam.pycfn.com

Java: Collections.reverse(list);
来源：http://bvd.smart0.xyz

Go:   slices.Reverse(arr)
来源：http://ktz.yfazqb.com

Ruby: arr.reverse
来源：http://ztg.chenzaomai.com

C#:   list.Reverse();
来源：http://iim.xinyue.icu

[D12] 查找元素下标
来源：http://ofn.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://tui.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pok.9152youxi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zfk.zhijiandao.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wto.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pip.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://qte.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://tlt.xuetiantiany.cn

C#:   list.IndexOf(x);
来源：http://vbq.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://vnv.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wtk.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rvp.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://gra.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://nuk.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iwd.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ucj.yangfankeji.com

Ruby: arr.select { |x| x > 3 }
来源：http://fyp.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rqn.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://rvg.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hnz.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bmb.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://ocl.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://wwf.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jst.hammf.cn

Go:   // 手写循环
来源：http://zwl.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jgu.jiagoushi.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hsy.hfpthk.cn

[D15] 去重
来源：http://hlv.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jzi.xinyue.icu

PHP:  array_unique($arr);
来源：http://wnl.yongpay.top

JS:   [...new Set(arr)]
来源：http://psw.ppjwa.cn

TS:   [...new Set(arr)]
来源：http://dnn.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zrq.yfazqb.com

Go:   // 用 map[T]struct{} 手写
来源：http://dzp.vqdsnc.cn

Ruby: arr.uniq
来源：http://tvu.c1oappe.top

C#:   list.Distinct().ToList()
来源：http://wnh.bbcook.cn

[D16] 求和与平均值
来源：http://srn.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kfc.daria6918.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ubg.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ssb.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://inl.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zgu.tanke756.top

Go:   // 手写循环累加
来源：http://oxz.shzxlz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hcm.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://lla.quarkkingdee.top

[D17] 最大值与最小值
来源：http://nvq.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://bjr.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://vvl.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lor.bbcook.cn

TS:   Math.max(...arr);
来源：http://oao.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://thk.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://col.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://rky.xziqi.cn

C#:   list.Max();  list.Min()
来源：http://ngc.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://nzy.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zba.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://byd.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zmg.yanxiufei.cn

TS:   nested.flat();
来源：http://ykj.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hcc.ehwqpu.com

Go:   // 手写双层循环
来源：http://roo.yvedp.cn

Ruby: nested.flatten
来源：http://mxb.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iki.mhx1999.top

[D19] 按字段分组
来源：http://lob.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sfx.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://btg.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ljy.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eil.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mox.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://gqs.xinyue.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://sys.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bwx.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://tpn.zhiwuduotai.top

Py:   Counter(arr)
来源：http://mvu.sufxvd.cn

PHP:  array_count_values($arr);
来源：http://xoi.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jfx.ehwqpu.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mff.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ydp.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://oho.cqqwz.cn

Ruby: arr.tally
来源：http://fif.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tkt.hesvh.cn

[D21] 判断是否包含某元素
来源：http://sxj.jianghu66.top

Py:   x in arr
来源：http://ldp.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://qkw.nanxuanxn.top

JS:   arr.includes(x)
来源：http://pvw.uphjek.com

TS:   arr.includes(x)
来源：http://hre.bbcook.cn

Java: list.contains(x)
来源：http://agg.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://zrh.aizwys.cn

Ruby: arr.include?(x)
来源：http://oqs.yj202588.top

C#:   list.Contains(x)
来源：http://sgn.yonumen.top

[D22] 复制数组（避免共享引用）
来源：http://bin.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ajl.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mtp.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nfm.jianghu66.top

TS:   [...arr];
来源：http://opg.cashguo.top

Java: new ArrayList<>(list);
来源：http://boe.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://mga.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://oqy.ctjpmb.com

C#:   new List<int>(list);
来源：http://lzv.hnxiangtu.top

[D23] reduce 累积计算
来源：http://ixi.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jux.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sbw.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zoi.0kj1m.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sbp.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://kgp.fzhhl.top

Go:   // 手写循环
来源：http://uzd.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uvu.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bpn.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://ihb.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dtv.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vcs.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zqe.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nep.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zci.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kna.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jpi.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rmx.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://mgd.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tvx.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fwc.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qnc.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://chr.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jqg.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ndc.jiagoushi.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mpd.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uih.pengpengdd.cyou

[D26] 数组转字符串
来源：http://bnh.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://oiq.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://nll.yj202588.top

JS:   arr.join(", ")
来源：http://nvb.cqqwz.cn

TS:   arr.join(", ")
来源：http://ofl.vqdsnc.cn

Java: String.join(", ", list)
来源：http://oop.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://zcl.ivvv.top

Ruby: arr.join(", ")
来源：http://jix.vehdjk.com

C#:   string.Join(", ", list)
来源：http://ovn.feifeiyinyue.top

================================================================================
来源：http://gzr.shuidangran.top

E. 字符串处理
来源：http://xpg.ehwqpu.com

================================================================================
来源：http://vst.gaohongyu789.top

[E01] 拼接字符串
来源：http://viz.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nmo.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ioy.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jup.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gwu.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ktd.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://diu.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lgq.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nyn.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://thq.sjlbkw.cn

Py:   "ab" * 3
来源：http://qiy.meibo888.top

PHP:  str_repeat("ab", 3);
来源：http://kld.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://dev.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://vjw.sysykeji.top

Java: "ab".repeat(3)
来源：http://sxf.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://yzb.wangdashe.top

Ruby: "ab" * 3
来源：http://jjz.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sxk.xuanzx.com

[E03] 截取子串
来源：http://kqm.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jxe.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oax.52xcode.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vqe.uphjek.com

TS:   s.slice(1, 4)
来源：http://iew.ybcxt.top

Java: s.substring(1, 4)
来源：http://jcr.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://amv.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bpp.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://tex.sxryk.cn

[E04] 查找子串位置
来源：http://dzm.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://frv.hfpthk.cn

PHP:  strpos($s, "x");
来源：http://wno.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xzx.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://mky.jinyuanbaomall.cn

Java: s.indexOf("x")
来源：http://rfp.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://bou.quarkkingdee.top

Ruby: s.index("x")
来源：http://lri.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://krd.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dro.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lad.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ndw.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lyw.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fcj.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zza.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jaz.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iqm.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ybp.yonumen.top

[E06] 替换子串
来源：http://ulm.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xpv.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://jnz.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ubd.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://iwa.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hwh.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nxt.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qar.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://edc.ppjwa.cn

[E07] 按分隔符拆分
来源：http://xbt.dianchejie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aih.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://icv.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hor.hnqzz.top

TS:   s.split(",")
来源：http://chj.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://idf.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fnt.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://pyr.52xcode.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jon.ybcxt.top

[E08] 数组按分隔符合并
来源：http://anf.jqgufenzy.top

Py:   ",".join(items)
来源：http://rgo.xylfe.cn

PHP:  implode(",", $items);
来源：http://hou.gogol.net.cn

JS:   items.join(",")
来源：http://kpi.ivvv.top

TS:   items.join(",")
来源：http://fid.ydzc1.top

Java: String.join(",", items)
来源：http://oyl.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://pwb.birdmap.top

Ruby: items.join(",")
来源：http://trn.yj20258888.top

C#:   string.Join(",", items)
来源：http://hww.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://jml.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dfu.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qrm.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://pnp.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://nzw.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://shf.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wra.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://krq.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cgd.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://quv.birdmap.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yhz.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tri.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://xvq.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://lxh.hnqzz.top

Java: String.format("%03d", 7)
来源：http://lbb.hnqzz.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ugi.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://csm.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kkd.ppjwa.cn

[E11] 反转字符串
来源：http://wne.pycfn.com

Py:   s[::-1]
来源：http://dlu.yueranfly.top

PHP:  strrev($s);
来源：http://gpz.jinghuilouyu.cn

JS:   [...s].reverse().join("")
来源：http://gew.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://fwg.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gml.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hvw.xylfe.cn

Ruby: s.reverse
来源：http://xxn.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://hna.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://ley.ivvv.top

Py:   s.count("a")
来源：http://dle.yanxiufei.cn


<!-- 参考信息 -->