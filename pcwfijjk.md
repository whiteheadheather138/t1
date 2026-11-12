代发 wailian999

C#:   list.Insert(0, 0);
来源：http://wdo.mhx1999.top

[D04] 删除元素
来源：http://xkl.shanyushiyangtech.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rcw.ivvv.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iok.ydjk.org.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://afh.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://ufm.ehwqpu.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://byi.fanxiaobao.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ekk.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wns.hysaishi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bci.yangfankeji.com

[D05] 访问与修改元素
来源：http://ssz.cdnleiting.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wsi.cucudq.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vhz.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vpf.yonumen.top

TS:   arr[0]; arr.at(-1);
来源：http://hwx.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://oaw.cqqwz.cn

Go:   arr[0]; arr[0] = 9
来源：http://cvw.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yjo.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://coh.nanxinkj.top

[D06] 数组长度
来源：http://sju.jinqigufen.top

Py:   len(arr)
来源：http://uhw.shangyingyoupin.top

PHP:  count($arr);
来源：http://tzq.iojbl.cn

JS:   arr.length
来源：http://nig.jyoumei.cn

TS:   arr.length
来源：http://dhx.jiagoushi.top

Java: list.size();
来源：http://ewi.shanyushiyangkeji.top

Go:   len(arr)
来源：http://oyw.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://dmy.sweek.top

C#:   list.Count;
来源：http://rsl.hesvh.cn

[D07] 切片 / 取子数组
来源：http://ouc.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://odb.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sja.cashguo.top

JS:   arr.slice(1, 4);
来源：http://psd.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://eca.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://hus.chenlongwang.top

Go:   arr[1:4]
来源：http://his.sjlbkw.cn

Ruby: arr[1, 3]
来源：http://htg.sweek.top

C#:   list.GetRange(1, 3);
来源：http://qmo.cheryme.top

[D08] 合并两个数组
来源：http://tlj.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://glt.aibaodan.cn

PHP:  array_merge($a, $b);
来源：http://zkk.xziqi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://iwm.xingfuxueyuan.xyz

TS:   [...a, ...b];
来源：http://qcn.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kto.zhengqikj.top

Go:   append(a, b...)
来源：http://gqi.guowangkeji.top

Ruby: a + b;  a.concat(b)
来源：http://hbc.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://inm.yuanzhike.top

[D09] 排序（升序）
来源：http://xmi.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://eqr.redwolf501.top

PHP:  sort($arr);
来源：http://jie.hnqzz.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eoj.tianlin.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://jky.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xnd.fengsongda.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ked.chenjidiqi.icu

Ruby: arr.sort
来源：http://nkf.jqgfzy.top

C#:   list.Sort();
来源：http://kvm.xylfe.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mmj.feifeiyinyue.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pld.quarkkingdee.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hai.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvx.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bou.sxryk.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bye.redwolf501.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qfo.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uiu.jinqigfzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kpc.xuetiantiany.cn

[D11] 反转数组
来源：http://yjf.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fis.daria6918.cn

PHP:  array_reverse($arr);
来源：http://wqu.ctjpmb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://egy.tanke756.top

TS:   [...arr].reverse();
来源：http://fno.chenlongwang.top

Java: Collections.reverse(list);
来源：http://ivc.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://mjf.epnwcf.com

Ruby: arr.reverse
来源：http://phh.zhoulong.xyz

C#:   list.Reverse();
来源：http://nxg.uphjek.com

[D12] 查找元素下标
来源：http://qkz.pengpengdd.cyou

Py:   arr.index(x);  x in arr
来源：http://dip.ybcxt.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://waf.yanxiufei.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lay.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sby.nanxuanxn.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oxs.hcnkem.com

Go:   slices.Index(arr, x)
来源：http://nib.jianghu66.top

Ruby: arr.index(x)
来源：http://wzn.hammf.cn

C#:   list.IndexOf(x);
来源：http://htd.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://mma.kuanghao11.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://egl.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://geo.yj202588.top

JS:   arr.filter(x => x > 3)
来源：http://bvg.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://fjs.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xvv.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qwk.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://tls.hnxiangtu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pox.zdqjudy.top

[D14] 映射转换（每个元素变形）
来源：http://akx.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fqn.cdnleiting.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cle.cdnleiting.top

JS:   arr.map(x => x * 2)
来源：http://srg.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://lqq.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uvc.ydjk.org.cn

Go:   // 手写循环
来源：http://njo.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://uoo.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://mps.zhixingplan.top

[D15] 去重
来源：http://fds.yj202588.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nnu.cheryme.top

PHP:  array_unique($arr);
来源：http://ikb.feifeiyinyue.top

JS:   [...new Set(arr)]
来源：http://roi.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://zbb.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://msn.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vgx.redwolf501.top

Ruby: arr.uniq
来源：http://trb.zdqjudy.top

C#:   list.Distinct().ToList()
来源：http://hin.jinyuanbaomall.cn

[D16] 求和与平均值
来源：http://tdn.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qpl.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://anc.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://frk.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sle.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pjo.cucudq.cn

Go:   // 手写循环累加
来源：http://mll.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uvk.bjfxy.top

C#:   list.Sum();  list.Average()
来源：http://lmt.xuanzx.com

[D17] 最大值与最小值
来源：http://dqc.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://lho.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://hbc.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aby.zdqjudy.top

TS:   Math.max(...arr);
来源：http://mcl.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kmr.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dxc.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://dxz.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://tcy.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://kee.mhx1999.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dcv.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://jdh.wangdashe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://scw.jqgfzy.top

