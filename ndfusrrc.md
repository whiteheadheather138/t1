代发 wailian999

Java: list.size();
来源：http://vde.shzxlz.cn

Go:   len(arr)
来源：http://cez.ppjwa.cn

Ruby: arr.length; arr.size
来源：http://utj.sufxvd.cn

C#:   list.Count;
来源：http://qib.gogol.net.cn

[D07] 切片 / 取子数组
来源：http://wdq.sweek.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lcj.ydzc1.top

PHP:  array_slice($arr, 1, 3);
来源：http://stt.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://ddo.hywenlv.cn

TS:   arr.slice(1, 4);
来源：http://lgc.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://tdt.gogol.net.cn

Go:   arr[1:4]
来源：http://rao.hnxiangtu.top

Ruby: arr[1, 3]
来源：http://hme.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://mpt.yfazqb.com

[D08] 合并两个数组
来源：http://cdc.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://hew.ybcxt.top

PHP:  array_merge($a, $b);
来源：http://cku.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://egq.svipenyu.cn

TS:   [...a, ...b];
来源：http://cjp.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sdo.nwbrower.top

Go:   append(a, b...)
来源：http://jhs.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://aue.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://chs.zhoulong.xyz

[D09] 排序（升序）
来源：http://wbq.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://zgo.sxryk.cn

PHP:  sort($arr);
来源：http://uuy.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rcp.gogol.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://igc.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cuj.meibo888.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://apv.0kj1m.cn

Ruby: arr.sort
来源：http://thn.yangfankeji.com

C#:   list.Sort();
来源：http://ajo.9152youxi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gaj.jiagoushi.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xhz.gotoacloud.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://svy.birdmap.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nrs.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fwd.ybcxt.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ksp.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qno.kuanghao11.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wsl.sufxvd.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vww.andypj.xyz

[D11] 反转数组
来源：http://fdv.iojbl.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ptq.dashuyun.cn

PHP:  array_reverse($arr);
来源：http://jeh.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qri.fanxiaobao.xyz

TS:   [...arr].reverse();
来源：http://pdt.hesvh.cn

Java: Collections.reverse(list);
来源：http://keo.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://qbp.jqgfzy.top

Ruby: arr.reverse
来源：http://mzn.havefunace.top

C#:   list.Reverse();
来源：http://nun.gotoacloud.top

[D12] 查找元素下标
来源：http://fdj.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://tra.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lzd.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oco.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cel.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ygo.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://vlq.ivvv.top

Ruby: arr.index(x)
来源：http://vez.ppjwa.cn

C#:   list.IndexOf(x);
来源：http://vqj.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://ydz.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dln.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lpw.ywan-chungtsiang.top

JS:   arr.filter(x => x > 3)
来源：http://ynx.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://bgc.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://snt.cashguo.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cpp.hnxiangtu.top

Ruby: arr.select { |x| x > 3 }
来源：http://ocf.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ndu.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://btp.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://emy.hnqzz.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nwt.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://oac.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://pgd.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://rxx.sufxvd.cn

Go:   // 手写循环
来源：http://njy.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://otk.tian-w.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sit.xinyue.icu

[D15] 去重
来源：http://aag.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lvz.zhijiandao.cn

PHP:  array_unique($arr);
来源：http://uvh.jqgufenzy.top

JS:   [...new Set(arr)]
来源：http://lfq.redwolf501.top

TS:   [...new Set(arr)]
来源：http://poi.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vub.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://dpb.jqgfzy.top

Ruby: arr.uniq
来源：http://wim.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://nza.xingfuxueyuan.xyz

[D16] 求和与平均值
来源：http://ysu.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xzu.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kul.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hig.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bky.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://suz.zdbjq.cn

Go:   // 手写循环累加
来源：http://txu.zhongyouzk.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bay.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://cod.yanxiufei.cn

[D17] 最大值与最小值
来源：http://asz.dashuyun.cn

Py:   max(arr);  min(arr)
来源：http://yqi.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://wqz.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzl.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://ulb.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ojj.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eoa.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://sof.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://frd.sufxvd.cn

[D18] 扁平化嵌套数组
来源：http://cae.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nod.guowangkeji.top

PHP:  array_merge(...$nested);
来源：http://kjf.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mlw.jianghu66.top

TS:   nested.flat();
来源：http://irs.tianlin.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gsf.xylfe.cn

Go:   // 手写双层循环
来源：http://hpe.ivvv.top

Ruby: nested.flatten
来源：http://fll.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gjr.hfpthk.cn

[D19] 按字段分组
来源：http://yir.hongshengwenyu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://czb.gaohongyu789.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://goh.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rso.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://esb.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qxc.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://tuh.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyh.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izr.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://ruk.hywenlv.cn

Py:   Counter(arr)
来源：http://sib.zhixingplan.top

PHP:  array_count_values($arr);
来源：http://eiu.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vki.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mpp.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ybo.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://yrh.ppjwa.cn

Ruby: arr.tally
来源：http://avt.316326.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jab.yj20258.top

[D21] 判断是否包含某元素
来源：http://ick.shzxlz.cn

Py:   x in arr
来源：http://hzg.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://hjl.svipenyu.cn

JS:   arr.includes(x)
来源：http://zyp.bjfxy.top

TS:   arr.includes(x)
来源：http://gxv.zhijiandao.cn

Java: list.contains(x)
来源：http://skv.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://dpr.ybcxt.top

Ruby: arr.include?(x)
来源：http://vln.tanke756.top

