代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://xxz.jiagoushi.top

Java: list.add(0, 0);
来源：http://wgr.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://opc.zycfv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xjr.ppjwa.cn

C#:   list.Insert(0, 0);
来源：http://eng.chenlongwang.top

[D04] 删除元素
来源：http://fnc.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tru.zhongyouzk.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ubf.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://avv.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://qpz.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ynp.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vzp.ybcxt.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://kwv.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nyd.guowangkeji.top

[D05] 访问与修改元素
来源：http://ktz.feifeiyinyue.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rrl.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dct.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dvg.sjlbkw.cn

TS:   arr[0]; arr.at(-1);
来源：http://lra.dianchejie.cn

Java: list.get(0); list.set(0, 9);
来源：http://udk.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://nqp.hongshengwenyu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aoq.gaohongyu789.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zua.jiagoushi.top

[D06] 数组长度
来源：http://ihf.sysykeji.top

Py:   len(arr)
来源：http://vzb.pycfn.com

PHP:  count($arr);
来源：http://uyy.andypj.xyz

JS:   arr.length
来源：http://abq.pycfn.com

TS:   arr.length
来源：http://heq.nwbrower.top

Java: list.size();
来源：http://jwl.cdnleiting.top

Go:   len(arr)
来源：http://trn.andypj.xyz

Ruby: arr.length; arr.size
来源：http://acd.zdqjudy.top

C#:   list.Count;
来源：http://dpo.shuidangran.top

[D07] 切片 / 取子数组
来源：http://iwe.jqgfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ahd.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://uyz.zdqjudy.top

JS:   arr.slice(1, 4);
来源：http://rrs.zhiwuduotai.top

TS:   arr.slice(1, 4);
来源：http://ozt.cqqwz.cn

Java: list.subList(1, 4);
来源：http://tqk.shzxlz.cn

Go:   arr[1:4]
来源：http://bpt.hesvh.cn

Ruby: arr[1, 3]
来源：http://pke.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://ooa.zhoulong.xyz

[D08] 合并两个数组
来源：http://mwv.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://tbd.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://nmd.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://htx.dashuyun.cn

TS:   [...a, ...b];
来源：http://uvn.daria6918.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sra.dianchejie.cn

Go:   append(a, b...)
来源：http://few.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://xdn.ctjpmb.com

C#:   a.Concat(b).ToList()
来源：http://fjo.jlsjyb.cn

[D09] 排序（升序）
来源：http://btp.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://zuu.hnxiangtu.top

PHP:  sort($arr);
来源：http://oqp.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vgg.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mlc.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dpi.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zqu.jqgfzy.top

Ruby: arr.sort
来源：http://kbj.guowangkeji.top

C#:   list.Sort();
来源：http://cac.jinqigufen.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nfi.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mcv.shanyushiyangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhv.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kce.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bhc.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uct.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://psh.vqdsnc.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gph.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dfd.yongpay.top

[D11] 反转数组
来源：http://qpq.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://xpf.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://ssv.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ubc.shzxlz.cn

TS:   [...arr].reverse();
来源：http://zxj.zhixingplan.top

Java: Collections.reverse(list);
来源：http://nwb.havefunace.top

Go:   slices.Reverse(arr)
来源：http://tyk.cqqwz.cn

Ruby: arr.reverse
来源：http://uvg.yj202588.top

C#:   list.Reverse();
来源：http://dow.haohaochexian.top

[D12] 查找元素下标
来源：http://cii.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://xat.tianlin.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gkx.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ltu.nwbrower.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wxx.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://aja.svipenyu.cn

Go:   slices.Index(arr, x)
来源：http://gpy.cashguo.top

Ruby: arr.index(x)
来源：http://grd.chenlongwang.top

C#:   list.IndexOf(x);
来源：http://rca.fengsongda.top

[D13] 过滤（保留满足条件的）
来源：http://udj.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yqn.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://psh.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://lqs.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://yda.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qvt.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pqa.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tka.hysaishi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fvr.hnqzz.top

[D14] 映射转换（每个元素变形）
来源：http://npr.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pfq.xylfe.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ccp.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://act.ybcxt.top

TS:   arr.map(x => x * 2)
来源：http://gcj.chenlongwang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tdl.ydjk.org.cn

Go:   // 手写循环
来源：http://qsw.fehbvm.com

Ruby: arr.map { |x| x * 2 }
来源：http://coh.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gas.zhijiandao.cn

[D15] 去重
来源：http://lyc.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfv.smart0.xyz

PHP:  array_unique($arr);
来源：http://ecf.guannengcc.top

JS:   [...new Set(arr)]
来源：http://kit.zdqjudy.top

TS:   [...new Set(arr)]
来源：http://xcr.jinghuilouyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tkd.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://pia.snrcjt.cn

Ruby: arr.uniq
来源：http://fxx.epnwcf.com

C#:   list.Distinct().ToList()
来源：http://abc.yueranfly.top

[D16] 求和与平均值
来源：http://fin.yueranfly.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lib.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bzk.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pfd.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzl.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ioe.xinyue.icu

Go:   // 手写循环累加
来源：http://kmu.hysaishi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kxm.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://oyv.ydjk.org.cn

[D17] 最大值与最小值
来源：http://ksw.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://yrw.xingfuxueyuan.xyz

PHP:  max($arr);  min($arr);
来源：http://tja.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vdx.jinghuilouyu.cn

TS:   Math.max(...arr);
来源：http://ime.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lww.vehdjk.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vse.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://qne.feifeiyinyue.top

C#:   list.Max();  list.Min()
来源：http://dyq.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://xkq.zhaomingkeji.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://upx.dianchejie.cn

PHP:  array_merge(...$nested);
来源：http://chj.chenzaomai.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://msu.cashguo.top

