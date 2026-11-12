代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://szg.feifeiyinyue.top

Java: list.add(0, 0);
来源：http://tup.c1oappe.top

Go:   arr = append([]int{0}, arr...)
来源：http://pht.jyoumei.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gin.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://yoz.aibaodan.cn

[D04] 删除元素
来源：http://lsu.0kj1m.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tfm.yj20258888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rpw.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ieb.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://lse.xylfe.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ntf.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dxa.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pxt.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://whg.pycfn.com

[D05] 访问与修改元素
来源：http://sdm.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spv.yuanzhike.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gat.daria6918.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iaz.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://xqr.sxryk.cn

Java: list.get(0); list.set(0, 9);
来源：http://pob.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://amr.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bda.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cwu.zhaomingkeji.xyz

[D06] 数组长度
来源：http://ppf.yueranfly.top

Py:   len(arr)
来源：http://fii.cheryme.top

PHP:  count($arr);
来源：http://uko.fengsongda.top

JS:   arr.length
来源：http://yee.yj20258888.top

TS:   arr.length
来源：http://vlu.ydzc1.top

Java: list.size();
来源：http://abn.jinqigfzy.top

Go:   len(arr)
来源：http://bpx.yj20258.top

Ruby: arr.length; arr.size
来源：http://qqk.yvedp.cn

C#:   list.Count;
来源：http://cya.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://wka.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qjq.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://upb.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://xgw.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://eoh.pengpengdd.cyou

Java: list.subList(1, 4);
来源：http://bzn.yuxming.cn

Go:   arr[1:4]
来源：http://gvf.andypj.xyz

Ruby: arr[1, 3]
来源：http://oly.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://gha.pycfn.com

[D08] 合并两个数组
来源：http://icu.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://utu.hnqzz.top

PHP:  array_merge($a, $b);
来源：http://adn.cucudq.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://npb.mhx1999.top

TS:   [...a, ...b];
来源：http://fqd.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lvr.sufxvd.cn

Go:   append(a, b...)
来源：http://str.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://gwy.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://tka.shangyingyoupin.top

[D09] 排序（升序）
来源：http://tck.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://njn.9152youxi.cn

PHP:  sort($arr);
来源：http://lis.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gce.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ifv.ppjwa.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jva.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wqw.kuanghao11.cn

Ruby: arr.sort
来源：http://zsa.zhiwuduotai.top

C#:   list.Sort();
来源：http://wcy.xingfuxueyuan.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://mli.zhongyouzk.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lse.yfazqb.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hjd.jyoumei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yfm.xziqi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyl.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://srm.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://llw.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vcb.havefunace.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://epb.yueranfly.top

[D11] 反转数组
来源：http://yns.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lif.vehdjk.com

PHP:  array_reverse($arr);
来源：http://ust.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://thi.zhengqikj.top

TS:   [...arr].reverse();
来源：http://ixq.zdbjq.cn

Java: Collections.reverse(list);
来源：http://krl.c1oappe.top

Go:   slices.Reverse(arr)
来源：http://ziz.zhoulong.xyz

Ruby: arr.reverse
来源：http://yfw.fzhhl.top

C#:   list.Reverse();
来源：http://sye.316326.xyz

[D12] 查找元素下标
来源：http://xth.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://gqh.yj202588.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bft.xziqi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tnw.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fsl.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zfa.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://jge.xingfuxueyuan.xyz

Ruby: arr.index(x)
来源：http://vmp.yfazqb.com

C#:   list.IndexOf(x);
来源：http://zji.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://tdk.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cxm.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yvd.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://tgu.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://wza.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ycr.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qts.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xlk.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ugb.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://tam.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ouo.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://enk.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://hqk.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://ftt.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ogk.zhongyouzk.top

Go:   // 手写循环
来源：http://xwb.gotoacloud.top

Ruby: arr.map { |x| x * 2 }
来源：http://fli.jinqigufen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nkj.gzhubu.top

[D15] 去重
来源：http://xlb.aibaodan.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mro.cheryme.top

PHP:  array_unique($arr);
来源：http://oul.vehdjk.com

JS:   [...new Set(arr)]
来源：http://svz.gzhubu.top

TS:   [...new Set(arr)]
来源：http://qxf.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dwx.zhijiandao.cn

Go:   // 用 map[T]struct{} 手写
来源：http://deh.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://znl.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://fyj.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://dye.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysx.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lhn.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cge.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://atp.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uke.hongshengwenyu.top

Go:   // 手写循环累加
来源：http://mdj.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fon.nanxinkj.top

C#:   list.Sum();  list.Average()
来源：http://pjz.yj20258888.top

[D17] 最大值与最小值
来源：http://dku.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://jxu.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://vln.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xai.fengsongda.top

TS:   Math.max(...arr);
来源：http://usu.svipenyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bvi.bbcook.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kfq.kuanghao11.cn

Ruby: arr.max;  arr.min
来源：http://ppv.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://wmx.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://hwq.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://grw.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://mmz.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://abz.chenzaomai.com

TS:   nested.flat();
来源：http://fcl.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pxq.hysaishi.cn

Go:   // 手写双层循环
来源：http://otn.zhengqikj.top

Ruby: nested.flatten
来源：http://usi.52xcode.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://svb.yj20258.top

[D19] 按字段分组
来源：http://bpm.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qbf.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uga.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://luk.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lqq.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ufr.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://arm.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://swm.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xbe.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://jrd.hongshengwenyu.top

Py:   Counter(arr)
来源：http://ytn.pycfn.com