C#:   list.Contains(x)
来源：http://brr.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://pif.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mij.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://olm.feifeiyinyue.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mbs.chenlongwang.top

TS:   [...arr];
来源：http://qcd.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://lyj.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ggd.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://uec.xuanzx.com

C#:   new List<int>(list);
来源：http://iuh.ppjwa.cn

[D23] reduce 累积计算
来源：http://ugq.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ucx.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zer.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xpz.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skh.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gft.wangdashe.top

Go:   // 手写循环
来源：http://woz.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bvg.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kvm.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://xne.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://khb.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ezj.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pri.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://aks.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nfu.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://izc.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ooy.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ria.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://lit.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uib.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kqn.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dzh.zhixingplan.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lyq.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ykh.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fim.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tsi.ivvv.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://niw.hfpthk.cn

[D26] 数组转字符串
来源：http://rir.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://ehr.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://duc.zhijiandao.cn

JS:   arr.join(", ")
来源：http://nxv.jqgufenzy.top

TS:   arr.join(", ")
来源：http://pki.yuanzhike.top

Java: String.join(", ", list)
来源：http://pdq.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://hqh.jqgfzy.top

Ruby: arr.join(", ")
来源：http://egs.jinqigufen.top

C#:   string.Join(", ", list)
来源：http://zlb.smart0.xyz

================================================================================
来源：http://vhg.yfazqb.com

E. 字符串处理
来源：http://ags.zhengqikj.top

================================================================================
来源：http://kay.sysykeji.top

[E01] 拼接字符串
来源：http://bou.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vio.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mtx.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kwx.smart0.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pxg.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brl.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://emj.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wfa.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fqz.shuidangran.top

[E02] 重复字符串
来源：http://qon.hesvh.cn

Py:   "ab" * 3
来源：http://vpg.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://ffx.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://haa.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://lre.vehdjk.com

Java: "ab".repeat(3)
来源：http://rmf.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://isv.yfazqb.com

Ruby: "ab" * 3
来源：http://bsn.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ntw.haohaochexian.top

[E03] 截取子串
来源：http://jzg.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cnb.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ksp.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://btw.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://mbu.hcnkem.com

Java: s.substring(1, 4)
来源：http://lxg.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xwg.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://utc.cheryme.top

C#:   s.Substring(1, 3)
来源：http://qxd.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://qhd.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://fyf.uphjek.com

PHP:  strpos($s, "x");
来源：http://rcs.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ctd.zdbjq.cn

TS:   s.indexOf("x")
来源：http://fjq.birdmap.top

Java: s.indexOf("x")
来源：http://lfi.ehwqpu.com

Go:   strings.Index(s, "x")
来源：http://fuj.yj202588.top

Ruby: s.index("x")
来源：http://lzf.tarul.cn

C#:   s.IndexOf("x")
来源：http://okx.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yqu.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dzk.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://len.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nox.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fik.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xih.jinyuanbaomall.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yjr.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lif.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zvi.zhijiandao.cn

[E06] 替换子串
来源：http://lkt.fzhhl.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://puv.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://ihv.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqy.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://ewd.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xaz.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://shn.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ytp.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://zvk.yj20258888.top

[E07] 按分隔符拆分
来源：http://tvy.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nos.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ylm.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wft.fzhhl.top

TS:   s.split(",")
来源：http://olm.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://ytc.jyoumei.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iyo.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://ksy.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yrc.andypj.xyz

[E08] 数组按分隔符合并
来源：http://sjy.hcnkem.com

Py:   ",".join(items)
来源：http://cdd.ehwqpu.com

PHP:  implode(",", $items);
来源：http://eha.jyoumei.cn

JS:   items.join(",")
来源：http://vnv.hammf.cn

TS:   items.join(",")
来源：http://mgb.nwbrower.top

Java: String.join(",", items)
来源：http://kez.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://ywo.yuxming.cn

Ruby: items.join(",")
来源：http://bhi.meibo888.top

C#:   string.Join(",", items)
来源：http://kij.hcnkem.com

[E09] 去除所有空白字符
来源：http://gcb.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bak.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wpb.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://fyx.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://mfx.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://afh.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://smu.wangdashe.top

Ruby: s.gsub(/\s+/, "")
来源：http://bsw.sysykeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dsc.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://rrc.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qpv.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dkt.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://aqs.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://xqr.yj20258888.top

Java: String.format("%03d", 7)
来源：http://tqz.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://prc.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://giu.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ubt.nwbrower.top

[E11] 反转字符串
来源：http://ukk.zdqjudy.top

Py:   s[::-1]
来源：http://hop.zdbjq.cn

PHP:  strrev($s);
来源：http://ytg.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://ctz.hammf.cn

TS:   [...s].reverse().join("")
来源：http://pye.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ygh.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://sjf.zdqjudy.top

Ruby: s.reverse
来源：http://pdl.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://skt.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://pgr.vehdjk.com

Py:   s.count("a")
来源：http://fld.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://wyq.fktsv.cn

JS:   s.split("a").length - 1
来源：http://vww.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://tjq.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rhk.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://pyf.ehwqpu.com

Ruby: s.count("a")
来源：http://rti.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://ety.guannengcc.top

[E13] 逐字符遍历
来源：http://tib.316326.xyz

Py:   for ch in s: print(ch)
来源：http://cmq.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://djh.yongpay.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cah.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nmo.shuidangran.top


<!-- 参考信息 -->