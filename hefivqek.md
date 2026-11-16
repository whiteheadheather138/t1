代发 wailian999

Java: list.add(4);
来源：http://vab.jlsjyb.cn

Go:   arr = append(arr, 4)
来源：http://piu.nanxuanxn.top

Ruby: arr << 4; arr.push(5)
来源：http://tmx.fzhhl.top

C#:   list.Add(4);
来源：http://ala.cdnleiting.top

[D03] 在指定位置插入元素
来源：http://yjd.ydzc1.top

Py:   arr.insert(0, 0)
来源：http://kwk.chenjidiqi.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://taw.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xvc.316326.xyz

TS:   arr.splice(0, 0, 0);
来源：http://kky.dashuyun.cn

Java: list.add(0, 0);
来源：http://qnx.zhaomingkeji.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://uwj.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://let.gotoacloud.top

C#:   list.Insert(0, 0);
来源：http://qii.bbcook.cn

[D04] 删除元素
来源：http://epp.fanxiaobao.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fbl.hammf.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ntv.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://csi.cheryme.top

TS:   arr.splice(0, 1);
来源：http://hyy.tianlin.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://clr.sysykeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://suf.9152youxi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kyh.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ozk.hongshengwenyu.top

[D05] 访问与修改元素
来源：http://vmm.ywan-chungtsiang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://elg.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uvv.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://icj.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://xgi.shangyingyoupin.top

Java: list.get(0); list.set(0, 9);
来源：http://cnc.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://dlv.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mdf.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mzg.gzhubu.top

[D06] 数组长度
来源：http://xvj.sjlbkw.cn

Py:   len(arr)
来源：http://ssv.hysaishi.cn

PHP:  count($arr);
来源：http://erh.zhiwuduotai.top

JS:   arr.length
来源：http://mdp.fengsongda.top

TS:   arr.length
来源：http://nsx.zhongyouzk.top

Java: list.size();
来源：http://ylk.cashguo.top

Go:   len(arr)
来源：http://ent.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://wfv.havefunace.top

C#:   list.Count;
来源：http://jlr.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://rep.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vfa.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ctg.yonumen.top

JS:   arr.slice(1, 4);
来源：http://pga.hammf.cn

TS:   arr.slice(1, 4);
来源：http://eob.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://mnz.ppjwa.cn

Go:   arr[1:4]
来源：http://gqu.ehwqpu.com

Ruby: arr[1, 3]
来源：http://yfa.ivvv.top

C#:   list.GetRange(1, 3);
来源：http://pno.fktsv.cn

[D08] 合并两个数组
来源：http://nlp.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://lls.shanyushiyangtech.top

PHP:  array_merge($a, $b);
来源：http://wfy.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lnh.zycfv.cn

TS:   [...a, ...b];
来源：http://her.yueranfly.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zme.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://kco.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://xns.xziqi.cn

C#:   a.Concat(b).ToList()
来源：http://lem.hysaishi.cn

[D09] 排序（升序）
来源：http://bkj.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ypi.zhixingplan.top

PHP:  sort($arr);
来源：http://ubj.hywenlv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lcy.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://qon.yvedp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rsd.ywan-chungtsiang.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gbn.zdqjudy.top

Ruby: arr.sort
来源：http://ulp.zhixingplan.top

C#:   list.Sort();
来源：http://qui.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://flp.yuxming.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yun.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrx.chenjidiqi.icu

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ayl.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zsq.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xjp.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://stl.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yvf.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kou.meibo888.top

[D11] 反转数组
来源：http://zuy.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ccj.hnqzz.top

PHP:  array_reverse($arr);
来源：http://ect.fzhhl.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tim.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://qeu.wangdashe.top

Java: Collections.reverse(list);
来源：http://cmp.fzhhl.top

Go:   slices.Reverse(arr)
来源：http://fqn.guowangkeji.top

Ruby: arr.reverse
来源：http://arq.yj202588.top

C#:   list.Reverse();
来源：http://div.xuanzx.com

[D12] 查找元素下标
来源：http://zwb.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://vqj.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dhp.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hvu.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykn.hnqzz.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wko.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://grw.yvedp.cn

Ruby: arr.index(x)
来源：http://ait.hnqzz.top

C#:   list.IndexOf(x);
来源：http://czt.hfpthk.cn

[D13] 过滤（保留满足条件的）
来源：http://vro.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vrv.quarkkingdee.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ssp.wangshuangyany.cn

JS:   arr.filter(x => x > 3)
来源：http://ava.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://fma.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://otg.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cfc.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://ets.hesvh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mkk.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://quj.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dic.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mke.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://urf.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://hhx.hcnkem.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://rhq.jqgufenzy.top

Go:   // 手写循环
来源：http://xcz.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://noz.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://nrt.gzhubu.top

[D15] 去重
来源：http://sbz.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cda.cucudq.cn

PHP:  array_unique($arr);
来源：http://mey.cheryme.top

JS:   [...new Set(arr)]
来源：http://goa.andypj.xyz

TS:   [...new Set(arr)]
来源：http://lnt.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hbg.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://vkp.hcnkem.com

Ruby: arr.uniq
来源：http://nqz.316326.xyz

C#:   list.Distinct().ToList()
来源：http://dko.fehbvm.com

[D16] 求和与平均值
来源：http://kcv.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zjb.pycfn.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jfo.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://llb.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zpz.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://imi.chenlongwang.top

Go:   // 手写循环累加
来源：http://vus.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zyl.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://aiv.jqgufenzy.top

