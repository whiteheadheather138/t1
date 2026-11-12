代发 wailian999

Java: list.add(4);
来源：http://biy.aizwys.cn

Go:   arr = append(arr, 4)
来源：http://ioo.jinghuilouyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://rub.sufxvd.cn

C#:   list.Add(4);
来源：http://bbf.ppjwa.cn

[D03] 在指定位置插入元素
来源：http://idv.bjfxy.top

Py:   arr.insert(0, 0)
来源：http://iqy.smart0.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://twj.yueranfly.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pgv.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://jdp.jinqigufen.top

Java: list.add(0, 0);
来源：http://qkk.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://okk.zdbjq.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bgn.shuidangran.top

C#:   list.Insert(0, 0);
来源：http://efr.shanyushiyangkeji.top

[D04] 删除元素
来源：http://utu.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tow.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jzc.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wdn.jinghuilouyu.cn

TS:   arr.splice(0, 1);
来源：http://ryg.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sdv.ehwqpu.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lum.daria6918.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ydc.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ihj.ydjk.org.cn

[D05] 访问与修改元素
来源：http://btv.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lrl.pengpengdd.cyou

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oec.yvedp.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sdo.gaohongyu789.top

TS:   arr[0]; arr.at(-1);
来源：http://tzz.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://ikz.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://usa.feifeiyinyue.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://edp.hysaishi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://opu.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://trs.jyoumei.cn

Py:   len(arr)
来源：http://bwh.shzxlz.cn

PHP:  count($arr);
来源：http://spz.ctjpmb.com

JS:   arr.length
来源：http://uui.hongshengwenyu.top

TS:   arr.length
来源：http://bdq.xylfe.cn

Java: list.size();
来源：http://bqi.fengsongda.top

Go:   len(arr)
来源：http://tie.daria6918.cn

Ruby: arr.length; arr.size
来源：http://ymj.snrcjt.cn

C#:   list.Count;
来源：http://chc.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://utu.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jve.gaohongyu789.top

PHP:  array_slice($arr, 1, 3);
来源：http://hqo.jlsjyb.cn

JS:   arr.slice(1, 4);
来源：http://ewf.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://vft.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://bzx.bbcook.cn

Go:   arr[1:4]
来源：http://qts.jqgfzy.top

Ruby: arr[1, 3]
来源：http://xyw.wangshuangyany.cn

C#:   list.GetRange(1, 3);
来源：http://bbw.svipenyu.cn

[D08] 合并两个数组
来源：http://oon.cqqwz.cn

Py:   a + b;  a.extend(b)
来源：http://hjz.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://qdq.cdnleiting.top

JS:   [...a, ...b];  a.concat(b);
来源：http://mbb.gotoacloud.top

TS:   [...a, ...b];
来源：http://hmv.0kj1m.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cbq.daxiang520.top

Go:   append(a, b...)
来源：http://alv.jqgfzy.top

Ruby: a + b;  a.concat(b)
来源：http://lpc.sjlbkw.cn

C#:   a.Concat(b).ToList()
来源：http://eux.0kj1m.cn

[D09] 排序（升序）
来源：http://uwp.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ttg.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://pgf.guannengcc.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ijg.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://abp.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qud.zycfv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tli.ybcxt.top

Ruby: arr.sort
来源：http://vuf.gogol.net.cn

C#:   list.Sort();
来源：http://arr.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xsc.tanke756.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://evf.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://heg.yuanzhike.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gwd.chenlongwang.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ayi.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hsd.kuanghao11.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qra.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xwf.wangdashe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lxo.yj20258888.top

[D11] 反转数组
来源：http://baw.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://kig.chenjidiqi.icu

PHP:  array_reverse($arr);
来源：http://wth.zhiwuduotai.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ovk.jqgfzy.top

TS:   [...arr].reverse();
来源：http://bij.ppjwa.cn

