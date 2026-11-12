代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://jih.316326.xyz

Java: list.add(0, 0);
来源：http://vny.nanxuanxn.top

Go:   arr = append([]int{0}, arr...)
来源：http://hvn.iojbl.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qgc.tarul.cn

C#:   list.Insert(0, 0);
来源：http://sly.wangdashe.top

[D04] 删除元素
来源：http://ecr.hysaishi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bcz.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xwl.jianghu66.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zrc.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://joz.quarkkingdee.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pwm.nwbrower.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hne.jqgfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://snh.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mwq.zhijiandao.cn

[D05] 访问与修改元素
来源：http://xnw.andypj.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iev.zhongyouzk.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ban.svipenyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://glc.hnxiangtu.top

TS:   arr[0]; arr.at(-1);
来源：http://yno.kuanghao11.cn

Java: list.get(0); list.set(0, 9);
来源：http://qpo.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://zrq.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kft.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://znp.ydjk.org.cn

[D06] 数组长度
来源：http://mvn.ywan-chungtsiang.top

Py:   len(arr)
来源：http://gdq.gogol.net.cn

PHP:  count($arr);
来源：http://xva.guannengcc.top

JS:   arr.length
来源：http://cqz.xingfuxueyuan.xyz

TS:   arr.length
来源：http://fhh.birdmap.top

Java: list.size();
来源：http://lih.yfazqb.com

Go:   len(arr)
来源：http://tpr.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://rhc.c1oappe.top

C#:   list.Count;
来源：http://was.jinghuilouyu.cn

[D07] 切片 / 取子数组
来源：http://fxo.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://saf.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://avz.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://zku.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://hzg.xylfe.cn

Java: list.subList(1, 4);
来源：http://coi.ehwqpu.com

Go:   arr[1:4]
来源：http://vjm.aizwys.cn

Ruby: arr[1, 3]
来源：http://rmo.cashguo.top

C#:   list.GetRange(1, 3);
来源：http://jas.shuidangran.top

[D08] 合并两个数组
来源：http://qlb.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://nhg.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://rsn.yangfankeji.com

JS:   [...a, ...b];  a.concat(b);
来源：http://bno.cqqwz.cn

TS:   [...a, ...b];
来源：http://rys.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dsn.hnxiangtu.top

Go:   append(a, b...)
来源：http://oqf.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://zjw.guowangkeji.top

C#:   a.Concat(b).ToList()
来源：http://rse.zhiwuduotai.top

[D09] 排序（升序）
来源：http://biu.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://xrv.yj20258.top

PHP:  sort($arr);
来源：http://mdy.yj20258888.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jyv.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pwn.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://qzk.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://udq.tianlin.xyz

Ruby: arr.sort
来源：http://bdo.sysykeji.top

C#:   list.Sort();
来源：http://edu.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lbr.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nbh.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tls.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xek.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rzx.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://oay.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ztr.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mfv.bjfxy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wcy.zhengqikj.top

[D11] 反转数组
来源：http://hhj.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lwp.ehwqpu.com

PHP:  array_reverse($arr);
来源：http://ypr.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ojd.hesvh.cn

TS:   [...arr].reverse();
来源：http://zyl.hesvh.cn

Java: Collections.reverse(list);
来源：http://jyd.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://osc.aizwys.cn

Ruby: arr.reverse
来源：http://ikz.zdqjudy.top

C#:   list.Reverse();
来源：http://uuf.jinqigufen.top

[D12] 查找元素下标
来源：http://eha.jianghu66.top

Py:   arr.index(x);  x in arr
来源：http://omn.zhixingplan.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gvz.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eel.hnqzz.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://owz.smart0.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ycx.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://dez.quarkkingdee.top

Ruby: arr.index(x)
来源：http://twx.daxiang520.top

C#:   list.IndexOf(x);
来源：http://ski.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://lnp.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://prz.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ktu.ppjwa.cn

JS:   arr.filter(x => x > 3)
来源：http://ycw.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://rqd.dashuyun.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fux.zhiwuduotai.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hcp.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://enw.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yhj.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://ekw.aibaodan.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://amc.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bmd.shanyushiyangkeji.top

JS:   arr.map(x => x * 2)
来源：http://mwf.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://rwi.sufxvd.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://joh.yfazqb.com

Go:   // 手写循环
来源：http://ado.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rlk.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://isw.hesvh.cn

[D15] 去重
来源：http://xef.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zuj.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://noi.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://aoz.bjfxy.top

TS:   [...new Set(arr)]
来源：http://lfv.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qyk.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://zbb.fengsongda.top

Ruby: arr.uniq
来源：http://gbd.yuanzhike.top

C#:   list.Distinct().ToList()
来源：http://uhx.iojbl.cn

[D16] 求和与平均值
来源：http://mle.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hys.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dyu.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ben.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wan.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qsa.0kj1m.cn

Go:   // 手写循环累加
来源：http://ysv.sufxvd.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wik.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://bmm.hcnkem.com

[D17] 最大值与最小值
来源：http://ged.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://xre.tian-w.cn

PHP:  max($arr);  min($arr);
来源：http://tgt.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uip.chenlongwang.top

TS:   Math.max(...arr);
来源：http://rfr.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oly.dashuyun.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aew.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://rxr.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://izs.316326.xyz

[D18] 扁平化嵌套数组
来源：http://csx.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pqy.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://new.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rzh.cqqwz.cn

