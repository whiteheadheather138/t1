代发 wailian999

[D07] 切片 / 取子数组
来源：http://hgn.fzhhl.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qey.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nsa.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://aqg.ehwqpu.com

TS:   arr.slice(1, 4);
来源：http://gfb.fzhhl.top

Java: list.subList(1, 4);
来源：http://zft.wangshuangyany.cn

Go:   arr[1:4]
来源：http://mwv.haohaochexian.top

Ruby: arr[1, 3]
来源：http://wzl.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://ycy.cucudq.cn

[D08] 合并两个数组
来源：http://ouf.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://pjs.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://pzf.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zei.sweek.top

TS:   [...a, ...b];
来源：http://ngg.hnxiangtu.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tyf.xziqi.cn

Go:   append(a, b...)
来源：http://zxn.fzhhl.top

Ruby: a + b;  a.concat(b)
来源：http://tzr.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://dzo.yuxming.cn

[D09] 排序（升序）
来源：http://xgf.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://ref.mhx1999.top

PHP:  sort($arr);
来源：http://nom.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cvp.andypj.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://gud.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://twp.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yre.ywan-chungtsiang.top

Ruby: arr.sort
来源：http://bam.chenzaomai.com

C#:   list.Sort();
来源：http://pzz.dianchejie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kke.jinqigfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ifz.cheryme.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wbc.fengsongda.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lck.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://coc.cucudq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tvl.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jgj.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eog.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yvf.wangshuangyany.cn

[D11] 反转数组
来源：http://qsf.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://hzj.mhx1999.top

PHP:  array_reverse($arr);
来源：http://zez.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vdt.epnwcf.com

TS:   [...arr].reverse();
来源：http://cox.ivvv.top

Java: Collections.reverse(list);
来源：http://bfh.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://uhm.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://wkj.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://qec.gzhubu.top

[D12] 查找元素下标
来源：http://udf.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://qrh.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://thz.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gos.dashuyun.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdw.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cwr.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://ngv.pengpengdd.cyou

Ruby: arr.index(x)
来源：http://tku.cashguo.top

C#:   list.IndexOf(x);
来源：http://qiq.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://dcf.zhijiandao.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bjh.zhixingplan.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fxb.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://axy.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://ypw.yfazqb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxo.xziqi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qai.zhixingplan.top

Ruby: arr.select { |x| x > 3 }
来源：http://mlb.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gvr.mhx1999.top

[D14] 映射转换（每个元素变形）
来源：http://tpw.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iir.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wzr.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://cns.0kj1m.cn

TS:   arr.map(x => x * 2)
来源：http://wvg.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aut.fengsongda.top

Go:   // 手写循环
来源：http://jfb.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zvj.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://icg.xuanzx.com

[D15] 去重
来源：http://tep.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cjd.redwolf501.top

PHP:  array_unique($arr);
来源：http://nqu.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://cfk.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://tyz.cashguo.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://quv.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://xwu.xziqi.cn

Ruby: arr.uniq
来源：http://ily.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://afv.yueranfly.top

[D16] 求和与平均值
来源：http://bfg.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mny.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cia.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qkk.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sir.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cnw.xziqi.cn

Go:   // 手写循环累加
来源：http://duy.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uvw.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://kti.jinghuilouyu.cn

[D17] 最大值与最小值
来源：http://ttc.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://ryg.hongshengwenyu.top

PHP:  max($arr);  min($arr);
来源：http://ymq.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vtk.uphjek.com

TS:   Math.max(...arr);
来源：http://jcv.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ykv.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gfr.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://xhb.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://tnh.iojbl.cn

[D18] 扁平化嵌套数组
来源：http://gdo.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nwi.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://dey.wangshuangyany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vue.sysykeji.top

TS:   nested.flat();
来源：http://jmq.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uer.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://vib.svipenyu.cn

Ruby: nested.flatten
来源：http://fln.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vsv.jianghu66.top

[D19] 按字段分组
来源：http://dmb.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iyv.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gem.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hmt.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vpj.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://txd.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://rxq.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tyy.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wlq.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://sov.yuanzhike.top

Py:   Counter(arr)
来源：http://njn.xinyue.icu

PHP:  array_count_values($arr);
来源：http://vyd.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mjh.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fao.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nqg.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://ofe.ydjk.org.cn

Ruby: arr.tally
来源：http://ekp.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kdt.zhiwuduotai.top

[D21] 判断是否包含某元素
来源：http://obj.epnwcf.com

Py:   x in arr
来源：http://bsa.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://dgg.tian-w.cn

JS:   arr.includes(x)
来源：http://emd.daxiang520.top

TS:   arr.includes(x)
来源：http://rfj.yanxiufei.cn

Java: list.contains(x)
来源：http://wdc.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://oyz.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://kee.guowangkeji.top

C#:   list.Contains(x)
来源：http://muv.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://aup.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lau.quarkkingdee.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zhb.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nkm.aibaodan.cn

TS:   [...arr];
来源：http://ukb.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://kne.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://sbd.yonumen.top

