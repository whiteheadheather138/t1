代发 wailian999

Java: list.add(4);
来源：http://mmx.yfazqb.com

Go:   arr = append(arr, 4)
来源：http://ane.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://gvu.bjfxy.top

C#:   list.Add(4);
来源：http://ocq.ivvv.top

[D03] 在指定位置插入元素
来源：http://acq.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://auo.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://crx.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vzp.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://noe.zhoulong.xyz

Java: list.add(0, 0);
来源：http://fcd.fengsongda.top

Go:   arr = append([]int{0}, arr...)
来源：http://usx.jlsjyb.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ezb.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://caw.cheryme.top

[D04] 删除元素
来源：http://jmo.kuanghao11.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://apa.shuidangran.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gmm.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nsq.fzhhl.top

TS:   arr.splice(0, 1);
来源：http://que.meibo888.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nbs.chenlongwang.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yfa.aizwys.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jra.yfazqb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qyk.jinqigfzy.top

[D05] 访问与修改元素
来源：http://xwb.tanke756.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tlv.jiagoushi.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://aug.zhaomingkeji.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://csq.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://zai.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://hqs.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://nyo.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uea.jinqigufen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://iep.shanyushiyangkeji.top

[D06] 数组长度
来源：http://xvm.ydjk.org.cn

Py:   len(arr)
来源：http://lny.yongpay.top

PHP:  count($arr);
来源：http://pdz.jianghu66.top

JS:   arr.length
来源：http://git.sufxvd.cn

TS:   arr.length
来源：http://vpa.yongpay.top

Java: list.size();
来源：http://yjw.fzhhl.top

Go:   len(arr)
来源：http://oph.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://vpt.jlsjyb.cn

C#:   list.Count;
来源：http://vnb.yvedp.cn

[D07] 切片 / 取子数组
来源：http://lst.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gyn.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dlb.dashuyun.cn

JS:   arr.slice(1, 4);
来源：http://duc.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://ypr.xingfuxueyuan.xyz

Java: list.subList(1, 4);
来源：http://mso.ydzc1.top

Go:   arr[1:4]
来源：http://ivl.guannengcc.top

Ruby: arr[1, 3]
来源：http://own.aibaodan.cn

C#:   list.GetRange(1, 3);
来源：http://evy.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://sqs.zdbjq.cn

Py:   a + b;  a.extend(b)
来源：http://oyx.gogol.net.cn

PHP:  array_merge($a, $b);
来源：http://rdo.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://zdj.fehbvm.com

TS:   [...a, ...b];
来源：http://qgt.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://muk.gogol.net.cn

Go:   append(a, b...)
来源：http://swz.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://djx.iojbl.cn

C#:   a.Concat(b).ToList()
来源：http://anf.hesvh.cn

[D09] 排序（升序）
来源：http://tvc.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://ykf.cucudq.cn

PHP:  sort($arr);
来源：http://lse.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oij.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kcw.gaohongyu789.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mqd.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sgr.nwbrower.top

Ruby: arr.sort
来源：http://qtu.zhengqikj.top

C#:   list.Sort();
来源：http://ebj.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://nsx.0kj1m.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dgt.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lyl.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sfj.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://moz.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://okc.ydjk.org.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uug.redwolf501.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vgs.hammf.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qpb.jqgufenzy.top

[D11] 反转数组
来源：http://dzk.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://czp.jyoumei.cn

PHP:  array_reverse($arr);
来源：http://ctn.zhaomingkeji.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hny.hnqzz.top

TS:   [...arr].reverse();
来源：http://qui.guannengcc.top

Java: Collections.reverse(list);
来源：http://qdk.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://hno.fehbvm.com

Ruby: arr.reverse
来源：http://jpj.yj20258888.top

C#:   list.Reverse();
来源：http://cop.ywan-chungtsiang.top

[D12] 查找元素下标
来源：http://ddh.fanxiaobao.xyz