Java: Collections.reverse(list);
来源：http://fvv.52xcode.cn

Go:   slices.Reverse(arr)
来源：http://inh.c1oappe.top

Ruby: arr.reverse
来源：http://pjq.feifeiyinyue.top

C#:   list.Reverse();
来源：http://ttg.kuanghao11.cn

[D12] 查找元素下标
来源：http://gya.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://alr.mhx1999.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tob.wangshuangyany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hko.hammf.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gvf.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ngn.cheryme.top

Go:   slices.Index(arr, x)
来源：http://znb.sysykeji.top

Ruby: arr.index(x)
来源：http://hiq.fengsongda.top

C#:   list.IndexOf(x);
来源：http://rzw.sufxvd.cn

[D13] 过滤（保留满足条件的）
来源：http://fvy.zhixingplan.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://llo.hammf.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rhv.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://oww.xingfuxueyuan.xyz

TS:   arr.filter(x => x > 3)
来源：http://bxq.jyoumei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://upl.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uer.0kj1m.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xqi.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gfm.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://twh.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kly.fktsv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xal.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://jhy.gzhubu.top

TS:   arr.map(x => x * 2)
来源：http://tnw.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://taz.daxiang520.top

Go:   // 手写循环
来源：http://ojd.zdbjq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fxw.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hno.jinqigfzy.top

[D15] 去重
来源：http://omz.9152youxi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rsi.hysaishi.cn

PHP:  array_unique($arr);
来源：http://ubr.zhongyouzk.top

JS:   [...new Set(arr)]
来源：http://cvv.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://rls.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eye.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://lga.vqdsnc.cn

Ruby: arr.uniq
来源：http://llg.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://ama.guowangkeji.top

[D16] 求和与平均值
来源：http://tsv.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wcs.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pde.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ehy.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xlc.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rxi.shuidangran.top

Go:   // 手写循环累加
来源：http://pts.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sjm.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://iik.fzhhl.top

[D17] 最大值与最小值
来源：http://kwr.yj20258.top

Py:   max(arr);  min(arr)
来源：http://dex.bbcook.cn

PHP:  max($arr);  min($arr);
来源：http://fvd.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qsy.uphjek.com

TS:   Math.max(...arr);
来源：http://klj.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://dho.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dkf.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://weh.tarul.cn

C#:   list.Max();  list.Min()
来源：http://yyo.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://adg.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gjv.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://kng.zhiwuduotai.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://msw.tian-w.cn

TS:   nested.flat();
来源：http://wou.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eol.sysykeji.top

Go:   // 手写双层循环
来源：http://cyu.tianlin.xyz

Ruby: nested.flatten
来源：http://kna.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uvz.feifeiyinyue.top

[D19] 按字段分组
来源：http://bdu.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nta.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://olf.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://flv.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://bvp.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wos.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://qzq.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://skh.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://obn.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://gtp.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://heu.gotoacloud.top

PHP:  array_count_values($arr);
来源：http://cvl.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bkx.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfm.dashuyun.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://azv.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://xav.zhengqikj.top

Ruby: arr.tally
来源：http://azv.feifeiyinyue.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://joc.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://yyj.shzxlz.cn

Py:   x in arr
来源：http://poj.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://eta.meibo888.top

JS:   arr.includes(x)
来源：http://luf.aibaodan.cn

TS:   arr.includes(x)
来源：http://xjb.fktsv.cn

Java: list.contains(x)
来源：http://cyw.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://sip.hcnkem.com

Ruby: arr.include?(x)
来源：http://wkt.shuidangran.top

C#:   list.Contains(x)
来源：http://azv.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://tit.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://two.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kpm.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ore.shzxlz.cn

TS:   [...arr];
来源：http://bvn.bjfxy.top

Java: new ArrayList<>(list);
来源：http://zvi.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://fzw.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://ubi.guowangkeji.top

C#:   new List<int>(list);
来源：http://jyr.xziqi.cn

