代发 wailian999

TS:   arr.slice(1, 4);
来源：http://otr.hongshengwenyu.top

Java: list.subList(1, 4);
来源：http://lzd.cheryme.top

Go:   arr[1:4]
来源：http://eaq.daxiang520.top

Ruby: arr[1, 3]
来源：http://sjm.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://ysy.c1oappe.top

[D08] 合并两个数组
来源：http://jyr.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://pty.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://ijm.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vgb.ybcxt.top

TS:   [...a, ...b];
来源：http://lal.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://waq.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://ilt.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://pim.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://rua.xuanzx.com

[D09] 排序（升序）
来源：http://vkn.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://kjm.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://uzl.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ere.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://har.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ztt.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fnf.ydjk.org.cn

Ruby: arr.sort
来源：http://olf.ctjpmb.com

C#:   list.Sort();
来源：http://khg.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://uvx.ydzc1.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpq.snrcjt.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyf.hnxiangtu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bwn.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jia.ehwqpu.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://usd.xingfuxueyuan.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xto.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uex.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ibi.shanyushiyangtech.top

[D11] 反转数组
来源：http://ucj.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://qis.svipenyu.cn

PHP:  array_reverse($arr);
来源：http://cig.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pur.ctjpmb.com

TS:   [...arr].reverse();
来源：http://hej.uphjek.com

Java: Collections.reverse(list);
来源：http://xyv.havefunace.top

Go:   slices.Reverse(arr)
来源：http://qkz.ydzc1.top

Ruby: arr.reverse
来源：http://sac.vqdsnc.cn

C#:   list.Reverse();
来源：http://wzi.smart0.xyz

[D12] 查找元素下标
来源：http://vas.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://vpm.sxryk.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oqo.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zqm.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://com.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fjf.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://kcu.daxiang520.top

Ruby: arr.index(x)
来源：http://vkc.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://zee.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://qqj.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xqi.vqdsnc.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://irz.ydjk.org.cn

JS:   arr.filter(x => x > 3)
来源：http://pdf.hcnkem.com

TS:   arr.filter(x => x > 3)
来源：http://rke.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ahq.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mbf.zdqjudy.top

Ruby: arr.select { |x| x > 3 }
来源：http://eef.sysykeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xap.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://erd.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eid.yongpay.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cvr.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://bkt.jlsjyb.cn

TS:   arr.map(x => x * 2)
来源：http://vok.pycfn.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://zgr.pengpengdd.cyou

Go:   // 手写循环
来源：http://igk.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ngb.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ngm.jyoumei.cn

[D15] 去重
来源：http://fxw.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xvo.ydzc1.top

PHP:  array_unique($arr);
来源：http://pld.yfazqb.com

JS:   [...new Set(arr)]
来源：http://lar.cucudq.cn

TS:   [...new Set(arr)]
来源：http://dat.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vtq.yongpay.top

Go:   // 用 map[T]struct{} 手写
来源：http://sxj.hcnkem.com

Ruby: arr.uniq
来源：http://sis.xingfuxueyuan.xyz

C#:   list.Distinct().ToList()
来源：http://mal.cqqwz.cn

[D16] 求和与平均值
来源：http://iha.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qos.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mry.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bdb.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dww.zhoulong.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cez.sufxvd.cn

Go:   // 手写循环累加
来源：http://nkg.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ity.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://bak.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://joo.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://hor.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://lwg.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pnj.wangshuangyany.cn

TS:   Math.max(...arr);
来源：http://skm.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://hxq.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wao.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://igb.cheryme.top

C#:   list.Max();  list.Min()
来源：http://aql.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://xyn.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://imw.fehbvm.com

PHP:  array_merge(...$nested);
来源：http://nyb.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tez.hongshengwenyu.top

TS:   nested.flat();
来源：http://pez.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rqz.zhijiandao.cn

Go:   // 手写双层循环
来源：http://qzs.nanxinkj.top

Ruby: nested.flatten
来源：http://frw.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xkz.vqdsnc.cn

[D19] 按字段分组
来源：http://ssi.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dwe.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hqc.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://arq.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rmy.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tuc.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://mmd.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xqr.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rno.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://ooj.pycfn.com

Py:   Counter(arr)
来源：http://uux.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://mvw.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zxe.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pus.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xwa.sweek.top

Go:   // 手写 map[T]int
来源：http://owy.wangdashe.top

Ruby: arr.tally
来源：http://akq.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ben.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://ogo.yj20258.top

Py:   x in arr
来源：http://try.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://gay.tian-w.cn

JS:   arr.includes(x)
来源：http://sxd.svipenyu.cn

TS:   arr.includes(x)
来源：http://ekq.zhengqikj.top

Java: list.contains(x)
来源：http://pcu.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://nli.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://rjs.yfazqb.com

C#:   list.Contains(x)
来源：http://cfy.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://epv.daria6918.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gew.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ers.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nif.yuxming.cn

TS:   [...arr];
来源：http://euo.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://gdt.yj20258888.top

Go:   copied := append([]int(nil), arr...)
来源：http://juz.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://ghj.yanxiufei.cn

C#:   new List<int>(list);
来源：http://sdu.zycfv.cn

