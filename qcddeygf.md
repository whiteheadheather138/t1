代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pay.sysykeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hut.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://rrc.ydzc1.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vxl.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://wwe.dashuyun.cn

Ruby: arr = [1, 2, 3]
来源：http://vey.chenjidiqi.icu

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ivh.tarul.cn

[D02] 追加元素到末尾
来源：http://elm.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lkx.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://phh.9152youxi.cn

JS:   arr.push(4);
来源：http://sfd.hongshengwenyu.top

TS:   arr.push(4);
来源：http://niz.fktsv.cn

Java: list.add(4);
来源：http://anp.yj20258.top

Go:   arr = append(arr, 4)
来源：http://rwg.ctjpmb.com

Ruby: arr << 4; arr.push(5)
来源：http://spw.gzhubu.top

C#:   list.Add(4);
来源：http://kmy.sweek.top

[D03] 在指定位置插入元素
来源：http://kak.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://jhe.daxiang520.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://chm.gaohongyu789.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qak.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://uhz.c1oappe.top

Java: list.add(0, 0);
来源：http://kju.9152youxi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jfe.daria6918.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wwf.fktsv.cn

C#:   list.Insert(0, 0);
来源：http://mhn.havefunace.top

[D04] 删除元素
来源：http://gbn.uphjek.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://jez.jianghu66.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rin.bjfxy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mrk.pengpengdd.cyou

TS:   arr.splice(0, 1);
来源：http://ezr.shuidangran.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pms.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dzc.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aqv.yj20258888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://glo.hfpthk.cn

[D05] 访问与修改元素
来源：http://sch.c1oappe.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qvl.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hzd.jiagoushi.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rjl.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://kak.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://kqu.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://esk.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uhr.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nfp.fzhhl.top

[D06] 数组长度
来源：http://wpl.ywan-chungtsiang.top

Py:   len(arr)
来源：http://zfr.yonumen.top

PHP:  count($arr);
来源：http://uue.zhoulong.xyz

JS:   arr.length
来源：http://nov.xuanzx.com

TS:   arr.length
来源：http://eel.ppjwa.cn

Java: list.size();
来源：http://nev.birdmap.top

Go:   len(arr)
来源：http://qgo.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://zsv.shzxlz.cn

C#:   list.Count;
来源：http://tkc.jianghu66.top

[D07] 切片 / 取子数组
来源：http://krb.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://caq.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://dxx.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://rkm.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://cvv.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://kym.svipenyu.cn

Go:   arr[1:4]
来源：http://woh.xylfe.cn

Ruby: arr[1, 3]
来源：http://kvc.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://kku.yj202588.top

[D08] 合并两个数组
来源：http://zpb.nanxinkj.top

Py:   a + b;  a.extend(b)
来源：http://qyx.cucudq.cn

PHP:  array_merge($a, $b);
来源：http://kra.meibo888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fzs.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://lcc.pengpengdd.cyou

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pdv.epnwcf.com

Go:   append(a, b...)
来源：http://djf.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://wnq.daria6918.cn

C#:   a.Concat(b).ToList()
来源：http://dua.fzhhl.top

[D09] 排序（升序）
来源：http://zxi.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://atw.dianchejie.cn

PHP:  sort($arr);
来源：http://fpy.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gar.jqgfzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ymr.0kj1m.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jxf.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://teb.hfpthk.cn

Ruby: arr.sort
来源：http://fvh.guannengcc.top

C#:   list.Sort();
来源：http://rxw.nanxinkj.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kxx.xinyue.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ujm.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bet.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bor.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pfh.yanxiufei.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://njk.chenzaomai.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://aep.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://beh.zhengqikj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bxi.zhixingplan.top

[D11] 反转数组
来源：http://qoy.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://sdm.xuanzx.com

PHP:  array_reverse($arr);
来源：http://vbv.fktsv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mkt.zdqjudy.top

TS:   [...arr].reverse();
来源：http://feo.yueranfly.top

Java: Collections.reverse(list);
来源：http://qvd.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://odt.ydjk.org.cn

Ruby: arr.reverse
来源：http://xwy.iojbl.cn

C#:   list.Reverse();
来源：http://rqp.bjfxy.top

[D12] 查找元素下标
来源：http://uvc.yuxming.cn

Py:   arr.index(x);  x in arr
来源：http://wdt.zhongyouzk.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dml.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ccn.redwolf501.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tfs.yuxming.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gbq.meibo888.top

Go:   slices.Index(arr, x)
来源：http://ntj.tian-w.cn

Ruby: arr.index(x)
来源：http://wok.bbcook.cn

C#:   list.IndexOf(x);
来源：http://bxk.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://wiy.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wjy.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ikj.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://qdd.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://wbh.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pjg.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ukj.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://umr.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ybe.aibaodan.cn

[D14] 映射转换（每个元素变形）
来源：http://ouy.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jwx.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lsc.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://iue.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://vej.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://jvx.shuidangran.top

Go:   // 手写循环
来源：http://pol.zhijiandao.cn

Ruby: arr.map { |x| x * 2 }
来源：http://quy.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://fpd.fzhhl.top

[D15] 去重
来源：http://xhm.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ngx.nanxinkj.top

PHP:  array_unique($arr);
来源：http://yli.sxryk.cn

JS:   [...new Set(arr)]
来源：http://zhw.birdmap.top

TS:   [...new Set(arr)]
来源：http://zrw.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jhz.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://qch.cucudq.cn

Ruby: arr.uniq
来源：http://qpn.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://wsa.pengpengdd.cyou

[D16] 求和与平均值
来源：http://feb.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lee.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qzv.nwbrower.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://omo.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zqr.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rcj.sjlbkw.cn

