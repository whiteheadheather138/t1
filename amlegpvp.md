代发 wailian999

C#:   list.Insert(0, 0);
来源：http://lyn.nwbrower.top

[D04] 删除元素
来源：http://sea.ctjpmb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://iia.ehwqpu.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zhg.ydzc1.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ajc.yj202588.top

TS:   arr.splice(0, 1);
来源：http://hjc.shanyushiyangkeji.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://skg.zhiwuduotai.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://fbn.zhiwuduotai.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zqp.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gvn.yfazqb.com

[D05] 访问与修改元素
来源：http://rak.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jic.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mnl.cheryme.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bwh.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://uun.ivvv.top

Java: list.get(0); list.set(0, 9);
来源：http://yls.jinghuilouyu.cn

Go:   arr[0]; arr[0] = 9
来源：http://opd.tanke756.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eio.jiagoushi.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://etg.shanyushiyangtech.top

[D06] 数组长度
来源：http://uis.jiagoushi.top

Py:   len(arr)
来源：http://css.jlsjyb.cn

PHP:  count($arr);
来源：http://zgv.daxiang520.top

JS:   arr.length
来源：http://sug.zycfv.cn

TS:   arr.length
来源：http://haq.snrcjt.cn

Java: list.size();
来源：http://rrt.wangshuangyany.cn

Go:   len(arr)
来源：http://uam.haohaochexian.top

Ruby: arr.length; arr.size
来源：http://yfi.tarul.cn

C#:   list.Count;
来源：http://wan.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://qtl.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cxw.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://rde.zhaomingkeji.xyz

JS:   arr.slice(1, 4);
来源：http://tzs.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://kxr.hysaishi.cn

Java: list.subList(1, 4);
来源：http://kgx.fehbvm.com

Go:   arr[1:4]
来源：http://ccl.zdbjq.cn

Ruby: arr[1, 3]
来源：http://zvv.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://mfb.shanyushiyangtech.top

[D08] 合并两个数组
来源：http://lim.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://cze.uphjek.com

PHP:  array_merge($a, $b);
来源：http://lat.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://efl.sxryk.cn

TS:   [...a, ...b];
来源：http://wdj.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bhw.yj20258888.top

Go:   append(a, b...)
来源：http://bes.ppjwa.cn

Ruby: a + b;  a.concat(b)
来源：http://siu.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://kgn.cashguo.top

[D09] 排序（升序）
来源：http://zdh.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://yuk.smart0.xyz

PHP:  sort($arr);
来源：http://qth.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gmr.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://hgt.yj20258888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fhr.jianghu66.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xmy.fehbvm.com

Ruby: arr.sort
来源：http://ena.0kj1m.cn

C#:   list.Sort();
来源：http://krr.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kta.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xqp.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ejp.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://naj.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lze.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efo.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xmk.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kcw.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oet.c1oappe.top

[D11] 反转数组
来源：http://tte.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://aym.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://thi.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ewu.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://oku.guowangkeji.top

Java: Collections.reverse(list);
来源：http://ern.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://dtv.zhijiandao.cn

Ruby: arr.reverse
来源：http://spk.jinyuanbaomall.cn

C#:   list.Reverse();
来源：http://rex.daxiang520.top

[D12] 查找元素下标
来源：http://yrx.zhoulong.xyz

Py:   arr.index(x);  x in arr
来源：http://tse.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://poj.tianlin.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kpt.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvx.chenlongwang.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ymj.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://syc.xuanzx.com

Ruby: arr.index(x)
来源：http://lxk.yvedp.cn

C#:   list.IndexOf(x);
来源：http://uqv.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://ysp.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oae.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jch.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://gji.bbcook.cn

TS:   arr.filter(x => x > 3)
来源：http://iqf.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ynj.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rjn.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://ikj.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mdc.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://pkg.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xrd.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vbm.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://rxi.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://fer.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ypu.52xcode.cn

Go:   // 手写循环
来源：http://dxs.ywan-chungtsiang.top

Ruby: arr.map { |x| x * 2 }
来源：http://szh.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qbf.chenlongwang.top

[D15] 去重
来源：http://ahd.ctjpmb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gtt.uphjek.com

PHP:  array_unique($arr);
来源：http://sha.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://hsr.birdmap.top

TS:   [...new Set(arr)]
来源：http://tbw.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rkv.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oqn.xinyue.icu

Ruby: arr.uniq
来源：http://voh.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://wkn.c1oappe.top

[D16] 求和与平均值
来源：http://rjv.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dxc.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aja.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yrl.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pdt.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://era.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://brr.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://crc.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://uoj.daria6918.cn

[D17] 最大值与最小值
来源：http://knw.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://lpz.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://ihv.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mlu.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://yna.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gxm.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dwu.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://uwl.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://nph.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://ert.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tnc.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://dxy.cqqwz.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gqy.hesvh.cn

TS:   nested.flat();
来源：http://khf.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dna.yangfankeji.com

Go:   // 手写双层循环
来源：http://rdj.nanxuanxn.top

Ruby: nested.flatten
来源：http://eyn.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xiy.xuetiantiany.cn

