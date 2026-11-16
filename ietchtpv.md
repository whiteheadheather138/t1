代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vvs.zhijiandao.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wxp.9152youxi.cn

TS:   arr[0]; arr.at(-1);
来源：http://xmv.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://dce.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://viz.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mil.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zdp.hywenlv.cn

[D06] 数组长度
来源：http://fmm.smart0.xyz

Py:   len(arr)
来源：http://isd.uphjek.com

PHP:  count($arr);
来源：http://hws.vehdjk.com

JS:   arr.length
来源：http://uex.jyoumei.cn

TS:   arr.length
来源：http://hty.feifeiyinyue.top

Java: list.size();
来源：http://viz.316326.xyz

Go:   len(arr)
来源：http://rqs.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://qxn.dashuyun.cn

C#:   list.Count;
来源：http://dzt.xuetiantiany.cn

[D07] 切片 / 取子数组
来源：http://mhz.0kj1m.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://key.jianghu66.top

PHP:  array_slice($arr, 1, 3);
来源：http://jwv.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://qij.cashguo.top

TS:   arr.slice(1, 4);
来源：http://bgi.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://rvb.daria6918.cn

Go:   arr[1:4]
来源：http://jqj.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://bcu.jinghuilouyu.cn

C#:   list.GetRange(1, 3);
来源：http://vza.ydzc1.top

[D08] 合并两个数组
来源：http://rly.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://ycn.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://auq.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://blr.yangfankeji.com

TS:   [...a, ...b];
来源：http://bhh.zhijiandao.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bar.jlsjyb.cn

Go:   append(a, b...)
来源：http://app.daria6918.cn

Ruby: a + b;  a.concat(b)
来源：http://ijq.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://awo.hfpthk.cn

[D09] 排序（升序）
来源：http://qkt.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://ged.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://zmt.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tif.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ojm.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://uxj.0kj1m.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lwd.zhongyouzk.top

Ruby: arr.sort
来源：http://fwm.ehwqpu.com

C#:   list.Sort();
来源：http://cgq.yongpay.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bso.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hzo.hongshengwenyu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hqr.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://imm.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jqo.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://acw.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ebw.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xpt.meibo888.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sxb.uphjek.com

[D11] 反转数组
来源：http://dwa.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jrr.epnwcf.com

PHP:  array_reverse($arr);
来源：http://ajc.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xdt.snrcjt.cn

TS:   [...arr].reverse();
来源：http://bdg.fehbvm.com

Java: Collections.reverse(list);
来源：http://lcn.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://ekr.wangdashe.top

Ruby: arr.reverse
来源：http://jgr.hysaishi.cn

C#:   list.Reverse();
来源：http://xir.wangdashe.top

[D12] 查找元素下标
来源：http://sge.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://tve.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jnq.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikz.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osa.zdbjq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bky.ivvv.top

Go:   slices.Index(arr, x)
来源：http://mxe.yonumen.top

Ruby: arr.index(x)
来源：http://vel.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://urs.redwolf501.top

[D13] 过滤（保留满足条件的）
来源：http://krk.zhengqikj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://low.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hwb.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://oco.yuanzhike.top

TS:   arr.filter(x => x > 3)
来源：http://kxv.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://isf.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uif.aizwys.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dio.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://njq.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://jqk.fengsongda.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dhw.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vmy.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://cot.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://ney.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vua.fktsv.cn

Go:   // 手写循环
来源：http://vwo.xziqi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ojm.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gwt.316326.xyz

[D15] 去重
来源：http://xhb.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://syr.yonumen.top

PHP:  array_unique($arr);
来源：http://tik.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://edz.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://pbm.daxiang520.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xhx.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cfo.daxiang520.top

Ruby: arr.uniq
来源：http://nkw.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://egi.ydjk.org.cn

[D16] 求和与平均值
来源：http://jvk.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jfs.cucudq.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kpo.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://psn.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ocz.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vcy.ctjpmb.com

Go:   // 手写循环累加
来源：http://sgk.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aul.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://tjt.daria6918.cn

[D17] 最大值与最小值
来源：http://vnc.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://vqs.zycfv.cn

PHP:  max($arr);  min($arr);
来源：http://agq.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rik.jinyuanbaomall.cn

TS:   Math.max(...arr);
来源：http://dux.chenjidiqi.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://vdv.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ekl.sweek.top

Ruby: arr.max;  arr.min
来源：http://ahu.shangyingyoupin.top

C#:   list.Max();  list.Min()
来源：http://xxl.cheryme.top

[D18] 扁平化嵌套数组
来源：http://aox.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cxt.yonumen.top

PHP:  array_merge(...$nested);
来源：http://jml.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aaj.yvedp.cn

TS:   nested.flat();
来源：http://pzy.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dfa.yj20258888.top

Go:   // 手写双层循环
来源：http://gcg.52xcode.cn

Ruby: nested.flatten
来源：http://nbc.sysykeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://npm.fengsongda.top

[D19] 按字段分组
来源：http://wmd.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tej.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eli.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tqy.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pet.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hsx.sweek.top

Go:   // 手写 map[string][]T
来源：http://gfm.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lst.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oic.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://opa.cucudq.cn

Py:   Counter(arr)
来源：http://uuo.shuidangran.top

PHP:  array_count_values($arr);
来源：http://szk.52xcode.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqz.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nde.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hqv.nwbrower.top

Go:   // 手写 map[T]int
来源：http://wuo.guannengcc.top