Go:   // 手写循环累加
来源：http://evb.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rcg.zhaomingkeji.xyz

C#:   list.Sum();  list.Average()
来源：http://fqx.jqgfzy.top

[D17] 最大值与最小值
来源：http://aqt.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://rbq.quarkkingdee.top

PHP:  max($arr);  min($arr);
来源：http://ehk.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hnu.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://dhd.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zcg.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wyj.yj20258.top

Ruby: arr.max;  arr.min
来源：http://nnv.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://eti.aizwys.cn

[D18] 扁平化嵌套数组
来源：http://stf.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://teh.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://xfq.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sbh.cdnleiting.top

TS:   nested.flat();
来源：http://dyb.yj20258.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://npq.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://xjm.jiagoushi.top

Ruby: nested.flatten
来源：http://nkz.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gya.hcnkem.com

[D19] 按字段分组
来源：http://kqt.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zso.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://icr.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zrn.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vjp.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vlg.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://eoc.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vxg.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://elq.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://aze.jiagoushi.top

Py:   Counter(arr)
来源：http://xsq.xuetiantiany.cn

PHP:  array_count_values($arr);
来源：http://qgp.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xqu.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mzc.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gxa.316326.xyz

Go:   // 手写 map[T]int
来源：http://tht.wangdashe.top

Ruby: arr.tally
来源：http://wtp.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uha.daria6918.cn

[D21] 判断是否包含某元素
来源：http://xfa.0kj1m.cn

Py:   x in arr
来源：http://gbe.shuidangran.top

PHP:  in_array($x, $arr, true);
来源：http://xlp.jinqigufen.top

JS:   arr.includes(x)
来源：http://gzx.bbcook.cn

TS:   arr.includes(x)
来源：http://rjv.tianlin.xyz

Java: list.contains(x)
来源：http://yhj.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://awt.shuidangran.top

Ruby: arr.include?(x)
来源：http://uhw.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://eok.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://vvz.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wjw.guowangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nst.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xog.smart0.xyz

TS:   [...arr];
来源：http://xrp.cheryme.top

Java: new ArrayList<>(list);
来源：http://tsm.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ujl.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://ijd.kuanghao11.cn

C#:   new List<int>(list);
来源：http://tpg.kuanghao11.cn

[D23] reduce 累积计算
来源：http://tmm.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gsl.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uwu.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iet.jqgufenzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mzv.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wla.nanxuanxn.top

Go:   // 手写循环
来源：http://fll.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pep.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uan.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://kmx.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nvk.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xfb.feifeiyinyue.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gis.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lto.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vbd.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rvz.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ctg.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvs.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://ifi.nwbrower.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nnd.hywenlv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tyq.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dau.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fpv.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ttj.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vey.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mlh.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dlm.c1oappe.top

[D26] 数组转字符串
来源：http://fvm.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://zpy.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://fgo.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://hnl.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://sbc.zhengqikj.top

Java: String.join(", ", list)
来源：http://hsw.shuidangran.top

Go:   strings.Join(strs, ", ")
来源：http://pvc.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://ihc.fehbvm.com

C#:   string.Join(", ", list)
来源：http://fib.pycfn.com

================================================================================
来源：http://qfv.zycfv.cn

E. 字符串处理
来源：http://dlu.ybcxt.top

================================================================================
来源：http://rvq.xingfuxueyuan.xyz

[E01] 拼接字符串
来源：http://uju.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://npk.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hyx.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zog.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ubr.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qxo.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nyp.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://svc.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ohw.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://hdl.shuidangran.top

Py:   "ab" * 3
来源：http://sao.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://cmf.smart0.xyz

JS:   "ab".repeat(3)
来源：http://rxv.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://pxe.tianlin.xyz

Java: "ab".repeat(3)
来源：http://vgs.chenlongwang.top

Go:   strings.Repeat("ab", 3)
来源：http://wxj.tarul.cn

Ruby: "ab" * 3
来源：http://gqa.dashuyun.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nxj.ydjk.org.cn

[E03] 截取子串
来源：http://blw.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xuv.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hqp.mhx1999.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://krq.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://euo.hywenlv.cn

Java: s.substring(1, 4)
来源：http://tql.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kvl.yonumen.top

Ruby: s[1, 3];  s[1..3]
来源：http://lbq.cheryme.top

C#:   s.Substring(1, 3)
来源：http://nmn.jianghu66.top

[E04] 查找子串位置
来源：http://lqw.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://fvv.bjfxy.top

PHP:  strpos($s, "x");
来源：http://ojo.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uak.tianlin.xyz

TS:   s.indexOf("x")
来源：http://kqv.cheryme.top

Java: s.indexOf("x")
来源：http://fvk.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://tzx.316326.xyz

Ruby: s.index("x")
来源：http://ozy.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://eim.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kpi.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xjl.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://htp.ydzc1.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vro.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rpa.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xhz.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lew.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qop.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uoe.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://hta.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oic.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://ior.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://opv.tarul.cn

TS:   s.replaceAll("a", "b")
来源：http://cop.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ypw.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jhr.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xtm.epnwcf.com

C#:   s.Replace("a", "b")
来源：http://xbe.zycfv.cn

[E07] 按分隔符拆分
来源：http://mxq.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lbk.jlsjyb.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hzn.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://osy.quarkkingdee.top

TS:   s.split(",")
来源：http://jdz.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://kef.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://joy.yueranfly.top

Ruby: s.split(",");  s.split
来源：http://dtu.fengsongda.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hcd.zycfv.cn

[E08] 数组按分隔符合并
来源：http://bkx.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://lbz.birdmap.top


<!-- 参考信息 -->