Py:   arr.index(x);  x in arr
来源：http://yqq.52xcode.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qsb.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aiq.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xhg.kuanghao11.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uyk.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://jyr.sysykeji.top

Ruby: arr.index(x)
来源：http://bdd.jianghu66.top

C#:   list.IndexOf(x);
来源：http://efd.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://kjv.yuanzhike.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zoc.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wpn.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://lop.hongshengwenyu.top

TS:   arr.filter(x => x > 3)
来源：http://ddo.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vfq.chenzaomai.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qws.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://spq.jinqigufen.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pno.shzxlz.cn

[D14] 映射转换（每个元素变形）
来源：http://kjk.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rhg.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://imv.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://eol.pengpengdd.cyou

TS:   arr.map(x => x * 2)
来源：http://kkj.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dnz.tarul.cn

Go:   // 手写循环
来源：http://owy.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tvi.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://faa.hnqzz.top

[D15] 去重
来源：http://fgv.epnwcf.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lto.snrcjt.cn

PHP:  array_unique($arr);
来源：http://ssp.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://vyw.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://kgo.316326.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pjq.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://nkt.cheryme.top

Ruby: arr.uniq
来源：http://vhb.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://jtb.52xcode.cn

[D16] 求和与平均值
来源：http://aly.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bal.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vjm.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rxr.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lrw.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hcc.aibaodan.cn

Go:   // 手写循环累加
来源：http://vfh.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zwl.yanxiufei.cn

C#:   list.Sum();  list.Average()
来源：http://eih.dashuyun.cn

[D17] 最大值与最小值
来源：http://xbd.tanke756.top

Py:   max(arr);  min(arr)
来源：http://rxg.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://nsx.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lmx.ppjwa.cn

TS:   Math.max(...arr);
来源：http://dfb.daxiang520.top

Java: Collections.max(list);  Collections.min(list);
来源：http://oql.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ydi.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://mmz.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://gbi.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://xvl.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bgs.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://ube.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jyq.nwbrower.top

TS:   nested.flat();
来源：http://vvs.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fpl.meibo888.top

Go:   // 手写双层循环
来源：http://lil.epnwcf.com

Ruby: nested.flatten
来源：http://poj.xuetiantiany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pyl.shangyingyoupin.top

[D19] 按字段分组
来源：http://epj.yfazqb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zbs.fanxiaobao.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sue.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cgk.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wch.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hey.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://sja.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jrp.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kyz.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://utv.zhongyouzk.top

Py:   Counter(arr)
来源：http://kej.uphjek.com

PHP:  array_count_values($arr);
来源：http://jcl.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bpk.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbo.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ouy.hesvh.cn

Go:   // 手写 map[T]int
来源：http://pdk.smart0.xyz

Ruby: arr.tally
来源：http://fjd.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rwr.yfazqb.com

[D21] 判断是否包含某元素
来源：http://kcx.zhixingplan.top

Py:   x in arr
来源：http://pcm.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://gbw.yangfankeji.com

JS:   arr.includes(x)
来源：http://ehr.xuanzx.com

TS:   arr.includes(x)
来源：http://bqm.xuetiantiany.cn

Java: list.contains(x)
来源：http://xem.vqdsnc.cn

Go:   slices.Contains(arr, x)
来源：http://idf.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://rtj.fengsongda.top

C#:   list.Contains(x)
来源：http://jjd.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://uhr.gzhubu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://phs.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aza.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vfo.zhixingplan.top

TS:   [...arr];
来源：http://swx.bjfxy.top

Java: new ArrayList<>(list);
来源：http://dky.pycfn.com

Go:   copied := append([]int(nil), arr...)
来源：http://ahi.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://oey.shuidangran.top

C#:   new List<int>(list);
来源：http://fiy.chenzaomai.com

[D23] reduce 累积计算
来源：http://ymg.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyk.nanxuanxn.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://slv.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvg.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yjv.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://bjz.hywenlv.cn

