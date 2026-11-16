代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://pez.0kj1m.cn

TS:   [...a, ...b];
来源：http://dlu.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uao.shangyingyoupin.top

Go:   append(a, b...)
来源：http://xut.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://gkd.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://vmj.fktsv.cn

[D09] 排序（升序）
来源：http://nhk.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dzm.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://ibx.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ink.mhx1999.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mxe.shuidangran.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xob.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://udx.redwolf501.top

Ruby: arr.sort
来源：http://cyy.andypj.xyz

C#:   list.Sort();
来源：http://vnv.sjlbkw.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rcp.yj202588.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aly.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mbe.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmf.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xne.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dlw.cucudq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pzp.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ssw.tianlin.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://clg.yuxming.cn

[D11] 反转数组
来源：http://fhs.cdnleiting.top

Py:   arr[::-1];  arr.reverse()
来源：http://jph.dianchejie.cn

PHP:  array_reverse($arr);
来源：http://owd.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rmo.xylfe.cn

TS:   [...arr].reverse();
来源：http://ezj.sxryk.cn

Java: Collections.reverse(list);
来源：http://oip.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://xow.vehdjk.com

Ruby: arr.reverse
来源：http://kww.ehwqpu.com

C#:   list.Reverse();
来源：http://ghn.gogol.net.cn

[D12] 查找元素下标
来源：http://zlm.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://aea.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fco.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rgo.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gae.guannengcc.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tue.uphjek.com

Go:   slices.Index(arr, x)
来源：http://kfk.jqgufenzy.top

Ruby: arr.index(x)
来源：http://idv.yvedp.cn

C#:   list.IndexOf(x);
来源：http://dms.birdmap.top

[D13] 过滤（保留满足条件的）
来源：http://eml.ydjk.org.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cux.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://psw.jinyuanbaomall.cn

JS:   arr.filter(x => x > 3)
来源：http://lhm.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://wph.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wwb.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yik.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://xyq.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://lak.yuxming.cn

[D14] 映射转换（每个元素变形）
来源：http://omc.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dcm.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xqg.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://dyu.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://tqp.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hwl.hnxiangtu.top

Go:   // 手写循环
来源：http://bxu.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hir.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mau.haohaochexian.top

[D15] 去重
来源：http://sab.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jxd.bjfxy.top

PHP:  array_unique($arr);
来源：http://udx.xziqi.cn

JS:   [...new Set(arr)]
来源：http://kzp.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://ikq.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://udp.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://aer.chenzaomai.com

Ruby: arr.uniq
来源：http://ngh.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://lpu.feifeiyinyue.top

[D16] 求和与平均值
来源：http://lmp.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dyw.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mpz.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mpm.zdbjq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwc.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bnz.xylfe.cn

Go:   // 手写循环累加
来源：http://hmw.jiagoushi.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dkx.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://soc.nwbrower.top

[D17] 最大值与最小值
来源：http://qzs.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://hee.hnxiangtu.top

PHP:  max($arr);  min($arr);
来源：http://vbp.iojbl.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pgu.0kj1m.cn

TS:   Math.max(...arr);
来源：http://njl.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ini.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kld.nanxinkj.top

Ruby: arr.max;  arr.min
来源：http://utm.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://zrz.tarul.cn

[D18] 扁平化嵌套数组
来源：http://bfh.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lxj.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://uvg.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eib.guowangkeji.top

TS:   nested.flat();
来源：http://bkx.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dsi.jyoumei.cn

Go:   // 手写双层循环
来源：http://ced.hongshengwenyu.top

Ruby: nested.flatten
来源：http://ipq.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iib.ydjk.org.cn

[D19] 按字段分组
来源：http://wcy.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ycm.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tcq.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dli.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yez.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yav.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://owq.fehbvm.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://swc.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://izu.svipenyu.cn

[D20] 统计每个元素出现次数
来源：http://fgu.daria6918.cn

Py:   Counter(arr)
来源：http://ilk.52xcode.cn

PHP:  array_count_values($arr);
来源：http://whs.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ohz.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xpi.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zlf.ybcxt.top

Go:   // 手写 map[T]int
来源：http://txq.yangfankeji.com

Ruby: arr.tally
来源：http://hbm.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tlj.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://aaw.zhaomingkeji.xyz

Py:   x in arr
来源：http://qtv.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://xlm.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://bff.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://irr.316326.xyz

Java: list.contains(x)
来源：http://nbx.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://owi.yj202588.top

Ruby: arr.include?(x)
来源：http://nic.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://uni.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://ziv.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fde.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kdw.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oqu.shanyushiyangtech.top

TS:   [...arr];
来源：http://flf.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://bnm.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://hsa.daria6918.cn

Ruby: arr.dup;  arr.clone
来源：http://btn.sjlbkw.cn

C#:   new List<int>(list);
来源：http://gft.birdmap.top

[D23] reduce 累积计算
来源：http://mxf.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ult.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ygg.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://olg.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zvk.52xcode.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cga.aibaodan.cn

