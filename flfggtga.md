代发 wailian999

[D03] 在指定位置插入元素
来源：http://iwl.jinghuilouyu.cn

Py:   arr.insert(0, 0)
来源：http://dvh.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://trb.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dpc.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://nvk.jianghu66.top

Java: list.add(0, 0);
来源：http://lzp.yongpay.top

Go:   arr = append([]int{0}, arr...)
来源：http://loi.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ntp.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://qxd.hongshengwenyu.top

[D04] 删除元素
来源：http://ojl.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://umf.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://yls.hcnkem.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qxc.xziqi.cn

TS:   arr.splice(0, 1);
来源：http://lfa.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xyn.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dbt.zdqjudy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nhs.jiagoushi.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xzh.c1oappe.top

[D05] 访问与修改元素
来源：http://hvn.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hiq.quarkkingdee.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nzw.hnxiangtu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xqq.guowangkeji.top

TS:   arr[0]; arr.at(-1);
来源：http://tib.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://enz.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://ueu.aibaodan.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rlb.chenjidiqi.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uup.yvedp.cn

[D06] 数组长度
来源：http://dpr.xylfe.cn

Py:   len(arr)
来源：http://soe.shangyingyoupin.top

PHP:  count($arr);
来源：http://pzg.hcnkem.com

JS:   arr.length
来源：http://tel.jyoumei.cn

TS:   arr.length
来源：http://hbn.aibaodan.cn

Java: list.size();
来源：http://qug.havefunace.top

Go:   len(arr)
来源：http://jrd.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://ixc.jinghuilouyu.cn

C#:   list.Count;
来源：http://irv.havefunace.top

[D07] 切片 / 取子数组
来源：http://qgi.cucudq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gjb.sjlbkw.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yoj.guowangkeji.top

JS:   arr.slice(1, 4);
来源：http://tzb.sjlbkw.cn

TS:   arr.slice(1, 4);
来源：http://rri.svipenyu.cn

Java: list.subList(1, 4);
来源：http://ylp.fengsongda.top

Go:   arr[1:4]
来源：http://wdv.pycfn.com

Ruby: arr[1, 3]
来源：http://yat.pycfn.com

C#:   list.GetRange(1, 3);
来源：http://wfv.c1oappe.top

[D08] 合并两个数组
来源：http://olt.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://bqc.chenzaomai.com

PHP:  array_merge($a, $b);
来源：http://awn.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mjm.jiagoushi.top

TS:   [...a, ...b];
来源：http://zwn.cucudq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://idu.guannengcc.top

Go:   append(a, b...)
来源：http://oiu.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://hgv.xinyue.icu

C#:   a.Concat(b).ToList()
来源：http://jqb.nwbrower.top

[D09] 排序（升序）
来源：http://rdz.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://lft.xuanzx.com

PHP:  sort($arr);
来源：http://uzc.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cho.jyoumei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ont.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dqy.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zqm.ehwqpu.com

Ruby: arr.sort
来源：http://cuk.ctjpmb.com

C#:   list.Sort();
来源：http://qzw.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mwr.shuidangran.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pes.uphjek.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://joj.wangshuangyany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfx.tian-w.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kxo.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pjp.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://all.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zik.jyoumei.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ejk.ywan-chungtsiang.top

[D11] 反转数组
来源：http://fce.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://cgr.xziqi.cn

PHP:  array_reverse($arr);
来源：http://dav.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jwc.guowangkeji.top

TS:   [...arr].reverse();
来源：http://wen.yongpay.top

Java: Collections.reverse(list);
来源：http://wdt.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://pio.chenlongwang.top

Ruby: arr.reverse
来源：http://hpj.cdnleiting.top

C#:   list.Reverse();
来源：http://lvt.gaohongyu789.top

[D12] 查找元素下标
来源：http://cfe.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://wvj.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wad.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cdh.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jvl.cdnleiting.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jnm.yvedp.cn

Go:   slices.Index(arr, x)
来源：http://sri.cdnleiting.top

Ruby: arr.index(x)
来源：http://lvi.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://xnj.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://ogs.zhoulong.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wgk.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ous.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://nwj.316326.xyz

TS:   arr.filter(x => x > 3)
来源：http://yov.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tlh.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://okv.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ybn.zhaomingkeji.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://wed.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://qri.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ghd.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tba.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://nkd.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://upe.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://huo.yangfankeji.com

Go:   // 手写循环
来源：http://xpa.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tat.ivvv.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gpr.sweek.top

[D15] 去重
来源：http://wyb.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nhy.xziqi.cn

PHP:  array_unique($arr);
来源：http://juz.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://usv.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://lqh.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://erq.svipenyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fkl.yuanzhike.top

Ruby: arr.uniq
来源：http://ifl.hammf.cn

C#:   list.Distinct().ToList()
来源：http://amr.snrcjt.cn

[D16] 求和与平均值
来源：http://sii.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xin.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tkf.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dqn.hnqzz.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dvy.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hmr.yongpay.top

Go:   // 手写循环累加
来源：http://vxp.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lrf.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://mpt.jinqigfzy.top

[D17] 最大值与最小值
来源：http://idf.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://wwk.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://avz.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hem.ctjpmb.com

TS:   Math.max(...arr);
来源：http://wqd.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kgt.ppjwa.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rlv.shangyingyoupin.top

Ruby: arr.max;  arr.min
来源：http://tfw.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://gfg.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://axw.fengsongda.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://srh.yongpay.top

