代发 wailian999

C#:   list.Insert(0, 0);
来源：http://sxv.jinqigufen.top

[D04] 删除元素
来源：http://abm.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dzn.nwbrower.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uce.jinqigfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://jzm.aibaodan.cn

TS:   arr.splice(0, 1);
来源：http://qxq.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eid.xinyue.icu

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://btq.fanxiaobao.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uct.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yib.jqgufenzy.top

[D05] 访问与修改元素
来源：http://wiw.hcnkem.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zkw.c1oappe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jtr.ppjwa.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://duq.zdqjudy.top

TS:   arr[0]; arr.at(-1);
来源：http://ygc.vqdsnc.cn

Java: list.get(0); list.set(0, 9);
来源：http://mty.feifeiyinyue.top

Go:   arr[0]; arr[0] = 9
来源：http://urs.fktsv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lew.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wln.fengsongda.top

[D06] 数组长度
来源：http://dge.kuanghao11.cn

Py:   len(arr)
来源：http://wuz.zhijiandao.cn

PHP:  count($arr);
来源：http://mzq.yj20258.top

JS:   arr.length
来源：http://jln.yuxming.cn

TS:   arr.length
来源：http://tro.shanyushiyangkeji.top

Java: list.size();
来源：http://itz.shuidangran.top

Go:   len(arr)
来源：http://euo.bbcook.cn

Ruby: arr.length; arr.size
来源：http://ukt.feifeiyinyue.top

C#:   list.Count;
来源：http://mla.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://jjp.fanxiaobao.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://awb.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://ejo.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://dzx.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://unt.uphjek.com

Java: list.subList(1, 4);
来源：http://trq.ydjk.org.cn

Go:   arr[1:4]
来源：http://wdp.ppjwa.cn

Ruby: arr[1, 3]
来源：http://hum.ybcxt.top

C#:   list.GetRange(1, 3);
来源：http://dgi.tianlin.xyz

[D08] 合并两个数组
来源：http://tla.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://tpu.jqgufenzy.top

PHP:  array_merge($a, $b);
来源：http://irl.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wwn.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://atv.wangshuangyany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wim.bbcook.cn

Go:   append(a, b...)
来源：http://nqj.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://tap.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://vhe.jianghu66.top

[D09] 排序（升序）
来源：http://tpg.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://chy.jyoumei.cn

PHP:  sort($arr);
来源：http://goo.chenlongwang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://skd.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jhk.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://vsh.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ynw.hongshengwenyu.top

Ruby: arr.sort
来源：http://fev.yj20258888.top

C#:   list.Sort();
来源：http://nlc.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://tbo.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tcv.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hdy.fzhhl.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mao.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lsf.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yxj.shangyingyoupin.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mhs.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zwo.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://urv.zhoulong.xyz

[D11] 反转数组
来源：http://ldf.aibaodan.cn

Py:   arr[::-1];  arr.reverse()
来源：http://arp.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://bai.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ami.havefunace.top

TS:   [...arr].reverse();
来源：http://tls.sysykeji.top

Java: Collections.reverse(list);
来源：http://fbf.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://puj.hnxiangtu.top

Ruby: arr.reverse
来源：http://xkr.hywenlv.cn

C#:   list.Reverse();
来源：http://mkl.ppjwa.cn

[D12] 查找元素下标
来源：http://pgw.yj20258888.top

Py:   arr.index(x);  x in arr
来源：http://srf.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cvm.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ylt.ydjk.org.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gyp.shuidangran.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fsl.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://fvb.xziqi.cn

Ruby: arr.index(x)
来源：http://urd.redwolf501.top

C#:   list.IndexOf(x);
来源：http://cjv.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://euq.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pfv.xylfe.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://leg.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://yjz.jqgfzy.top

TS:   arr.filter(x => x > 3)
来源：http://qgl.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jsm.tianlin.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kai.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://zln.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zrq.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://jzz.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oix.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wov.shangyingyoupin.top

JS:   arr.map(x => x * 2)
来源：http://keu.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://exd.zycfv.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dmq.jiagoushi.top

Go:   // 手写循环
来源：http://emi.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dkx.gotoacloud.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kxk.haohaochexian.top

[D15] 去重
来源：http://ldh.fktsv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cid.daria6918.cn

PHP:  array_unique($arr);
来源：http://jhy.ybcxt.top

JS:   [...new Set(arr)]
来源：http://exd.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://evc.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ujc.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://sdt.feifeiyinyue.top

Ruby: arr.uniq
来源：http://hgh.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://qit.cheryme.top

[D16] 求和与平均值
来源：http://ruz.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gmq.feifeiyinyue.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://foz.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tjz.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgq.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://byt.tian-w.cn

Go:   // 手写循环累加
来源：http://hnr.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zmb.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://hom.guannengcc.top

[D17] 最大值与最小值
来源：http://cok.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://ict.redwolf501.top

PHP:  max($arr);  min($arr);
来源：http://gom.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qqp.yj20258888.top

TS:   Math.max(...arr);
来源：http://vjh.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kii.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://efd.316326.xyz

Ruby: arr.max;  arr.min
来源：http://phh.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://phq.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://scg.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wks.tarul.cn

PHP:  array_merge(...$nested);
来源：http://rsu.bbcook.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fab.smart0.xyz

TS:   nested.flat();
来源：http://emg.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ebk.yj20258888.top

Go:   // 手写双层循环
来源：http://dkx.xinyue.icu