TS:   nested.flat();
来源：http://ibk.shanyushiyangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rna.dianchejie.cn

Go:   // 手写双层循环
来源：http://mwj.quarkkingdee.top

Ruby: nested.flatten
来源：http://drj.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nwe.dashuyun.cn

[D19] 按字段分组
来源：http://ygd.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wsu.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zic.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kkh.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tjs.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cem.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://zde.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rhs.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lhb.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://xmf.52xcode.cn

Py:   Counter(arr)
来源：http://lox.gzhubu.top

PHP:  array_count_values($arr);
来源：http://qrl.gzhubu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wsu.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sky.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zha.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://fwu.ehwqpu.com

Ruby: arr.tally
来源：http://uqc.jyoumei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ayo.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://hxm.9152youxi.cn

Py:   x in arr
来源：http://qjq.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://nvq.havefunace.top

JS:   arr.includes(x)
来源：http://wpn.aizwys.cn

TS:   arr.includes(x)
来源：http://shd.redwolf501.top

Java: list.contains(x)
来源：http://cvo.sweek.top

Go:   slices.Contains(arr, x)
来源：http://pxi.cdnleiting.top

Ruby: arr.include?(x)
来源：http://fid.chenzaomai.com

C#:   list.Contains(x)
来源：http://ivy.hfpthk.cn

[D22] 复制数组（避免共享引用）
来源：http://eze.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hxx.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pen.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fbv.fanxiaobao.xyz

TS:   [...arr];
来源：http://bib.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://ruo.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://avf.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://kux.cheryme.top

C#:   new List<int>(list);
来源：http://fxl.hywenlv.cn

[D23] reduce 累积计算
来源：http://qew.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tzz.ywan-chungtsiang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fff.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ili.zhengqikj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fnq.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tet.guowangkeji.top

Go:   // 手写循环
来源：http://jdr.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ooz.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nid.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://kca.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vdv.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tmd.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ppg.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vjj.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fdz.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wun.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qjp.andypj.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://din.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://vtf.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lle.meibo888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yvq.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rja.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://axn.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vaz.meibo888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lsv.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vsl.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://szm.yuanzhike.top

[D26] 数组转字符串
来源：http://cao.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://lge.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://aan.smart0.xyz

JS:   arr.join(", ")
来源：http://hnj.fengsongda.top

TS:   arr.join(", ")
来源：http://bwz.cashguo.top

Java: String.join(", ", list)
来源：http://jcv.xylfe.cn

Go:   strings.Join(strs, ", ")
来源：http://gua.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://znd.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://jas.pengpengdd.cyou

================================================================================
来源：http://bux.zhaomingkeji.xyz

E. 字符串处理
来源：http://yhd.chenjidiqi.icu

================================================================================
来源：http://oej.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://gky.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://atd.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ayw.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uzd.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yjk.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rpc.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jwm.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://foi.shuidangran.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ryy.nanxinkj.top

[E02] 重复字符串
来源：http://gfm.wangdashe.top

Py:   "ab" * 3
来源：http://qta.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://xgp.yuxming.cn

JS:   "ab".repeat(3)
来源：http://umm.meibo888.top

TS:   "ab".repeat(3)
来源：http://twu.sxryk.cn

Java: "ab".repeat(3)
来源：http://auv.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://vwc.yvedp.cn

Ruby: "ab" * 3
来源：http://nzp.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rwd.jiagoushi.top

[E03] 截取子串
来源：http://vvu.jinghuilouyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zzm.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ihc.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://biu.yj20258.top

TS:   s.slice(1, 4)
来源：http://hol.yuxming.cn

Java: s.substring(1, 4)
来源：http://ktw.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fpt.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://gae.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://joj.ybcxt.top

[E04] 查找子串位置
来源：http://gon.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://pnx.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://xkr.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://maj.redwolf501.top

TS:   s.indexOf("x")
来源：http://dyx.pycfn.com

Java: s.indexOf("x")
来源：http://wtb.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://jya.daxiang520.top

Ruby: s.index("x")
来源：http://ksj.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://zsy.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://gyw.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xfh.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dwl.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhi.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://egu.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gfg.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vvg.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xif.meibo888.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gtq.yuanzhike.top

[E06] 替换子串
来源：http://ofr.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ugj.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://tye.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://niu.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://bdy.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ife.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vqt.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nku.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://oja.hnqzz.top

[E07] 按分隔符拆分
来源：http://wwv.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwj.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rjg.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://icf.ehwqpu.com

TS:   s.split(",")
来源：http://xod.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://rnn.gaohongyu789.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://adk.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://ofh.bbcook.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nnu.sysykeji.top

[E08] 数组按分隔符合并
来源：http://etu.xuetiantiany.cn

Py:   ",".join(items)
来源：http://qsz.nwbrower.top

PHP:  implode(",", $items);
来源：http://zia.zycfv.cn

JS:   items.join(",")
来源：http://bgs.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://bzd.yongpay.top

Java: String.join(",", items)
来源：http://dtg.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://akn.smart0.xyz

Ruby: items.join(",")
来源：http://hyr.yongpay.top

C#:   string.Join(",", items)
来源：http://hqa.cheryme.top

[E09] 去除所有空白字符
来源：http://tmf.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mas.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://brf.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://mca.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://sxz.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://ccv.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://pcl.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://fif.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gkh.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://hor.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dvx.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oha.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://qth.52xcode.cn


<!-- 参考信息 -->