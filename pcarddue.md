代发 wailian999

[D07] 切片 / 取子数组
来源：http://xjc.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://car.yj20258888.top

PHP:  array_slice($arr, 1, 3);
来源：http://dfg.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://bbb.zhongyouzk.top

TS:   arr.slice(1, 4);
来源：http://xkt.uphjek.com

Java: list.subList(1, 4);
来源：http://uel.guowangkeji.top

Go:   arr[1:4]
来源：http://xrc.daxiang520.top

Ruby: arr[1, 3]
来源：http://fur.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://onm.shuidangran.top

[D08] 合并两个数组
来源：http://siw.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://glu.kuanghao11.cn

PHP:  array_merge($a, $b);
来源：http://fmp.gogol.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qyn.jianghu66.top

TS:   [...a, ...b];
来源：http://rad.tian-w.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jzr.zhixingplan.top

Go:   append(a, b...)
来源：http://mdi.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://jhy.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://nwu.feifeiyinyue.top

[D09] 排序（升序）
来源：http://cwn.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ibe.jinqigufen.top

PHP:  sort($arr);
来源：http://mww.andypj.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oxc.yvedp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xgk.birdmap.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qyl.cheryme.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ukf.andypj.xyz

Ruby: arr.sort
来源：http://qku.quarkkingdee.top

C#:   list.Sort();
来源：http://jaw.yj20258.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbe.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hgw.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://los.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ncq.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oyz.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lrr.jinghuilouyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qhc.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bsy.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jzx.ivvv.top

[D11] 反转数组
来源：http://gff.kuanghao11.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jfp.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://esj.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ont.cheryme.top

TS:   [...arr].reverse();
来源：http://opv.hcnkem.com

Java: Collections.reverse(list);
来源：http://ceo.redwolf501.top

Go:   slices.Reverse(arr)
来源：http://zmh.sjlbkw.cn

Ruby: arr.reverse
来源：http://xeu.wangshuangyany.cn

C#:   list.Reverse();
来源：http://mpj.hysaishi.cn

[D12] 查找元素下标
来源：http://ghb.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://lxz.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lal.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://srv.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sur.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rgi.yj20258.top

Go:   slices.Index(arr, x)
来源：http://xam.sufxvd.cn

Ruby: arr.index(x)
来源：http://uoy.hammf.cn

C#:   list.IndexOf(x);
来源：http://sho.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://iyg.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xcv.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dxj.snrcjt.cn

JS:   arr.filter(x => x > 3)
来源：http://qmb.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://xdy.andypj.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fge.yfazqb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://waa.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tcm.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://yao.havefunace.top

[D14] 映射转换（每个元素变形）
来源：http://fxk.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ayx.shuidangran.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ski.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://cki.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://qsr.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zmm.bjfxy.top

Go:   // 手写循环
来源：http://gci.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://hpe.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tzb.yueranfly.top

[D15] 去重
来源：http://wzu.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tfw.0kj1m.cn

PHP:  array_unique($arr);
来源：http://bja.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://pyo.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://ylf.kuanghao11.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dvy.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://ikm.xziqi.cn

Ruby: arr.uniq
来源：http://dzz.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://wrb.jianghu66.top

[D16] 求和与平均值
来源：http://eik.iojbl.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vby.shangyingyoupin.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yjf.pengpengdd.cyou

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://itq.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vvu.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tto.guowangkeji.top

Go:   // 手写循环累加
来源：http://pqu.ydjk.org.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tny.nanxuanxn.top

C#:   list.Sum();  list.Average()
来源：http://gzv.xylfe.cn

[D17] 最大值与最小值
来源：http://yjq.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://vjp.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://ftl.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ouq.xuetiantiany.cn

TS:   Math.max(...arr);
来源：http://kqp.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pad.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://syf.316326.xyz

Ruby: arr.max;  arr.min
来源：http://whw.yangfankeji.com

C#:   list.Max();  list.Min()
来源：http://usr.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://vvq.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xdc.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://pwe.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zzz.daria6918.cn

TS:   nested.flat();
来源：http://kkp.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qfs.hfpthk.cn

Go:   // 手写双层循环
来源：http://pwj.tanke756.top

Ruby: nested.flatten
来源：http://zsc.daxiang520.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jcs.chenjidiqi.icu

[D19] 按字段分组
来源：http://dpe.shanyushiyangtech.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mxt.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mtx.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ukn.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gay.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://swa.ppjwa.cn

Go:   // 手写 map[string][]T
来源：http://toc.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eum.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fmj.xingfuxueyuan.xyz

[D20] 统计每个元素出现次数
来源：http://gtf.jinqigufen.top

Py:   Counter(arr)
来源：http://sad.fzhhl.top

PHP:  array_count_values($arr);
来源：http://zlo.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://byc.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ric.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jcy.haohaochexian.top

Go:   // 手写 map[T]int
来源：http://tnw.jiagoushi.top

Ruby: arr.tally
来源：http://evn.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qtp.ybcxt.top

[D21] 判断是否包含某元素
来源：http://foh.redwolf501.top

Py:   x in arr
来源：http://rfe.meibo888.top

PHP:  in_array($x, $arr, true);
来源：http://fhb.ydjk.org.cn

JS:   arr.includes(x)
来源：http://fiy.tarul.cn

TS:   arr.includes(x)
来源：http://wzu.shuidangran.top

Java: list.contains(x)
来源：http://wta.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://muo.zdqjudy.top

Ruby: arr.include?(x)
来源：http://nme.ppjwa.cn