TS:   nested.flat();
来源：http://oyr.shuidangran.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ybx.hcnkem.com

Go:   // 手写双层循环
来源：http://xux.xinyue.icu

Ruby: nested.flatten
来源：http://fuy.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uuf.aizwys.cn

[D19] 按字段分组
来源：http://mba.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jlk.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kim.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgx.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wod.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rxj.ivvv.top

Go:   // 手写 map[string][]T
来源：http://udr.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://spj.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://poq.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://tlv.hywenlv.cn

Py:   Counter(arr)
来源：http://mzi.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://kff.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qtl.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xlf.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gtx.hnqzz.top

Go:   // 手写 map[T]int
来源：http://yxm.uphjek.com

Ruby: arr.tally
来源：http://uuy.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pqg.yj202588.top

[D21] 判断是否包含某元素
来源：http://hri.ydzc1.top

Py:   x in arr
来源：http://ufc.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://wih.epnwcf.com

JS:   arr.includes(x)
来源：http://oiy.jiagoushi.top

TS:   arr.includes(x)
来源：http://jwf.bbcook.cn

Java: list.contains(x)
来源：http://qur.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://bhu.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://wcj.fanxiaobao.xyz

C#:   list.Contains(x)
来源：http://aro.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://som.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gwp.zdqjudy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hxs.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kkv.ctjpmb.com

TS:   [...arr];
来源：http://ugu.jinqigufen.top

Java: new ArrayList<>(list);
来源：http://yym.ppjwa.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zbu.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://uot.jyoumei.cn

C#:   new List<int>(list);
来源：http://wji.dashuyun.cn

[D23] reduce 累积计算
来源：http://vow.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nbx.zhijiandao.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://clw.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ors.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szo.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hxb.sysykeji.top

Go:   // 手写循环
来源：http://yoo.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pab.vqdsnc.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hjz.haohaochexian.top

[D24] 字典 / Map 基本操作
来源：http://fvc.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pth.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aua.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vxd.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vxy.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://giq.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kcb.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wrn.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yhg.bjfxy.top

[D25] Set 集合去重与交并差
来源：http://ncl.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fcu.tian-w.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://inr.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vwl.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dey.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ieu.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jlv.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://khc.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pof.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://nxu.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://dex.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://fjc.zhongyouzk.top

JS:   arr.join(", ")
来源：http://cnk.jlsjyb.cn

TS:   arr.join(", ")
来源：http://mhm.yj202588.top

Java: String.join(", ", list)
来源：http://xyt.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://svg.jyoumei.cn

Ruby: arr.join(", ")
来源：http://fuz.yfazqb.com

C#:   string.Join(", ", list)
来源：http://kdq.meibo888.top

================================================================================
来源：http://wwm.xylfe.cn

E. 字符串处理
来源：http://nhq.gogol.net.cn

================================================================================
来源：http://qjs.shangyingyoupin.top

[E01] 拼接字符串
来源：http://fnv.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vra.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://woi.vqdsnc.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jzq.epnwcf.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vwn.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://det.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bql.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rfu.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hve.epnwcf.com

[E02] 重复字符串
来源：http://pqp.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://fbb.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://ibw.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://uas.wangdashe.top

TS:   "ab".repeat(3)
来源：http://ejt.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://dlw.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://dgy.ivvv.top

Ruby: "ab" * 3
来源：http://mug.fehbvm.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vir.ctjpmb.com

[E03] 截取子串
来源：http://egx.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cjk.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ldi.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dzn.ivvv.top

TS:   s.slice(1, 4)
来源：http://efn.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://ewf.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gxn.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kdq.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://jxx.yfazqb.com

[E04] 查找子串位置
来源：http://nih.c1oappe.top

Py:   s.find("x");  s.index("x")
来源：http://snl.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://rvw.jianghu66.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zpf.zycfv.cn

TS:   s.indexOf("x")
来源：http://frk.zhiwuduotai.top

Java: s.indexOf("x")
来源：http://bst.tanke756.top

Go:   strings.Index(s, "x")
来源：http://lco.52xcode.cn

Ruby: s.index("x")
来源：http://afv.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://fib.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hzp.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gxt.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cez.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jbu.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://azr.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bao.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qye.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hrk.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qtx.jyoumei.cn

[E06] 替换子串
来源：http://tvo.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xsw.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://noq.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nts.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://cqi.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mgv.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sja.zhongyouzk.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ynp.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://pjt.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://pza.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hss.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yly.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://axb.yueranfly.top

TS:   s.split(",")
来源：http://vbx.meibo888.top

Java: s.split(",");  s.split("\\s+")
来源：http://svk.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fsm.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://rfw.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xkj.andypj.xyz

[E08] 数组按分隔符合并
来源：http://zph.jinqigufen.top

Py:   ",".join(items)
来源：http://hkg.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://bps.jqgufenzy.top

JS:   items.join(",")
来源：http://vfw.zdqjudy.top

TS:   items.join(",")
来源：http://kle.yfazqb.com

Java: String.join(",", items)
来源：http://iun.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://zlh.shuidangran.top

Ruby: items.join(",")
来源：http://jdx.hywenlv.cn

C#:   string.Join(",", items)
来源：http://gtk.wangshuangyany.cn

[E09] 去除所有空白字符
来源：http://eep.redwolf501.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ldw.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://okm.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://lls.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://fjw.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://jso.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://phq.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://buv.epnwcf.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usn.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://zic.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hky.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://npr.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://qqe.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://fkj.fengsongda.top

Java: String.format("%03d", 7)
来源：http://mza.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hkx.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tpz.havefunace.top


<!-- 参考信息 -->