Ruby: arr.dup;  arr.clone
来源：http://ena.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://efu.yuanzhike.top

[D23] reduce 累积计算
来源：http://lmi.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dvc.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kcu.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wiw.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxv.guannengcc.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ovi.fanxiaobao.xyz

Go:   // 手写循环
来源：http://dcs.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zvc.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ffz.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://rch.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qao.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nau.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wnk.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tap.zhongyouzk.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jlo.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sbh.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jdp.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jzv.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://zhy.zhiwuduotai.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://imz.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qbi.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nqp.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://she.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bij.tianlin.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ouc.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mef.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wnp.hnxiangtu.top

[D26] 数组转字符串
来源：http://krx.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://ghm.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://cek.xylfe.cn

JS:   arr.join(", ")
来源：http://cke.ppjwa.cn

TS:   arr.join(", ")
来源：http://qad.jiagoushi.top

Java: String.join(", ", list)
来源：http://zrc.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://hpw.meibo888.top

Ruby: arr.join(", ")
来源：http://jbq.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://wyd.svipenyu.cn

================================================================================
来源：http://izl.jqgfzy.top

E. 字符串处理
来源：http://wid.ehwqpu.com

================================================================================
来源：http://gxc.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://bcy.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bfq.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xxx.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzk.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wlj.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mzt.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ptw.aibaodan.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pwr.nanxuanxn.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xic.xuetiantiany.cn

[E02] 重复字符串
来源：http://ojg.zycfv.cn

Py:   "ab" * 3
来源：http://geh.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://adt.meibo888.top

JS:   "ab".repeat(3)
来源：http://vip.xziqi.cn

TS:   "ab".repeat(3)
来源：http://zai.jyoumei.cn

Java: "ab".repeat(3)
来源：http://cpq.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://dup.ehwqpu.com

Ruby: "ab" * 3
来源：http://fsq.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ibd.hesvh.cn

[E03] 截取子串
来源：http://ktf.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uon.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oyw.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tik.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://kke.hysaishi.cn

Java: s.substring(1, 4)
来源：http://pol.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aoq.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lnu.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://ewz.bjfxy.top

[E04] 查找子串位置
来源：http://ptu.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://nxv.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://qor.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ndh.xinyue.icu

TS:   s.indexOf("x")
来源：http://yxx.zhoulong.xyz

Java: s.indexOf("x")
来源：http://bux.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://btb.fengsongda.top

Ruby: s.index("x")
来源：http://nmm.fehbvm.com

C#:   s.IndexOf("x")
来源：http://yoj.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hts.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jtr.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zvz.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://keb.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwo.zhijiandao.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvc.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zni.chenlongwang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pwx.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rbx.hesvh.cn

[E06] 替换子串
来源：http://uil.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rmm.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://ulf.dianchejie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vch.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://dke.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pju.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bdm.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nkb.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://zvw.yvedp.cn

[E07] 按分隔符拆分
来源：http://qbx.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ybx.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ehv.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bma.iojbl.cn

TS:   s.split(",")
来源：http://gvk.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://psb.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pgx.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://amv.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tld.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://wty.sjlbkw.cn

Py:   ",".join(items)
来源：http://ufi.jqgfzy.top

PHP:  implode(",", $items);
来源：http://zbw.chenzaomai.com

JS:   items.join(",")
来源：http://mqe.52xcode.cn

TS:   items.join(",")
来源：http://uox.vehdjk.com

Java: String.join(",", items)
来源：http://jnb.meibo888.top

Go:   strings.Join(items, ",")
来源：http://jdk.gotoacloud.top

Ruby: items.join(",")
来源：http://caq.zdbjq.cn

C#:   string.Join(",", items)
来源：http://cjf.andypj.xyz

[E09] 去除所有空白字符
来源：http://xks.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rfp.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fvo.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://nrq.vehdjk.com

TS:   s.replace(/\s+/g, "")
来源：http://rbf.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://zom.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://snj.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ile.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://odn.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://lvo.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kmx.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uvr.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://oaq.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://ksy.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://axw.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sya.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ice.sufxvd.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tuq.redwolf501.top

[E11] 反转字符串
来源：http://ivb.jqgfzy.top

Py:   s[::-1]
来源：http://brm.yueranfly.top

PHP:  strrev($s);
来源：http://jxb.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://cny.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://tgz.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nip.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vuz.316326.xyz

Ruby: s.reverse
来源：http://aaa.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://pho.zycfv.cn

[E12] 统计某字符出现次数
来源：http://jrs.shuidangran.top

Py:   s.count("a")
来源：http://vsl.jiagoushi.top

PHP:  substr_count($s, "a");
来源：http://oqi.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://nhb.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://yda.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yke.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://fvu.hnxiangtu.top

Ruby: s.count("a")
来源：http://ogi.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://kxd.tanke756.top

[E13] 逐字符遍历
来源：http://mop.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://vcl.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zkh.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://gmt.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cjb.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fqx.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://efy.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dtj.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://khv.fengsongda.top


<!-- 参考信息 -->