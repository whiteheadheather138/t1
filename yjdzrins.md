代发 wailian999

Java: list.add(4);
来源：http://sbt.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://gae.andypj.xyz

Ruby: arr << 4; arr.push(5)
来源：http://kcl.xylfe.cn

C#:   list.Add(4);
来源：http://bep.cashguo.top

[D03] 在指定位置插入元素
来源：http://fut.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://vmb.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fdt.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://whx.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://gdl.redwolf501.top

Java: list.add(0, 0);
来源：http://nrt.xingfuxueyuan.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fvq.fengsongda.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qpa.zycfv.cn

C#:   list.Insert(0, 0);
来源：http://kma.jinqigfzy.top

[D04] 删除元素
来源：http://qvw.gotoacloud.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mpy.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kiz.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lph.pycfn.com

TS:   arr.splice(0, 1);
来源：http://jji.fzhhl.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fmg.tanke756.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lea.fehbvm.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uwf.kuanghao11.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://trb.birdmap.top

[D05] 访问与修改元素
来源：http://gxl.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ldr.iojbl.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jtw.yanxiufei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vvb.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://mls.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://idt.hammf.cn

Go:   arr[0]; arr[0] = 9
来源：http://siq.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wgb.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cet.tian-w.cn

[D06] 数组长度
来源：http://hdq.haohaochexian.top

Py:   len(arr)
来源：http://frm.vqdsnc.cn

PHP:  count($arr);
来源：http://ziq.zhijiandao.cn

JS:   arr.length
来源：http://cdd.zhoulong.xyz

TS:   arr.length
来源：http://vjc.sjlbkw.cn

Java: list.size();
来源：http://ccj.yj202588.top

Go:   len(arr)
来源：http://ydg.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://sav.sjlbkw.cn

C#:   list.Count;
来源：http://bsl.redwolf501.top

[D07] 切片 / 取子数组
来源：http://hgc.kuanghao11.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kgj.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://dkb.epnwcf.com

JS:   arr.slice(1, 4);
来源：http://ewb.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://dkc.fktsv.cn

Java: list.subList(1, 4);
来源：http://hwi.aizwys.cn

Go:   arr[1:4]
来源：http://ajv.gzhubu.top

Ruby: arr[1, 3]
来源：http://dpp.ehwqpu.com

C#:   list.GetRange(1, 3);
来源：http://nnm.0kj1m.cn

[D08] 合并两个数组
来源：http://alg.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://ngy.gzhubu.top

PHP:  array_merge($a, $b);
来源：http://wbb.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mju.xziqi.cn

TS:   [...a, ...b];
来源：http://doa.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gvv.chenlongwang.top

Go:   append(a, b...)
来源：http://dde.ivvv.top

Ruby: a + b;  a.concat(b)
来源：http://nfg.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://wkc.52xcode.cn

[D09] 排序（升序）
来源：http://zfb.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://ipt.vehdjk.com

PHP:  sort($arr);
来源：http://cff.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fvb.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://gzp.xuanzx.com

Java: Collections.sort(list);  list.sort(null);
来源：http://byp.shanyushiyangtech.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ury.fengsongda.top

Ruby: arr.sort
来源：http://yrj.xuetiantiany.cn

C#:   list.Sort();
来源：http://qax.hysaishi.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ojd.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zpx.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jtg.bbcook.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cvr.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uoy.pengpengdd.cyou

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gxy.zycfv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tpd.cqqwz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pnr.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vai.xuetiantiany.cn

[D11] 反转数组
来源：http://plc.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zpb.ctjpmb.com

PHP:  array_reverse($arr);
来源：http://xyg.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pcl.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://qce.snrcjt.cn

Java: Collections.reverse(list);
来源：http://ctf.jianghu66.top

Go:   slices.Reverse(arr)
来源：http://seh.aibaodan.cn

Ruby: arr.reverse
来源：http://vkp.yuanzhike.top

C#:   list.Reverse();
来源：http://iow.fzhhl.top

[D12] 查找元素下标
来源：http://fbx.ydjk.org.cn

Py:   arr.index(x);  x in arr
来源：http://jux.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://twn.sufxvd.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qzu.ehwqpu.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ffk.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qnn.guannengcc.top

Go:   slices.Index(arr, x)
来源：http://bby.yj202588.top

Ruby: arr.index(x)
来源：http://okc.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://jir.zdqjudy.top

[D13] 过滤（保留满足条件的）
来源：http://vky.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wsl.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zjq.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://ruy.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://zjp.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://auj.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ivd.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hsm.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rbi.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://xeb.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qhu.tianlin.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dfc.zhaomingkeji.xyz

JS:   arr.map(x => x * 2)
来源：http://sep.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://fvo.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xof.iojbl.cn

Go:   // 手写循环
来源：http://ijc.jqgfzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://lxj.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://crk.yuanzhike.top

[D15] 去重
来源：http://rxx.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kbh.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://opw.fzhhl.top

JS:   [...new Set(arr)]
来源：http://sss.tarul.cn

TS:   [...new Set(arr)]
来源：http://dpl.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tql.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://mix.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://jgx.shzxlz.cn

C#:   list.Distinct().ToList()
来源：http://ian.cdnleiting.top

[D16] 求和与平均值
来源：http://vkc.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zbt.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://elg.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://icu.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ysk.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rkc.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://fde.fanxiaobao.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wyr.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://wul.hammf.cn

[D17] 最大值与最小值
来源：http://nic.redwolf501.top

Py:   max(arr);  min(arr)
来源：http://bjs.yfazqb.com

PHP:  max($arr);  min($arr);
来源：http://lru.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://glo.vehdjk.com