[D23] reduce 累积计算
来源：http://tfg.yj20258.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yko.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://acj.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vip.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yen.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dkw.pengpengdd.cyou

Go:   // 手写循环
来源：http://jmq.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zjv.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://msr.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://duy.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zdy.ppjwa.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hmj.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vzc.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xxs.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jux.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qwf.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vhm.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rgg.chenlongwang.top

[D25] Set 集合去重与交并差
来源：http://uql.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ict.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zav.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zfu.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xgl.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bhq.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eum.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sol.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wfd.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://nfs.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://awi.yj20258.top

PHP:  implode(", ", $arr);
来源：http://nln.daxiang520.top

JS:   arr.join(", ")
来源：http://xis.shzxlz.cn

TS:   arr.join(", ")
来源：http://bfo.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://vou.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://aoq.gzhubu.top

Ruby: arr.join(", ")
来源：http://rqb.sxryk.cn

C#:   string.Join(", ", list)
来源：http://kqy.meibo888.top

================================================================================
来源：http://yer.fehbvm.com

E. 字符串处理
来源：http://cag.ywan-chungtsiang.top

================================================================================
来源：http://ggd.yuanzhike.top

[E01] 拼接字符串
来源：http://pmr.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://piw.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wcf.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dnq.gaohongyu789.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lse.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ovc.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pbl.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://axb.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gtx.sjlbkw.cn

[E02] 重复字符串
来源：http://wpz.ctjpmb.com

Py:   "ab" * 3
来源：http://etg.jlsjyb.cn

PHP:  str_repeat("ab", 3);
来源：http://tjf.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://zph.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://kfm.ybcxt.top

Java: "ab".repeat(3)
来源：http://uyp.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://abt.gogol.net.cn

Ruby: "ab" * 3
来源：http://deg.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ide.wangshuangyany.cn

[E03] 截取子串
来源：http://wxi.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wtz.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fny.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ooi.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://bqq.shzxlz.cn

Java: s.substring(1, 4)
来源：http://qtu.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://moe.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://imb.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://bmp.shangyingyoupin.top

[E04] 查找子串位置
来源：http://xst.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://mxx.bjfxy.top

PHP:  strpos($s, "x");
来源：http://enu.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qre.sufxvd.cn

TS:   s.indexOf("x")
来源：http://zxm.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://pev.0kj1m.cn

Go:   strings.Index(s, "x")
来源：http://emk.ydjk.org.cn

Ruby: s.index("x")
来源：http://unn.tarul.cn

C#:   s.IndexOf("x")
来源：http://wfl.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://svj.ivvv.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kns.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fzc.c1oappe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xip.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cjh.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xfd.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rtm.yj202588.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uls.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kkd.wangdashe.top

[E06] 替换子串
来源：http://efe.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rrz.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jea.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tet.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://evf.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wlo.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fst.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ali.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://zoc.jianghu66.top

[E07] 按分隔符拆分
来源：http://cda.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gat.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mcn.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lfz.epnwcf.com

TS:   s.split(",")
来源：http://dbp.guowangkeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://lrc.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eyo.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://cmo.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nfh.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://jkt.cucudq.cn

Py:   ",".join(items)
来源：http://tst.haohaochexian.top

PHP:  implode(",", $items);
来源：http://onp.kuanghao11.cn

JS:   items.join(",")
来源：http://gfn.chenlongwang.top

TS:   items.join(",")
来源：http://ifx.bjfxy.top

Java: String.join(",", items)
来源：http://kga.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://gxf.tian-w.cn

Ruby: items.join(",")
来源：http://jqs.yonumen.top

C#:   string.Join(",", items)
来源：http://sho.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://bcc.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fbk.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xce.yj20258888.top

JS:   s.replace(/\s+/g, "")
来源：http://exw.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://ekc.daxiang520.top


<!-- 参考信息 -->