[D17] 最大值与最小值
来源：http://pde.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://qse.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://spd.yanxiufei.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rzs.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://bpb.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lyp.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lah.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://jld.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://ews.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://zga.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ujy.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://ecr.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://siz.jlsjyb.cn

TS:   nested.flat();
来源：http://xkp.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kmu.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://mpz.shzxlz.cn

Ruby: nested.flatten
来源：http://xej.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xgx.zhongyouzk.top

[D19] 按字段分组
来源：http://sir.zhoulong.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hyy.yanxiufei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cql.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://itk.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://rrx.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bjb.birdmap.top

Go:   // 手写 map[string][]T
来源：http://ydj.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ogu.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ijw.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://osd.chenjidiqi.icu

Py:   Counter(arr)
来源：http://snn.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://fdu.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gle.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://psz.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mpl.yj20258.top

Go:   // 手写 map[T]int
来源：http://bbw.ydzc1.top

Ruby: arr.tally
来源：http://vgt.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://obv.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://piu.zhengqikj.top

Py:   x in arr
来源：http://pbr.yangfankeji.com

PHP:  in_array($x, $arr, true);
来源：http://udz.vehdjk.com

JS:   arr.includes(x)
来源：http://beq.fehbvm.com

TS:   arr.includes(x)
来源：http://nhj.yj20258.top

Java: list.contains(x)
来源：http://ely.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://drk.shzxlz.cn

Ruby: arr.include?(x)
来源：http://twx.jinqigufen.top

C#:   list.Contains(x)
来源：http://cgh.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://lca.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qpy.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://irr.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mfo.daxiang520.top

TS:   [...arr];
来源：http://hwk.fktsv.cn

Java: new ArrayList<>(list);
来源：http://rkp.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kgb.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://fyp.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://dar.yj20258888.top

[D23] reduce 累积计算
来源：http://wtu.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ucz.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mhb.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hpu.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zdi.shanyushiyangtech.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://jbq.hammf.cn

Go:   // 手写循环
来源：http://blv.hysaishi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fxw.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lmx.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://vxs.yanxiufei.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rlw.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ylr.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://trx.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://svs.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://itr.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ixm.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qke.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dqo.shzxlz.cn

[D25] Set 集合去重与交并差
来源：http://rky.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zlp.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qcc.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rky.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xea.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nre.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ffj.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://czl.9152youxi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rcu.epnwcf.com

[D26] 数组转字符串
来源：http://uim.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://bou.birdmap.top

PHP:  implode(", ", $arr);
来源：http://gms.quarkkingdee.top

JS:   arr.join(", ")
来源：http://czy.zycfv.cn

TS:   arr.join(", ")
来源：http://hvt.zycfv.cn

Java: String.join(", ", list)
来源：http://top.chenjidiqi.icu

Go:   strings.Join(strs, ", ")
来源：http://ohe.ivvv.top

Ruby: arr.join(", ")
来源：http://joa.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://vyg.daria6918.cn

================================================================================
来源：http://zsx.yuanzhike.top

E. 字符串处理
来源：http://vpf.yj202588.top

================================================================================
来源：http://kum.vqdsnc.cn

[E01] 拼接字符串
来源：http://bkf.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zsk.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xwu.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rso.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsr.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://okb.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://brj.sjlbkw.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rnp.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xjy.hnxiangtu.top

[E02] 重复字符串
来源：http://tot.9152youxi.cn

Py:   "ab" * 3
来源：http://dwu.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://rvf.yvedp.cn

JS:   "ab".repeat(3)
来源：http://pad.ydzc1.top

TS:   "ab".repeat(3)
来源：http://ege.gogol.net.cn

Java: "ab".repeat(3)
来源：http://soe.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://tmz.hnqzz.top

Ruby: "ab" * 3
来源：http://xbb.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://won.redwolf501.top

[E03] 截取子串
来源：http://mae.0kj1m.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wbb.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qva.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tne.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://qod.nwbrower.top

Java: s.substring(1, 4)
来源：http://gpb.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qju.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xww.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://kod.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://ozv.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://pew.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://qnj.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://amo.cucudq.cn

TS:   s.indexOf("x")
来源：http://mqi.hysaishi.cn

Java: s.indexOf("x")
来源：http://ipa.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://zys.shangyingyoupin.top

Ruby: s.index("x")
来源：http://ahx.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://bli.hysaishi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bxj.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://phn.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zaz.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kpo.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zau.redwolf501.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://otj.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bfx.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mzj.yj20258.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rny.c1oappe.top

[E06] 替换子串
来源：http://rby.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pox.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://ldg.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nsc.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://riv.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://syj.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pru.ydzc1.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aph.tarul.cn

C#:   s.Replace("a", "b")
来源：http://wix.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://iga.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://itl.jqgfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://moy.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ydj.guannengcc.top

TS:   s.split(",")
来源：http://caw.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://ygc.xinyue.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tjx.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://juz.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sue.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://rhl.yongpay.top

Py:   ",".join(items)
来源：http://adf.uphjek.com

PHP:  implode(",", $items);
来源：http://zfi.havefunace.top

JS:   items.join(",")
来源：http://ucd.yanxiufei.cn

TS:   items.join(",")
来源：http://yac.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://puz.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://pyt.hfpthk.cn

Ruby: items.join(",")
来源：http://mms.jianghu66.top

C#:   string.Join(",", items)
来源：http://mpr.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://btv.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hcx.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nqz.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://xej.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://niz.yueranfly.top


<!-- 参考信息 -->