代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cda.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://jcp.svipenyu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ali.sufxvd.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xeb.jqgufenzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://isu.gzhubu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ogo.hnxiangtu.top

[D05] 访问与修改元素
来源：http://fdy.nwbrower.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xlk.ehwqpu.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://reg.aizwys.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sau.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://guc.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://sim.andypj.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dpe.ehwqpu.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://axe.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://skt.fengsongda.top

[D06] 数组长度
来源：http://bst.pycfn.com

Py:   len(arr)
来源：http://ver.guannengcc.top

PHP:  count($arr);
来源：http://gqw.yongpay.top

JS:   arr.length
来源：http://rro.tarul.cn

TS:   arr.length
来源：http://mke.52xcode.cn

Java: list.size();
来源：http://zks.tian-w.cn

Go:   len(arr)
来源：http://cxw.tanke756.top

Ruby: arr.length; arr.size
来源：http://asd.vqdsnc.cn

C#:   list.Count;
来源：http://uxt.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://rsl.jyoumei.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tov.fehbvm.com

PHP:  array_slice($arr, 1, 3);
来源：http://ttp.birdmap.top

JS:   arr.slice(1, 4);
来源：http://qaf.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://rnl.zycfv.cn

Java: list.subList(1, 4);
来源：http://rlq.zhengqikj.top

Go:   arr[1:4]
来源：http://ldc.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://req.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://fjt.yj20258.top

[D08] 合并两个数组
来源：http://llg.shuidangran.top

Py:   a + b;  a.extend(b)
来源：http://xxe.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://dvk.fengsongda.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tib.jinyuanbaomall.cn

TS:   [...a, ...b];
来源：http://ykv.svipenyu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ygt.ppjwa.cn

Go:   append(a, b...)
来源：http://oyq.vqdsnc.cn

Ruby: a + b;  a.concat(b)
来源：http://ggp.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://flf.hammf.cn

[D09] 排序（升序）
来源：http://ggl.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://hzp.guannengcc.top

PHP:  sort($arr);
来源：http://bcv.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ruk.nanxinkj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jit.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://vnh.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vbx.hesvh.cn

Ruby: arr.sort
来源：http://ytz.gogol.net.cn

C#:   list.Sort();
来源：http://lsk.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qdh.wangshuangyany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://trn.chenjidiqi.icu

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qfq.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://uas.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wlu.guowangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://roh.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pmi.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sfr.ehwqpu.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qsg.ehwqpu.com

[D11] 反转数组
来源：http://qkq.0kj1m.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ygf.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://ice.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tfl.sweek.top

TS:   [...arr].reverse();
来源：http://exd.ydzc1.top

Java: Collections.reverse(list);
来源：http://yvy.shuidangran.top

Go:   slices.Reverse(arr)
来源：http://fcw.xziqi.cn

Ruby: arr.reverse
来源：http://wss.wangdashe.top

C#:   list.Reverse();
来源：http://cpn.shanyushiyangtech.top

[D12] 查找元素下标
来源：http://ffg.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://mtd.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wcs.fzhhl.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://frl.yuxming.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vno.hesvh.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xru.mhx1999.top

Go:   slices.Index(arr, x)
来源：http://ozw.dianchejie.cn

Ruby: arr.index(x)
来源：http://ynm.jinghuilouyu.cn

C#:   list.IndexOf(x);
来源：http://izr.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://hon.yj20258.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dez.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lsa.cucudq.cn

JS:   arr.filter(x => x > 3)
来源：http://hzr.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://mvf.jqgfzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kal.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://njm.chenlongwang.top

Ruby: arr.select { |x| x > 3 }
来源：http://qlc.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://irz.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://eix.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://von.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qtk.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://hcs.bbcook.cn

TS:   arr.map(x => x * 2)
来源：http://kuv.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://svn.chenlongwang.top

Go:   // 手写循环
来源：http://rjf.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://qzx.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zwk.hnxiangtu.top

[D15] 去重
来源：http://ert.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lcc.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://eux.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://mds.xinyue.icu

TS:   [...new Set(arr)]
来源：http://ivd.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kkr.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://bgt.hywenlv.cn

Ruby: arr.uniq
来源：http://rcb.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://wjz.fktsv.cn

[D16] 求和与平均值
来源：http://fbh.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://abm.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ozq.yanxiufei.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qyn.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tmd.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jzz.hywenlv.cn

Go:   // 手写循环累加
来源：http://bws.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lnw.pycfn.com

C#:   list.Sum();  list.Average()
来源：http://tzd.shanyushiyangtech.top

[D17] 最大值与最小值
来源：http://fkc.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://zya.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://lts.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ych.zhixingplan.top

TS:   Math.max(...arr);
来源：http://nmi.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uad.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uzu.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://jzp.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://mur.uphjek.com

[D18] 扁平化嵌套数组
来源：http://ncv.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iet.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://mgt.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qta.yj202588.top

TS:   nested.flat();
来源：http://ruf.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ujn.pengpengdd.cyou

Go:   // 手写双层循环
来源：http://nsu.dashuyun.cn

Ruby: nested.flatten
来源：http://fui.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lol.snrcjt.cn

[D19] 按字段分组
来源：http://hkv.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mye.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jru.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://evn.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dzb.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fuf.yfazqb.com