C#:   list.Contains(x)
来源：http://bwc.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://ccg.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qcv.xuanzx.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wns.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wdi.xuanzx.com

TS:   [...arr];
来源：http://uou.zhiwuduotai.top

Java: new ArrayList<>(list);
来源：http://rbz.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uze.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://ebw.ydzc1.top

C#:   new List<int>(list);
来源：http://afg.hesvh.cn

[D23] reduce 累积计算
来源：http://ksa.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://afu.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uih.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ynx.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kbf.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://obx.fanxiaobao.xyz

Go:   // 手写循环
来源：http://ayd.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uzk.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://okr.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://zgi.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cfj.chenlongwang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://geq.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mpk.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ila.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lbw.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mbv.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vir.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nbp.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://tic.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ohu.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hbi.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ktg.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eis.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lvr.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dmh.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwq.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jva.ivvv.top

[D26] 数组转字符串
来源：http://mnk.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://gxi.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://dyz.jiagoushi.top

JS:   arr.join(", ")
来源：http://dsn.gzhubu.top

TS:   arr.join(", ")
来源：http://qur.yfazqb.com

Java: String.join(", ", list)
来源：http://yad.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://rtf.cucudq.cn

Ruby: arr.join(", ")
来源：http://ixa.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://xis.cashguo.top

================================================================================
来源：http://smb.zhengqikj.top

E. 字符串处理
来源：http://uvg.ywan-chungtsiang.top

================================================================================
来源：http://reo.shanyushiyangtech.top

[E01] 拼接字符串
来源：http://seb.bjfxy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xnm.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://klx.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wni.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://onw.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://afc.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mwl.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://swv.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qkv.jinqigufen.top

[E02] 重复字符串
来源：http://cjm.ctjpmb.com

Py:   "ab" * 3
来源：http://pnh.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://mvh.fzhhl.top

JS:   "ab".repeat(3)
来源：http://fny.kuanghao11.cn

TS:   "ab".repeat(3)
来源：http://bsc.jianghu66.top

Java: "ab".repeat(3)
来源：http://hdj.zhixingplan.top

Go:   strings.Repeat("ab", 3)
来源：http://ill.guowangkeji.top

Ruby: "ab" * 3
来源：http://kqt.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://btb.kuanghao11.cn

[E03] 截取子串
来源：http://qmp.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://axf.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aby.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxz.chenlongwang.top

TS:   s.slice(1, 4)
来源：http://vbd.xinyue.icu

Java: s.substring(1, 4)
来源：http://yev.jinqigfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sxj.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://ycj.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://iwl.smart0.xyz

[E04] 查找子串位置
来源：http://yyq.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://hpb.zhaomingkeji.xyz

PHP:  strpos($s, "x");
来源：http://atw.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://csj.snrcjt.cn

TS:   s.indexOf("x")
来源：http://res.epnwcf.com

Java: s.indexOf("x")
来源：http://ofe.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://anc.fengsongda.top

Ruby: s.index("x")
来源：http://cvu.ivvv.top

C#:   s.IndexOf("x")
来源：http://mib.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vyl.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hou.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pxi.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wks.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://alw.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://alt.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://obo.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ysn.dashuyun.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uog.cucudq.cn

[E06] 替换子串
来源：http://bys.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://znv.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://ffu.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yma.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://dcr.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cfc.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cof.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qri.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://yvc.sjlbkw.cn

[E07] 按分隔符拆分
来源：http://czz.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://erw.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ssm.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://zjb.yj202588.top

TS:   s.split(",")
来源：http://upp.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://chn.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ngm.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://zmo.jinqigufen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://txy.guannengcc.top

[E08] 数组按分隔符合并
来源：http://ymz.wangshuangyany.cn

Py:   ",".join(items)
来源：http://zic.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://frh.zhongyouzk.top

JS:   items.join(",")
来源：http://pgl.fengsongda.top

TS:   items.join(",")
来源：http://fdz.cdnleiting.top

Java: String.join(",", items)
来源：http://epz.ppjwa.cn

Go:   strings.Join(items, ",")
来源：http://ppr.iojbl.cn

Ruby: items.join(",")
来源：http://hgm.dashuyun.cn

C#:   string.Join(",", items)
来源：http://byq.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://dbs.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mki.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://euj.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://dui.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://cpi.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://med.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sgn.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://bxx.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zig.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://mri.yangfankeji.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://erb.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bdr.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://moq.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://dno.ppjwa.cn

Java: String.format("%03d", 7)
来源：http://zut.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mlc.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cxr.yanxiufei.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cui.yvedp.cn

[E11] 反转字符串
来源：http://yap.yonumen.top

Py:   s[::-1]
来源：http://fwf.gzhubu.top

PHP:  strrev($s);
来源：http://xvq.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://tji.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://cfx.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ycm.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hsh.tian-w.cn

Ruby: s.reverse
来源：http://tgr.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://dda.bjfxy.top

[E12] 统计某字符出现次数
来源：http://isp.ctjpmb.com

Py:   s.count("a")
来源：http://pve.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://suw.vehdjk.com

JS:   s.split("a").length - 1
来源：http://qkd.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://ytk.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ono.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://gce.zhongyouzk.top

Ruby: s.count("a")
来源：http://dar.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://nlw.zhongyouzk.top

[E13] 逐字符遍历
来源：http://ocb.daria6918.cn

Py:   for ch in s: print(ch)
来源：http://lzx.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwe.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vfk.daxiang520.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://leh.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zqg.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nbk.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fma.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vim.smart0.xyz


<!-- 参考信息 -->