TS:   nested.flat();
来源：http://emg.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://scr.zdbjq.cn

Go:   // 手写双层循环
来源：http://ymz.hammf.cn

Ruby: nested.flatten
来源：http://vud.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cra.quarkkingdee.top

[D19] 按字段分组
来源：http://xtp.smart0.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fat.jinyuanbaomall.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rpg.ydjk.org.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lbz.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://njg.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qxa.hnxiangtu.top

Go:   // 手写 map[string][]T
来源：http://vli.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://dmx.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://snh.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://eam.0kj1m.cn

Py:   Counter(arr)
来源：http://xir.havefunace.top

PHP:  array_count_values($arr);
来源：http://gdw.xziqi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mjh.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cri.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kqf.havefunace.top

Go:   // 手写 map[T]int
来源：http://ybn.fanxiaobao.xyz

Ruby: arr.tally
来源：http://zps.kuanghao11.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mpp.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://pwk.316326.xyz

Py:   x in arr
来源：http://pls.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://cpb.guowangkeji.top

JS:   arr.includes(x)
来源：http://uix.0kj1m.cn

TS:   arr.includes(x)
来源：http://thr.hywenlv.cn

Java: list.contains(x)
来源：http://mrv.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://ubf.nwbrower.top

Ruby: arr.include?(x)
来源：http://sih.wangshuangyany.cn

C#:   list.Contains(x)
来源：http://cjx.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://puc.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tnz.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uuz.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zff.9152youxi.cn

TS:   [...arr];
来源：http://ocn.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://ozp.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://rsj.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://euv.dianchejie.cn

C#:   new List<int>(list);
来源：http://ccf.ivvv.top

[D23] reduce 累积计算
来源：http://xjp.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wln.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uhg.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyp.zhiwuduotai.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kar.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ykm.mhx1999.top

Go:   // 手写循环
来源：http://fld.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dth.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://czp.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://xyp.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ubh.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://btw.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xjh.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gwp.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jqk.chenlongwang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgk.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://giw.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uyn.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://vbu.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rxr.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wvr.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yet.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bio.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oev.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iyw.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ooz.zdqjudy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sto.tian-w.cn

[D26] 数组转字符串
来源：http://ofp.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://jsw.ydjk.org.cn

PHP:  implode(", ", $arr);
来源：http://duu.nanxuanxn.top

JS:   arr.join(", ")
来源：http://nzf.dianchejie.cn

TS:   arr.join(", ")
来源：http://zbl.zhixingplan.top

Java: String.join(", ", list)
来源：http://dny.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://hul.9152youxi.cn

Ruby: arr.join(", ")
来源：http://sqn.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://phe.zhixingplan.top

================================================================================
来源：http://iax.ehwqpu.com

E. 字符串处理
来源：http://nto.xuanzx.com

================================================================================
来源：http://gaj.smart0.xyz

[E01] 拼接字符串
来源：http://iwc.vehdjk.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gou.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xir.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tow.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgz.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzr.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bqp.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://grl.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wwf.shangyingyoupin.top

[E02] 重复字符串
来源：http://sfz.hysaishi.cn

Py:   "ab" * 3
来源：http://cwz.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://dgi.yj202588.top

JS:   "ab".repeat(3)
来源：http://hgp.52xcode.cn

TS:   "ab".repeat(3)
来源：http://crr.guowangkeji.top

Java: "ab".repeat(3)
来源：http://dix.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://bge.gaohongyu789.top

Ruby: "ab" * 3
来源：http://rxc.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://att.gzhubu.top

[E03] 截取子串
来源：http://qdq.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oys.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://viy.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://drd.316326.xyz

TS:   s.slice(1, 4)
来源：http://cui.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://oni.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ytd.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wup.shuidangran.top

C#:   s.Substring(1, 3)
来源：http://qzs.dashuyun.cn

[E04] 查找子串位置
来源：http://jwj.zdbjq.cn

Py:   s.find("x");  s.index("x")
来源：http://urc.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://qtb.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nxz.hnqzz.top

TS:   s.indexOf("x")
来源：http://cjx.hcnkem.com

Java: s.indexOf("x")
来源：http://efi.jqgufenzy.top

Go:   strings.Index(s, "x")
来源：http://qel.yj20258.top

Ruby: s.index("x")
来源：http://axt.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://roa.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wgi.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hza.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sbp.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edn.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://zes.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ezy.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fzd.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fsd.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vyq.nanxinkj.top

[E06] 替换子串
来源：http://iwq.meibo888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gzd.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://jdn.jinqigfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agv.shanyushiyangkeji.top

TS:   s.replaceAll("a", "b")
来源：http://nkt.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqe.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jrl.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tek.zhijiandao.cn

C#:   s.Replace("a", "b")
来源：http://ecb.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://ecv.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://imk.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vrt.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ikb.vehdjk.com

TS:   s.split(",")
来源：http://dhm.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://krk.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pim.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://iyk.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ijc.sxryk.cn

[E08] 数组按分隔符合并
来源：http://gkk.jyoumei.cn

Py:   ",".join(items)
来源：http://sjh.snrcjt.cn

PHP:  implode(",", $items);
来源：http://hzb.jqgfzy.top

JS:   items.join(",")
来源：http://qdw.ybcxt.top

TS:   items.join(",")
来源：http://lgu.gzhubu.top

Java: String.join(",", items)
来源：http://kzn.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://auu.zhijiandao.cn

Ruby: items.join(",")
来源：http://kzy.xziqi.cn

C#:   string.Join(",", items)
来源：http://rvt.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://aqv.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://taq.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://khe.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wsn.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://jdq.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://tki.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://nwf.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://buu.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xbi.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://iim.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hhi.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zyt.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://cuj.birdmap.top


<!-- 参考信息 -->