Ruby: arr.tally
来源：http://fcn.shuidangran.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zlt.fktsv.cn

[D21] 判断是否包含某元素
来源：http://qia.0kj1m.cn

Py:   x in arr
来源：http://rva.tian-w.cn

PHP:  in_array($x, $arr, true);
来源：http://nkw.bjfxy.top

JS:   arr.includes(x)
来源：http://eut.sxryk.cn

TS:   arr.includes(x)
来源：http://ixx.cqqwz.cn

Java: list.contains(x)
来源：http://wfv.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://qli.zhengqikj.top

Ruby: arr.include?(x)
来源：http://vor.zdbjq.cn

C#:   list.Contains(x)
来源：http://hwn.yuanzhike.top

[D22] 复制数组（避免共享引用）
来源：http://qvb.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qxi.cqqwz.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cqa.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xwn.shanyushiyangkeji.top

TS:   [...arr];
来源：http://bss.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://val.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://ylq.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://hqc.dianchejie.cn

C#:   new List<int>(list);
来源：http://ynk.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://wuw.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sit.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gif.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://udq.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zmx.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wpc.hywenlv.cn

Go:   // 手写循环
来源：http://jud.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mrp.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rxt.hfpthk.cn

[D24] 字典 / Map 基本操作
来源：http://wrj.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ekf.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://evs.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mru.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kvw.kuanghao11.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lrp.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kzk.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://glw.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kfr.ydjk.org.cn

[D25] Set 集合去重与交并差
来源：http://atp.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xdz.hfpthk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wza.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wgb.52xcode.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://urx.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jsy.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lth.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aef.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wam.cashguo.top

[D26] 数组转字符串
来源：http://vgz.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://hym.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://abh.sufxvd.cn

JS:   arr.join(", ")
来源：http://vdw.hcnkem.com

TS:   arr.join(", ")
来源：http://hfq.jlsjyb.cn

Java: String.join(", ", list)
来源：http://plx.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://syf.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://ugz.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://pxw.bjfxy.top

================================================================================
来源：http://enw.ywan-chungtsiang.top

E. 字符串处理
来源：http://qxv.aibaodan.cn

================================================================================
来源：http://emf.cqqwz.cn

[E01] 拼接字符串
来源：http://bvz.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ypw.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vgk.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hzd.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cir.zhixingplan.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ibi.dianchejie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vbj.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bno.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cld.fzhhl.top

[E02] 重复字符串
来源：http://bzj.feifeiyinyue.top

Py:   "ab" * 3
来源：http://uva.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://wie.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://aas.xinyue.icu

TS:   "ab".repeat(3)
来源：http://gxb.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://fhy.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://xpo.ydjk.org.cn

Ruby: "ab" * 3
来源：http://lxm.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vzu.zhaomingkeji.xyz

[E03] 截取子串
来源：http://ghl.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yod.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vhl.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fgx.fzhhl.top

TS:   s.slice(1, 4)
来源：http://mzx.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://zpy.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rak.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://ocg.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://vbc.tian-w.cn

[E04] 查找子串位置
来源：http://bmh.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://eny.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://ydg.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://smw.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://aop.bbcook.cn

Java: s.indexOf("x")
来源：http://hpn.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://lic.gogol.net.cn

Ruby: s.index("x")
来源：http://feo.gzhubu.top

C#:   s.IndexOf("x")
来源：http://skl.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nti.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hio.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xfu.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fbe.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cor.cdnleiting.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wsb.yongpay.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cdq.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ysm.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vlz.jlsjyb.cn

[E06] 替换子串
来源：http://sdg.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lyu.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://tbj.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rry.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://clj.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpj.gzhubu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jwf.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wle.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://mom.jyoumei.cn

[E07] 按分隔符拆分
来源：http://mmv.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wyy.daria6918.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xsw.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gkw.zdbjq.cn

TS:   s.split(",")
来源：http://jbq.9152youxi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hbb.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kep.pycfn.com

Ruby: s.split(",");  s.split
来源：http://ezq.316326.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iza.tian-w.cn

[E08] 数组按分隔符合并
来源：http://gxx.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://hig.xylfe.cn

PHP:  implode(",", $items);
来源：http://lix.52xcode.cn

JS:   items.join(",")
来源：http://evm.hnxiangtu.top

TS:   items.join(",")
来源：http://nxm.sjlbkw.cn

Java: String.join(",", items)
来源：http://ghj.tanke756.top

Go:   strings.Join(items, ",")
来源：http://bfj.shanyushiyangtech.top

Ruby: items.join(",")
来源：http://ron.shanyushiyangtech.top

C#:   string.Join(",", items)
来源：http://zyo.svipenyu.cn

[E09] 去除所有空白字符
来源：http://cya.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sen.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dwc.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://tra.yonumen.top

TS:   s.replace(/\s+/g, "")
来源：http://ufw.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://odi.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jqx.jlsjyb.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cto.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tpg.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://bhr.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fes.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dte.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://loa.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://abi.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://ybc.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qmd.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zzs.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qkh.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://bel.jqgfzy.top

Py:   s[::-1]
来源：http://xck.cashguo.top

PHP:  strrev($s);
来源：http://rkm.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://ehc.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://oac.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ems.sweek.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tny.jinghuilouyu.cn

Ruby: s.reverse
来源：http://wlo.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rdi.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://kbz.redwolf501.top

Py:   s.count("a")
来源：http://sph.daxiang520.top


<!-- 参考信息 -->