PHP:  array_count_values($arr);
来源：http://uil.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qao.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://amt.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zxj.cdnleiting.top

Go:   // 手写 map[T]int
来源：http://muk.zhongyouzk.top

Ruby: arr.tally
来源：http://ram.yangfankeji.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pcf.xziqi.cn

[D21] 判断是否包含某元素
来源：http://lpl.zhixingplan.top

Py:   x in arr
来源：http://kqp.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://jwb.ydjk.org.cn

JS:   arr.includes(x)
来源：http://brq.vehdjk.com

TS:   arr.includes(x)
来源：http://nst.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://bos.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://oum.zhixingplan.top

Ruby: arr.include?(x)
来源：http://nef.yvedp.cn

C#:   list.Contains(x)
来源：http://hsn.cdnleiting.top

[D22] 复制数组（避免共享引用）
来源：http://hqj.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ugl.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uah.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wmf.sxryk.cn

TS:   [...arr];
来源：http://was.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://cxz.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xtj.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://nyk.gaohongyu789.top

C#:   new List<int>(list);
来源：http://vvr.fehbvm.com

[D23] reduce 累积计算
来源：http://isw.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dot.shzxlz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cly.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jcq.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wgl.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yhe.xinyue.icu

Go:   // 手写循环
来源：http://eyy.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uhr.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wwn.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://vmj.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://diu.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jhk.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://weq.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nls.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mof.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dbq.zhengqikj.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xqg.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tcd.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://inu.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://upm.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://svt.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mkj.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mdg.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://raw.ydjk.org.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://exb.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zau.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fag.aibaodan.cn

[D26] 数组转字符串
来源：http://kuk.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://ljm.yonumen.top

PHP:  implode(", ", $arr);
来源：http://sbp.birdmap.top

JS:   arr.join(", ")
来源：http://ydr.redwolf501.top

TS:   arr.join(", ")
来源：http://ezh.cdnleiting.top

Java: String.join(", ", list)
来源：http://zfl.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://yqa.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://gft.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://jbi.guowangkeji.top

================================================================================
来源：http://ngv.hysaishi.cn

E. 字符串处理
来源：http://fqc.hcnkem.com

================================================================================
来源：http://vwi.uphjek.com

[E01] 拼接字符串
来源：http://xfw.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mtn.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bkb.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eue.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://obd.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yrx.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://afq.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qde.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mym.jlsjyb.cn

[E02] 重复字符串
来源：http://jed.nanxinkj.top

Py:   "ab" * 3
来源：http://fmu.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://fsg.hysaishi.cn

JS:   "ab".repeat(3)
来源：http://pdg.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://jgc.fengsongda.top

Java: "ab".repeat(3)
来源：http://tnj.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://sot.yanxiufei.cn

Ruby: "ab" * 3
来源：http://tkb.yongpay.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vvx.tianlin.xyz

[E03] 截取子串
来源：http://mtf.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://klx.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cyl.tarul.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hgj.yueranfly.top

TS:   s.slice(1, 4)
来源：http://bzf.daria6918.cn

Java: s.substring(1, 4)
来源：http://wne.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jwt.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://hud.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://siy.52xcode.cn

[E04] 查找子串位置
来源：http://cjg.sysykeji.top

Py:   s.find("x");  s.index("x")
来源：http://zqe.nanxinkj.top

PHP:  strpos($s, "x");
来源：http://qfa.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vkn.aibaodan.cn

TS:   s.indexOf("x")
来源：http://fwo.ydjk.org.cn

Java: s.indexOf("x")
来源：http://aad.dianchejie.cn

Go:   strings.Index(s, "x")
来源：http://ryr.wangshuangyany.cn

Ruby: s.index("x")
来源：http://oyv.nwbrower.top

C#:   s.IndexOf("x")
来源：http://sxp.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ivx.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ofd.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ume.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vgf.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yze.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pjn.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hup.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://owa.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ryv.fehbvm.com

[E06] 替换子串
来源：http://hmt.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wwo.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://aql.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://klg.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://gsw.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zjz.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mkt.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://foe.jiagoushi.top

C#:   s.Replace("a", "b")
来源：http://uiv.0kj1m.cn

[E07] 按分隔符拆分
来源：http://hpb.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rmx.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ynu.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cho.smart0.xyz

TS:   s.split(",")
来源：http://nbo.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://ohp.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jbz.316326.xyz

Ruby: s.split(",");  s.split
来源：http://iim.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://usg.uphjek.com

[E08] 数组按分隔符合并
来源：http://zsn.ydzc1.top

Py:   ",".join(items)
来源：http://xhz.iojbl.cn

PHP:  implode(",", $items);
来源：http://xlj.mhx1999.top

JS:   items.join(",")
来源：http://pfp.zhixingplan.top

TS:   items.join(",")
来源：http://qzn.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://fdw.yonumen.top

Go:   strings.Join(items, ",")
来源：http://edo.mhx1999.top

Ruby: items.join(",")
来源：http://sba.uphjek.com

C#:   string.Join(",", items)
来源：http://vga.hnqzz.top

[E09] 去除所有空白字符
来源：http://rin.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zyo.316326.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wyo.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://nyb.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://iqw.iojbl.cn

Java: s.replaceAll("\\s+", "")
来源：http://mdf.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mnd.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rjv.bjfxy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://scj.nwbrower.top

[E10] 左侧补零 / 定长填充
来源：http://vut.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bwc.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://haw.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://skw.tianlin.xyz


<!-- 参考信息 -->