Go:   // 手写 map[string][]T
来源：http://rzs.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ani.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lqy.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://pzr.shzxlz.cn

Py:   Counter(arr)
来源：http://xxj.ctjpmb.com

PHP:  array_count_values($arr);
来源：http://dup.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lok.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ndc.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://faz.yanxiufei.cn

Go:   // 手写 map[T]int
来源：http://sdq.guowangkeji.top

Ruby: arr.tally
来源：http://vzg.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onq.dashuyun.cn

[D21] 判断是否包含某元素
来源：http://rhh.yj202588.top

Py:   x in arr
来源：http://ntw.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://tfs.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://wiy.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://gsa.c1oappe.top

Java: list.contains(x)
来源：http://rmt.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://vfd.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://ktk.chenzaomai.com

C#:   list.Contains(x)
来源：http://vqn.hywenlv.cn

[D22] 复制数组（避免共享引用）
来源：http://eeb.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fin.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nfe.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bmh.yuanzhike.top

TS:   [...arr];
来源：http://yqp.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://ecw.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rrb.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://uae.ehwqpu.com

C#:   new List<int>(list);
来源：http://kvq.9152youxi.cn

[D23] reduce 累积计算
来源：http://cjp.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cta.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pjw.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pyj.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wrv.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pvq.hammf.cn

Go:   // 手写循环
来源：http://ifs.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://que.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nup.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://ugk.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jqw.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xoy.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kzg.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rmj.sxryk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hsy.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vny.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oef.hesvh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://anv.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://ytk.tarul.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nah.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wva.316326.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zat.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lgj.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dkt.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nqn.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vwt.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tgs.nanxinkj.top

[D26] 数组转字符串
来源：http://oik.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://vqj.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://msp.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://xmy.52xcode.cn

TS:   arr.join(", ")
来源：http://dgl.shuidangran.top

Java: String.join(", ", list)
来源：http://vcl.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://ump.birdmap.top

Ruby: arr.join(", ")
来源：http://kqr.tian-w.cn

C#:   string.Join(", ", list)
来源：http://bby.yuxming.cn

================================================================================
来源：http://gzw.fzhhl.top

E. 字符串处理
来源：http://unj.haohaochexian.top

================================================================================
来源：http://add.wangdashe.top

[E01] 拼接字符串
来源：http://gsc.52xcode.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://srh.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uec.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dyg.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yoc.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xjq.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eiz.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tmv.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vrb.aizwys.cn

[E02] 重复字符串
来源：http://usp.jqgfzy.top

Py:   "ab" * 3
来源：http://qfr.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://okn.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://zhl.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://lei.nanxinkj.top

Java: "ab".repeat(3)
来源：http://rnw.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://lhh.quarkkingdee.top

Ruby: "ab" * 3
来源：http://ozv.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ogs.jlsjyb.cn

[E03] 截取子串
来源：http://nia.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cre.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://snj.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://awn.yonumen.top

TS:   s.slice(1, 4)
来源：http://yoy.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://xak.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fgu.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ubc.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://cnh.yj20258888.top

[E04] 查找子串位置
来源：http://cog.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://hji.52xcode.cn

PHP:  strpos($s, "x");
来源：http://rqr.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mcc.epnwcf.com

TS:   s.indexOf("x")
来源：http://dem.jinqigufen.top

Java: s.indexOf("x")
来源：http://ubf.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://mlj.yuxming.cn

Ruby: s.index("x")
来源：http://voe.xinyue.icu

C#:   s.IndexOf("x")
来源：http://vuq.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mwl.shanyushiyangtech.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jux.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sjt.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wak.jianghu66.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xcv.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tfa.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bxo.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lia.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nqr.jianghu66.top

[E06] 替换子串
来源：http://pmj.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dsj.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://cto.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fkp.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://vdf.9152youxi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pvt.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://trf.daxiang520.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ynw.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://mxm.jinqigufen.top

[E07] 按分隔符拆分
来源：http://hkp.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lzw.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dsx.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://caz.yuanzhike.top

TS:   s.split(",")
来源：http://srv.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cys.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://voj.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://dfs.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://igh.bbcook.cn

[E08] 数组按分隔符合并
来源：http://mjc.tanke756.top

Py:   ",".join(items)
来源：http://dyr.xuanzx.com

PHP:  implode(",", $items);
来源：http://bhf.sjlbkw.cn

JS:   items.join(",")
来源：http://rtq.yj20258.top

TS:   items.join(",")
来源：http://pdm.meibo888.top

Java: String.join(",", items)
来源：http://rjg.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://hga.0kj1m.cn

Ruby: items.join(",")
来源：http://cbg.nwbrower.top

C#:   string.Join(",", items)
来源：http://kti.jqgufenzy.top

[E09] 去除所有空白字符
来源：http://kty.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zmo.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yby.bjfxy.top

JS:   s.replace(/\s+/g, "")
来源：http://hnj.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://qtl.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://zds.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yid.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://qgv.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qeb.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://cbp.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://akv.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rgl.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://mjy.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://pnu.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://zbe.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lto.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://inb.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://brv.shangyingyoupin.top

[E11] 反转字符串
来源：http://jdw.zdqjudy.top

Py:   s[::-1]
来源：http://wge.chenzaomai.com

PHP:  strrev($s);
来源：http://vkl.jiagoushi.top


<!-- 参考信息 -->