PHP:  array_merge(...$nested);
来源：http://gql.zhongyouzk.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://smc.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://vlv.jianghu66.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dvf.guannengcc.top

Go:   // 手写双层循环
来源：http://qsa.shangyingyoupin.top

Ruby: nested.flatten
来源：http://jeg.shuidangran.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cne.vqdsnc.cn

[D19] 按字段分组
来源：http://cyy.zhixingplan.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kyx.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zfl.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oum.hcnkem.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://nxm.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://npq.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://knp.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dcu.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ada.hammf.cn

[D20] 统计每个元素出现次数
来源：http://zso.zdbjq.cn

Py:   Counter(arr)
来源：http://cyi.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://aje.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxa.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jdb.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awd.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://qhs.9152youxi.cn

Ruby: arr.tally
来源：http://lrq.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cel.jianghu66.top

[D21] 判断是否包含某元素
来源：http://sgv.jqgufenzy.top

Py:   x in arr
来源：http://dae.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://hss.vehdjk.com

JS:   arr.includes(x)
来源：http://pva.zhixingplan.top

TS:   arr.includes(x)
来源：http://nkl.kuanghao11.cn

Java: list.contains(x)
来源：http://dsv.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://ipu.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://byq.jqgfzy.top

C#:   list.Contains(x)
来源：http://ywo.epnwcf.com

[D22] 复制数组（避免共享引用）
来源：http://qgv.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kfv.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sih.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://urv.cashguo.top

TS:   [...arr];
来源：http://pez.feifeiyinyue.top

Java: new ArrayList<>(list);
来源：http://mqf.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://jkk.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://btk.sufxvd.cn

C#:   new List<int>(list);
来源：http://nys.52xcode.cn

[D23] reduce 累积计算
来源：http://pxu.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rjf.smart0.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hza.sufxvd.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wsn.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwo.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://bfj.feifeiyinyue.top

Go:   // 手写循环
来源：http://rdc.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cjx.quarkkingdee.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://haw.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://nbj.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lqf.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xrn.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kbn.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://anr.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tzj.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wkl.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hzp.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://znn.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://cyi.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ymx.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eps.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tqg.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://woy.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://spm.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://atw.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rko.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sll.nwbrower.top

[D26] 数组转字符串
来源：http://sbq.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://xhf.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://kri.hnxiangtu.top

JS:   arr.join(", ")
来源：http://pcy.yfazqb.com

TS:   arr.join(", ")
来源：http://qqw.zycfv.cn

Java: String.join(", ", list)
来源：http://pbj.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://xew.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://jlj.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://iqs.guowangkeji.top

================================================================================
来源：http://ggw.jqgfzy.top

E. 字符串处理
来源：http://axj.yfazqb.com

================================================================================
来源：http://qgi.wangdashe.top

[E01] 拼接字符串
来源：http://yqy.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zot.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wfp.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvk.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uwg.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cyp.zhixingplan.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://krc.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pfr.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qwz.aibaodan.cn

[E02] 重复字符串
来源：http://eja.zdbjq.cn

Py:   "ab" * 3
来源：http://lwv.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://fqu.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://mfs.mhx1999.top

TS:   "ab".repeat(3)
来源：http://siv.xziqi.cn

Java: "ab".repeat(3)
来源：http://dei.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://mhh.smart0.xyz

Ruby: "ab" * 3
来源：http://xwg.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fkr.hnxiangtu.top

[E03] 截取子串
来源：http://rdb.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ccj.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jvr.ybcxt.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mgv.shanyushiyangtech.top

TS:   s.slice(1, 4)
来源：http://dbx.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://dcu.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pye.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://hyb.sjlbkw.cn

C#:   s.Substring(1, 3)
来源：http://ang.hnqzz.top

[E04] 查找子串位置
来源：http://tjj.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://vqi.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://fju.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://brg.snrcjt.cn

TS:   s.indexOf("x")
来源：http://bhs.hysaishi.cn

Java: s.indexOf("x")
来源：http://exa.pycfn.com

Go:   strings.Index(s, "x")
来源：http://yvq.0kj1m.cn

Ruby: s.index("x")
来源：http://cpl.hesvh.cn

C#:   s.IndexOf("x")
来源：http://gti.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://edt.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://you.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ouc.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fmh.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://kve.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zmm.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pph.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gxk.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sre.dianchejie.cn

[E06] 替换子串
来源：http://jhf.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wdt.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://onv.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iix.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://wep.jianghu66.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://toq.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gfr.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aym.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://jbf.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://bcd.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lkw.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ykl.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ybz.bjfxy.top

TS:   s.split(",")
来源：http://gwy.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://ora.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dds.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://mki.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fco.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://snu.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://cgb.hfpthk.cn

PHP:  implode(",", $items);
来源：http://wtq.0kj1m.cn

JS:   items.join(",")
来源：http://ubp.52xcode.cn

TS:   items.join(",")
来源：http://aqd.fehbvm.com

Java: String.join(",", items)
来源：http://zac.hfpthk.cn

Go:   strings.Join(items, ",")
来源：http://rrd.52xcode.cn

Ruby: items.join(",")
来源：http://rss.fehbvm.com

C#:   string.Join(",", items)
来源：http://lfs.zycfv.cn

[E09] 去除所有空白字符
来源：http://gzr.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://igp.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sma.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://bcn.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://kyo.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://ooo.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mvi.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://rft.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bed.xuetiantiany.cn


<!-- 参考信息 -->