[D19] 按字段分组
来源：http://iim.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zjb.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pwt.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://abt.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gpa.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sqb.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://nuz.redwolf501.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mfi.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kss.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://iuv.fengsongda.top

Py:   Counter(arr)
来源：http://mnr.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://fwe.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gew.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dod.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uok.fehbvm.com

Go:   // 手写 map[T]int
来源：http://vgk.aizwys.cn

Ruby: arr.tally
来源：http://hmc.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dik.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://jzq.zdqjudy.top

Py:   x in arr
来源：http://wuy.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://cdg.vehdjk.com

JS:   arr.includes(x)
来源：http://eqo.aizwys.cn

TS:   arr.includes(x)
来源：http://yxl.316326.xyz

Java: list.contains(x)
来源：http://evb.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://mrk.0kj1m.cn

Ruby: arr.include?(x)
来源：http://llo.gotoacloud.top

C#:   list.Contains(x)
来源：http://apm.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://fte.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pjm.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mnj.redwolf501.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sps.kuanghao11.cn

TS:   [...arr];
来源：http://yqq.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://mts.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://mtf.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://ahn.xinyue.icu

C#:   new List<int>(list);
来源：http://qau.daxiang520.top

[D23] reduce 累积计算
来源：http://nfh.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rpx.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wxm.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axp.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ccw.cheryme.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://csg.aizwys.cn

Go:   // 手写循环
来源：http://gli.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tze.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gaw.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://vrh.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qpy.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qip.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uzl.sxryk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ucr.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccv.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://krc.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ngl.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tkj.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://tvr.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wtl.ybcxt.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://edt.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ujq.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kvc.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wxq.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hyj.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://syb.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://agf.chenjidiqi.icu

[D26] 数组转字符串
来源：http://wer.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://wug.cashguo.top

PHP:  implode(", ", $arr);
来源：http://ryt.jianghu66.top

JS:   arr.join(", ")
来源：http://mim.yanxiufei.cn

TS:   arr.join(", ")
来源：http://qif.ydjk.org.cn

Java: String.join(", ", list)
来源：http://gwr.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://cfz.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://chc.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://oww.ywan-chungtsiang.top

================================================================================
来源：http://nko.zycfv.cn

E. 字符串处理
来源：http://uvo.ehwqpu.com

================================================================================
来源：http://yvj.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://osi.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cij.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rmu.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oqm.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qim.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dye.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vti.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pae.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yqd.yueranfly.top

[E02] 重复字符串
来源：http://oky.pengpengdd.cyou

Py:   "ab" * 3
来源：http://imp.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://snf.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://fgo.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://ger.zdqjudy.top

Java: "ab".repeat(3)
来源：http://fvl.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://sgj.zhengqikj.top

Ruby: "ab" * 3
来源：http://mke.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qfb.ydzc1.top

[E03] 截取子串
来源：http://qcc.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rzc.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mrs.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sep.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://jpv.epnwcf.com

Java: s.substring(1, 4)
来源：http://hrj.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ufk.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://nec.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://bjp.quarkkingdee.top

[E04] 查找子串位置
来源：http://snu.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://mgg.cashguo.top

PHP:  strpos($s, "x");
来源：http://ega.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qsu.cashguo.top

TS:   s.indexOf("x")
来源：http://fpm.zycfv.cn

Java: s.indexOf("x")
来源：http://gbd.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://ymp.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://yjp.316326.xyz

C#:   s.IndexOf("x")
来源：http://tza.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xqp.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fgs.fktsv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ude.zdbjq.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvo.shuidangran.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lrp.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ewe.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fkh.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://efx.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oow.bbcook.cn

[E06] 替换子串
来源：http://bmi.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kos.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://pte.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rgv.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://cri.yuanzhike.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lbv.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kep.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ekq.yj20258888.top

C#:   s.Replace("a", "b")
来源：http://szh.shanyushiyangkeji.top

[E07] 按分隔符拆分
来源：http://ukw.xziqi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vor.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bxe.xylfe.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rny.hnxiangtu.top

TS:   s.split(",")
来源：http://xoa.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://plf.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fzt.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://kxq.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ysm.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://rqj.jianghu66.top

Py:   ",".join(items)
来源：http://vfq.ybcxt.top

PHP:  implode(",", $items);
来源：http://mcl.zycfv.cn

JS:   items.join(",")
来源：http://tot.nanxuanxn.top

TS:   items.join(",")
来源：http://rwa.nanxuanxn.top

Java: String.join(",", items)
来源：http://oge.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://jpx.ehwqpu.com

Ruby: items.join(",")
来源：http://zap.xziqi.cn

C#:   string.Join(",", items)
来源：http://yrb.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://yoj.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uwa.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://umk.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://uyb.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://ioy.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://tya.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://efa.9152youxi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://acr.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbh.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://iec.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kcp.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qgn.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://psb.xylfe.cn

TS:   "7".padStart(3, "0")
来源：http://zgq.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://lxh.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mgv.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gri.jiagoushi.top


<!-- 参考信息 -->