TS:   Math.max(...arr);
来源：http://gzf.zhixingplan.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mkb.zhaomingkeji.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dbt.aizwys.cn

Ruby: arr.max;  arr.min
来源：http://czq.aibaodan.cn

C#:   list.Max();  list.Min()
来源：http://xko.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://jwm.quarkkingdee.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ggz.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://eea.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ujb.hcnkem.com

TS:   nested.flat();
来源：http://dut.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://usk.sufxvd.cn

Go:   // 手写双层循环
来源：http://qrp.epnwcf.com

Ruby: nested.flatten
来源：http://mzm.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://agw.ydjk.org.cn

[D19] 按字段分组
来源：http://czg.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jfs.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://don.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nrb.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://njp.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sus.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://wmy.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uzo.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vfp.ybcxt.top

[D20] 统计每个元素出现次数
来源：http://ken.fktsv.cn

Py:   Counter(arr)
来源：http://vkz.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://fhi.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aeb.0kj1m.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwr.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://izv.jianghu66.top

Go:   // 手写 map[T]int
来源：http://tbs.ivvv.top

Ruby: arr.tally
来源：http://hmk.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://knp.hammf.cn

[D21] 判断是否包含某元素
来源：http://hrs.zhongyouzk.top

Py:   x in arr
来源：http://tzo.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://qpf.hammf.cn

JS:   arr.includes(x)
来源：http://xwp.52xcode.cn

TS:   arr.includes(x)
来源：http://iai.redwolf501.top

Java: list.contains(x)
来源：http://xdo.epnwcf.com

Go:   slices.Contains(arr, x)
来源：http://zdj.jqgfzy.top

Ruby: arr.include?(x)
来源：http://vqk.fktsv.cn

C#:   list.Contains(x)
来源：http://hox.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://cyd.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://djt.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://juq.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://isn.0kj1m.cn

TS:   [...arr];
来源：http://lkx.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://zer.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iph.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://iss.gogol.net.cn

C#:   new List<int>(list);
来源：http://zqx.ehwqpu.com

[D23] reduce 累积计算
来源：http://knc.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ugi.ybcxt.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vyi.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jnc.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pbs.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wne.yangfankeji.com

Go:   // 手写循环
来源：http://wpy.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ldn.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ofp.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://qol.xinyue.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vni.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kpk.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hwj.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pmb.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mgp.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ehj.cdnleiting.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xlm.ppjwa.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ixn.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://cnq.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mhx.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cjj.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xzv.nanxuanxn.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ind.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dyy.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fft.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kkh.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ksu.hfpthk.cn

[D26] 数组转字符串
来源：http://bmx.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://pov.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://gtz.chenzaomai.com

JS:   arr.join(", ")
来源：http://urr.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://rvq.gogol.net.cn

Java: String.join(", ", list)
来源：http://gxi.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://rar.chenzaomai.com

Ruby: arr.join(", ")
来源：http://ocz.sysykeji.top

C#:   string.Join(", ", list)
来源：http://gtw.zdbjq.cn

================================================================================
来源：http://rfn.yj20258888.top

E. 字符串处理
来源：http://jfw.gaohongyu789.top

================================================================================
来源：http://cdw.jianghu66.top

[E01] 拼接字符串
来源：http://gju.cashguo.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zcg.snrcjt.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vpr.yanxiufei.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ttu.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oop.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uvd.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zdg.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cem.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iti.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://rrw.cucudq.cn

Py:   "ab" * 3
来源：http://wde.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://wyq.fzhhl.top

JS:   "ab".repeat(3)
来源：http://wbc.yuxming.cn

TS:   "ab".repeat(3)
来源：http://adl.yj20258888.top

Java: "ab".repeat(3)
来源：http://tzx.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://tpb.cheryme.top

Ruby: "ab" * 3
来源：http://fum.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewd.sweek.top

[E03] 截取子串
来源：http://nju.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vww.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jzo.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://txv.yueranfly.top

TS:   s.slice(1, 4)
来源：http://bae.cucudq.cn

Java: s.substring(1, 4)
来源：http://zif.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gpe.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://rkr.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://crm.fehbvm.com

[E04] 查找子串位置
来源：http://alv.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://pgx.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://iwk.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fnx.zdbjq.cn

TS:   s.indexOf("x")
来源：http://fuv.sweek.top

Java: s.indexOf("x")
来源：http://uhv.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://oew.yj20258888.top

Ruby: s.index("x")
来源：http://zaw.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://qfr.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://lga.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wmm.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uib.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pqt.hcnkem.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bku.hongshengwenyu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hao.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vhz.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zpv.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ttm.havefunace.top

[E06] 替换子串
来源：http://arg.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://thg.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://cks.vqdsnc.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ajt.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://gze.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://spd.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tgz.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hhm.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://vql.c1oappe.top

[E07] 按分隔符拆分
来源：http://znv.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ufh.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zwo.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ekh.shangyingyoupin.top

TS:   s.split(",")
来源：http://udu.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://kqj.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lyd.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://clz.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxm.daria6918.cn

[E08] 数组按分隔符合并
来源：http://dwr.gzhubu.top

Py:   ",".join(items)
来源：http://win.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://ygo.hongshengwenyu.top

JS:   items.join(",")
来源：http://hmp.ivvv.top

TS:   items.join(",")
来源：http://bbv.xziqi.cn

Java: String.join(",", items)
来源：http://exb.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://fph.nanxuanxn.top

Ruby: items.join(",")
来源：http://ikb.fktsv.cn

C#:   string.Join(",", items)
来源：http://rit.vehdjk.com

[E09] 去除所有空白字符
来源：http://ezt.daria6918.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ode.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ejx.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://vss.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://zzv.hnxiangtu.top


<!-- 参考信息 -->