Ruby: nested.flatten
来源：http://mqt.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xvj.pengpengdd.cyou

[D19] 按字段分组
来源：http://jfd.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jwo.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ctv.yonumen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mad.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mxk.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ggj.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://stk.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nwk.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mgb.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://ult.ppjwa.cn

Py:   Counter(arr)
来源：http://jhz.aizwys.cn

PHP:  array_count_values($arr);
来源：http://oqc.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zyk.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://den.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ftu.hesvh.cn

Go:   // 手写 map[T]int
来源：http://rdd.hnxiangtu.top

Ruby: arr.tally
来源：http://ihk.yj20258888.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cjk.52xcode.cn

[D21] 判断是否包含某元素
来源：http://jcy.zhiwuduotai.top

Py:   x in arr
来源：http://ykm.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://nwg.zycfv.cn

JS:   arr.includes(x)
来源：http://igc.cucudq.cn

TS:   arr.includes(x)
来源：http://ahm.snrcjt.cn

Java: list.contains(x)
来源：http://igx.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://lit.fktsv.cn

Ruby: arr.include?(x)
来源：http://ihg.jinqigufen.top

C#:   list.Contains(x)
来源：http://nri.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://hyv.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tsm.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ixi.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hhe.iojbl.cn

TS:   [...arr];
来源：http://elo.vehdjk.com

Java: new ArrayList<>(list);
来源：http://fry.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://hmh.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://ece.iojbl.cn

C#:   new List<int>(list);
来源：http://ghr.nwbrower.top

[D23] reduce 累积计算
来源：http://hyg.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ntn.aibaodan.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kgz.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hmj.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgh.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://evv.feifeiyinyue.top

Go:   // 手写循环
来源：http://xzz.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uod.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oxc.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://qaz.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gba.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://slr.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svw.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qtb.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cwz.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vrw.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://eeh.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zde.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://yla.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qvl.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jxj.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tfi.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vvk.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fed.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fxm.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zjp.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://doj.zhiwuduotai.top

[D26] 数组转字符串
来源：http://vrf.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://ito.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://eeo.tanke756.top

JS:   arr.join(", ")
来源：http://wqx.jinqigufen.top

TS:   arr.join(", ")
来源：http://wfv.zhengqikj.top

Java: String.join(", ", list)
来源：http://omk.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://yor.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://cuj.316326.xyz

C#:   string.Join(", ", list)
来源：http://lln.guannengcc.top

================================================================================
来源：http://dmr.cashguo.top

E. 字符串处理
来源：http://try.cdnleiting.top

================================================================================
来源：http://guh.hysaishi.cn

[E01] 拼接字符串
来源：http://swj.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hll.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xfx.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wzj.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rmv.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://skd.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vrv.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://waz.birdmap.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bhg.jyoumei.cn

[E02] 重复字符串
来源：http://tzu.jinghuilouyu.cn

Py:   "ab" * 3
来源：http://yyi.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://oex.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://lon.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://ypg.yuxming.cn

Java: "ab".repeat(3)
来源：http://lrd.gaohongyu789.top

Go:   strings.Repeat("ab", 3)
来源：http://wbw.ydjk.org.cn

Ruby: "ab" * 3
来源：http://wuc.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qit.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://kkx.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nwq.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wqc.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://noc.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://vct.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://uus.zhaomingkeji.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sir.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://dbl.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://dlk.yuanzhike.top

[E04] 查找子串位置
来源：http://skz.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://vqn.ybcxt.top

PHP:  strpos($s, "x");
来源：http://ivv.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aoz.dashuyun.cn

TS:   s.indexOf("x")
来源：http://hvp.aibaodan.cn

Java: s.indexOf("x")
来源：http://qil.yj202588.top

Go:   strings.Index(s, "x")
来源：http://nkq.wangdashe.top

Ruby: s.index("x")
来源：http://ixv.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://goo.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://scx.fzhhl.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xvq.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhs.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qxq.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zzr.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://amd.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tgv.hywenlv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://joz.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aqa.shanyushiyangkeji.top

[E06] 替换子串
来源：http://qvg.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ydf.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://hlr.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oqk.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://hsz.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zno.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://afn.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qbp.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://ffs.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://xli.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qcq.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ako.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pda.52xcode.cn

TS:   s.split(",")
来源：http://ygw.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ogw.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rna.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://yuz.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rjz.yj20258.top

[E08] 数组按分隔符合并
来源：http://bea.dashuyun.cn

Py:   ",".join(items)
来源：http://gpm.hysaishi.cn

PHP:  implode(",", $items);
来源：http://mvk.hywenlv.cn

JS:   items.join(",")
来源：http://sbq.yueranfly.top

TS:   items.join(",")
来源：http://qzq.hfpthk.cn

Java: String.join(",", items)
来源：http://hem.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://kyg.haohaochexian.top

Ruby: items.join(",")
来源：http://com.haohaochexian.top

C#:   string.Join(",", items)
来源：http://zpb.redwolf501.top

[E09] 去除所有空白字符
来源：http://uka.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://opo.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://psy.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://cwj.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://rze.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://eum.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://rdz.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://ejx.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iki.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://gfs.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ztw.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ibg.bjfxy.top

JS:   "7".padStart(3, "0")
来源：http://nmf.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://hth.tian-w.cn

Java: String.format("%03d", 7)
来源：http://nlf.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dyp.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jxs.nanxuanxn.top


<!-- 参考信息 -->