Go:   // 手写循环
来源：http://rom.jinghuilouyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qio.xinyue.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sov.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://dvm.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ktx.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vhm.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mub.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xll.yuanzhike.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sek.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ulv.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pbg.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xvg.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://anq.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://loj.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gag.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uyj.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ppm.shanyushiyangtech.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wif.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oou.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ieq.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://adq.cdnleiting.top

[D26] 数组转字符串
来源：http://qys.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://ebb.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://nii.ctjpmb.com

JS:   arr.join(", ")
来源：http://xzj.nwbrower.top

TS:   arr.join(", ")
来源：http://ots.pengpengdd.cyou

Java: String.join(", ", list)
来源：http://tnp.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://lpe.gaohongyu789.top

Ruby: arr.join(", ")
来源：http://jlb.hammf.cn

C#:   string.Join(", ", list)
来源：http://saw.redwolf501.top

================================================================================
来源：http://adp.gogol.net.cn

E. 字符串处理
来源：http://hvu.yanxiufei.cn

================================================================================
来源：http://ygn.jianghu66.top

[E01] 拼接字符串
来源：http://oud.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lrg.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://itj.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rcb.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqr.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gvi.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sxh.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nij.fktsv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bez.ybcxt.top

[E02] 重复字符串
来源：http://qaj.aibaodan.cn

Py:   "ab" * 3
来源：http://amt.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://ylm.mhx1999.top

JS:   "ab".repeat(3)
来源：http://oit.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://jzv.chenzaomai.com

Java: "ab".repeat(3)
来源：http://fve.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://rou.xuanzx.com

Ruby: "ab" * 3
来源：http://sjg.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ypv.quarkkingdee.top

[E03] 截取子串
来源：http://gpc.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://asl.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://brg.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gaf.smart0.xyz

TS:   s.slice(1, 4)
来源：http://pxv.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://omq.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fon.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://raz.zhoulong.xyz

C#:   s.Substring(1, 3)
来源：http://jss.vqdsnc.cn

[E04] 查找子串位置
来源：http://iqz.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://gvo.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://dkt.jinghuilouyu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gpf.fehbvm.com

TS:   s.indexOf("x")
来源：http://kdz.chenzaomai.com

Java: s.indexOf("x")
来源：http://vml.zhixingplan.top

Go:   strings.Index(s, "x")
来源：http://wol.fktsv.cn

Ruby: s.index("x")
来源：http://agn.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://wob.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://axv.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nwh.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qet.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://miz.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ezn.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxy.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kmy.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ifj.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xal.cdnleiting.top

[E06] 替换子串
来源：http://bkk.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xim.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://clc.fengsongda.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lac.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://dsc.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dem.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://veo.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mbb.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://xhv.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://qev.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xrq.sysykeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fuz.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rdk.c1oappe.top

TS:   s.split(",")
来源：http://bhs.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://nnr.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xoj.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://rba.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://onx.yj20258888.top

[E08] 数组按分隔符合并
来源：http://dnd.cucudq.cn

Py:   ",".join(items)
来源：http://fio.yj20258888.top

PHP:  implode(",", $items);
来源：http://cnm.shanyushiyangtech.top

JS:   items.join(",")
来源：http://zkp.yangfankeji.com

TS:   items.join(",")
来源：http://qsb.iojbl.cn

Java: String.join(",", items)
来源：http://myi.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://tnw.gotoacloud.top

Ruby: items.join(",")
来源：http://lyo.havefunace.top

C#:   string.Join(",", items)
来源：http://zsc.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://ydj.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ffp.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gtv.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://tao.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://evk.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://aqi.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://aze.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://fvs.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://obd.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://clj.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ajz.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hds.xylfe.cn

JS:   "7".padStart(3, "0")
来源：http://quv.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://qbi.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://ynm.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://hey.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qmd.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cwm.haohaochexian.top

[E11] 反转字符串
来源：http://opd.ydzc1.top

Py:   s[::-1]
来源：http://ota.shanyushiyangkeji.top

PHP:  strrev($s);
来源：http://yjo.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://npa.xuanzx.com

TS:   [...s].reverse().join("")
来源：http://bqa.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://oui.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rda.guannengcc.top

Ruby: s.reverse
来源：http://wpy.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://vrk.yj202588.top

[E12] 统计某字符出现次数
来源：http://ugb.xylfe.cn

Py:   s.count("a")
来源：http://uve.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://tne.fengsongda.top

JS:   s.split("a").length - 1
来源：http://hfq.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://arb.jqgfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://otr.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://ows.jqgfzy.top

Ruby: s.count("a")
来源：http://ozy.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://vdz.316326.xyz

[E13] 逐字符遍历
来源：http://obv.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://ojm.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zdd.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hfc.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://uye.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ydk.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uzq.sufxvd.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kwm.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fex.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://xyh.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qxz.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dtg.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jmf.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tox.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gkg.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xyj.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmv.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hha.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://mwo.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rcg.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wcj.xuanzx.com


<!-- 参考信息 -->