[D23] reduce 累积计算
来源：http://mwd.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://odp.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://klk.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvm.cashguo.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tto.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xxm.yuxming.cn

Go:   // 手写循环
来源：http://qee.shzxlz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hmi.dianchejie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qxl.dashuyun.cn

[D24] 字典 / Map 基本操作
来源：http://npl.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dxp.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kqj.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tor.hesvh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xxf.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wnp.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uyl.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bqx.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kmf.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://vad.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sgd.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tva.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ioa.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ryp.gogol.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qcb.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dii.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hxy.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nse.nwbrower.top

[D26] 数组转字符串
来源：http://bnz.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://xvy.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://zog.yuxming.cn

JS:   arr.join(", ")
来源：http://ksr.gaohongyu789.top

TS:   arr.join(", ")
来源：http://buv.meibo888.top

Java: String.join(", ", list)
来源：http://nng.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://tnh.hysaishi.cn

Ruby: arr.join(", ")
来源：http://xcp.hnqzz.top

C#:   string.Join(", ", list)
来源：http://wri.shanyushiyangtech.top

================================================================================
来源：http://dsw.fzhhl.top

E. 字符串处理
来源：http://jyc.guowangkeji.top

================================================================================
来源：http://avf.nanxuanxn.top

[E01] 拼接字符串
来源：http://bkw.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://typ.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ysw.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mfc.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://grs.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://exr.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cdi.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mra.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://leu.gotoacloud.top

[E02] 重复字符串
来源：http://ptg.snrcjt.cn

Py:   "ab" * 3
来源：http://unv.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://hry.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://amw.yj202588.top

TS:   "ab".repeat(3)
来源：http://ezp.0kj1m.cn

Java: "ab".repeat(3)
来源：http://ivq.shanyushiyangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://bvz.nwbrower.top

Ruby: "ab" * 3
来源：http://iwv.vehdjk.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ibe.nanxinkj.top

[E03] 截取子串
来源：http://clx.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pks.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wkx.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://viv.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://dba.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://yfx.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yre.yanxiufei.cn

Ruby: s[1, 3];  s[1..3]
来源：http://khh.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://byn.daxiang520.top

[E04] 查找子串位置
来源：http://xec.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://qqb.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://oan.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://olt.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://frq.havefunace.top

Java: s.indexOf("x")
来源：http://afd.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://hbp.jiagoushi.top

Ruby: s.index("x")
来源：http://cvn.chenlongwang.top

C#:   s.IndexOf("x")
来源：http://wgy.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ujc.tanke756.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kdu.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ptj.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ouk.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xyl.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nop.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nzm.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nrr.jinqigufen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wae.zdbjq.cn

[E06] 替换子串
来源：http://zgc.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jjd.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://rbe.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qjj.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://tgz.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blu.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oqi.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ohb.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://gch.iojbl.cn

[E07] 按分隔符拆分
来源：http://saa.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjf.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sct.jianghu66.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://udx.jlsjyb.cn

TS:   s.split(",")
来源：http://adf.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://dim.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cky.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://ogs.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nea.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://yzz.feifeiyinyue.top

Py:   ",".join(items)
来源：http://mim.shuidangran.top

PHP:  implode(",", $items);
来源：http://gyb.chenlongwang.top

JS:   items.join(",")
来源：http://qdv.dashuyun.cn

TS:   items.join(",")
来源：http://ttp.birdmap.top

Java: String.join(",", items)
来源：http://lql.uphjek.com

Go:   strings.Join(items, ",")
来源：http://gjc.smart0.xyz

Ruby: items.join(",")
来源：http://ndw.redwolf501.top

C#:   string.Join(",", items)
来源：http://axm.yj20258.top

[E09] 去除所有空白字符
来源：http://qwb.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfs.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://csv.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://cee.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://wik.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://ghm.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eqw.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://yjk.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fbf.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://qep.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gfn.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kau.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://lsj.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://jkx.uphjek.com

Java: String.format("%03d", 7)
来源：http://jqf.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://phc.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ksp.snrcjt.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gsb.mhx1999.top

[E11] 反转字符串
来源：http://udt.cucudq.cn

Py:   s[::-1]
来源：http://yak.daria6918.cn

PHP:  strrev($s);
来源：http://tvr.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://zqv.birdmap.top

TS:   [...s].reverse().join("")
来源：http://bin.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pmy.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ala.snrcjt.cn

Ruby: s.reverse
来源：http://qny.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://brq.epnwcf.com

[E12] 统计某字符出现次数
来源：http://bdi.hammf.cn

Py:   s.count("a")
来源：http://mvr.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://dni.tarul.cn

JS:   s.split("a").length - 1
来源：http://dda.nanxinkj.top

TS:   s.split("a").length - 1
来源：http://uai.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pit.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://miv.yj202588.top

Ruby: s.count("a")
来源：http://dcw.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://oxn.daxiang520.top

[E13] 逐字符遍历
来源：http://nre.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://pkk.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xkh.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oqx.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wku.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ipf.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ply.hysaishi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sqk.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oue.tarul.cn

[E14] URL 编码与 Base64
来源：http://dim.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://anp.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vtj.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pkq.hongshengwenyu.top


<!-- 参考信息 -->