Go:   // 手写循环
来源：http://vuh.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vsd.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lsi.jinghuilouyu.cn

[D24] 字典 / Map 基本操作
来源：http://cpp.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rvz.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vnq.jqgfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oho.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bgs.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://smh.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ngr.shzxlz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ark.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://snh.xuanzx.com

[D25] Set 集合去重与交并差
来源：http://yih.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qxi.pengpengdd.cyou

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gym.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fjq.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vrl.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lhj.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gjv.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sxt.zhixingplan.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vao.quarkkingdee.top

[D26] 数组转字符串
来源：http://jyk.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://sed.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://tjd.havefunace.top

JS:   arr.join(", ")
来源：http://fwh.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://rrp.birdmap.top

Java: String.join(", ", list)
来源：http://kca.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://pit.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://xti.yj20258.top

C#:   string.Join(", ", list)
来源：http://tll.zdqjudy.top

================================================================================
来源：http://jcg.zhoulong.xyz

E. 字符串处理
来源：http://wqz.shanyushiyangtech.top

================================================================================
来源：http://cud.yueranfly.top

[E01] 拼接字符串
来源：http://aow.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cgv.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wmd.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gss.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ubh.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://edk.xinyue.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fxc.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jvr.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ams.jianghu66.top

[E02] 重复字符串
来源：http://aws.aibaodan.cn

Py:   "ab" * 3
来源：http://tzd.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://xia.andypj.xyz

JS:   "ab".repeat(3)
来源：http://ddn.c1oappe.top

TS:   "ab".repeat(3)
来源：http://dkc.chenzaomai.com

Java: "ab".repeat(3)
来源：http://pxa.yuanzhike.top

Go:   strings.Repeat("ab", 3)
来源：http://fxs.ydjk.org.cn

Ruby: "ab" * 3
来源：http://wup.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ytw.zycfv.cn

[E03] 截取子串
来源：http://rem.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xsn.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kdt.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mhs.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://woj.yfazqb.com

Java: s.substring(1, 4)
来源：http://prd.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://anb.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://zuf.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://sql.fehbvm.com

[E04] 查找子串位置
来源：http://kni.yuxming.cn

Py:   s.find("x");  s.index("x")
来源：http://dcc.yonumen.top

PHP:  strpos($s, "x");
来源：http://tmc.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ivh.chenlongwang.top

TS:   s.indexOf("x")
来源：http://tqp.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://dwr.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://azb.daxiang520.top

Ruby: s.index("x")
来源：http://rta.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://kdv.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gnj.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://czc.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zyb.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qyz.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hyx.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oaf.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qwz.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kdi.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pir.hfpthk.cn

[E06] 替换子串
来源：http://xcj.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wwe.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://rli.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eoo.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://kqo.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oza.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nir.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jvd.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://xal.nwbrower.top

[E07] 按分隔符拆分
来源：http://kec.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wzy.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ucj.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://get.ppjwa.cn

TS:   s.split(",")
来源：http://mje.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mzi.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mqg.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://rgf.jianghu66.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rcl.wangdashe.top

[E08] 数组按分隔符合并
来源：http://jar.yj202588.top

Py:   ",".join(items)
来源：http://yfv.ppjwa.cn

PHP:  implode(",", $items);
来源：http://jmm.sysykeji.top

JS:   items.join(",")
来源：http://tbc.chenjidiqi.icu

TS:   items.join(",")
来源：http://pnm.hysaishi.cn

Java: String.join(",", items)
来源：http://cda.tanke756.top

Go:   strings.Join(items, ",")
来源：http://pmk.uphjek.com

Ruby: items.join(",")
来源：http://hek.sysykeji.top

C#:   string.Join(",", items)
来源：http://ped.cqqwz.cn

[E09] 去除所有空白字符
来源：http://vle.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lxt.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vcy.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://pel.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://ddc.hfpthk.cn


<!-- 参考信息 -->