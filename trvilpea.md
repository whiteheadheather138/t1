代发 wailian999

C#:   list.Insert(0, 0);
来源：http://dpa.shanyushiyangtech.top

[D04] 删除元素
来源：http://niw.jqgfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://das.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uvm.jinyuanbaomall.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hpj.shzxlz.cn

TS:   arr.splice(0, 1);
来源：http://kum.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gke.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://unu.yuanzhike.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mms.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yqs.wangshuangyany.cn

[D05] 访问与修改元素
来源：http://xrk.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://oer.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ttc.hesvh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pwd.fehbvm.com

TS:   arr[0]; arr.at(-1);
来源：http://gik.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://ecd.sxryk.cn

Go:   arr[0]; arr[0] = 9
来源：http://qpz.xziqi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://czz.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uam.ivvv.top

[D06] 数组长度
来源：http://bqf.yuxming.cn

Py:   len(arr)
来源：http://biv.shzxlz.cn

PHP:  count($arr);
来源：http://dnt.redwolf501.top

JS:   arr.length
来源：http://qxc.fengsongda.top

TS:   arr.length
来源：http://zzx.fengsongda.top

Java: list.size();
来源：http://xrd.shanyushiyangkeji.top

Go:   len(arr)
来源：http://ngo.yfazqb.com

Ruby: arr.length; arr.size
来源：http://kew.hammf.cn

C#:   list.Count;
来源：http://jux.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://ovn.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://noy.hywenlv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gxg.ctjpmb.com

JS:   arr.slice(1, 4);
来源：http://trj.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://myu.yvedp.cn

Java: list.subList(1, 4);
来源：http://ynb.hammf.cn

Go:   arr[1:4]
来源：http://loy.ivvv.top

Ruby: arr[1, 3]
来源：http://nsf.dianchejie.cn

C#:   list.GetRange(1, 3);
来源：http://auf.tarul.cn

[D08] 合并两个数组
来源：http://shx.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://tde.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://nhy.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ffp.zdqjudy.top

TS:   [...a, ...b];
来源：http://ewp.hcnkem.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mbo.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://dvb.hcnkem.com

Ruby: a + b;  a.concat(b)
来源：http://kwl.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://zeb.quarkkingdee.top

[D09] 排序（升序）
来源：http://kwc.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://mzr.yj202588.top

PHP:  sort($arr);
来源：http://odb.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dha.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kqt.hcnkem.com

Java: Collections.sort(list);  list.sort(null);
来源：http://tax.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zso.uphjek.com

Ruby: arr.sort
来源：http://kzz.sjlbkw.cn

C#:   list.Sort();
来源：http://ivh.ydjk.org.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://xnm.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ozi.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kle.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xkc.vehdjk.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tyn.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xzj.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://biq.chenzaomai.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xzz.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qzr.gogol.net.cn

[D11] 反转数组
来源：http://xfi.yanxiufei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jta.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://qti.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gnq.jinqigufen.top

TS:   [...arr].reverse();
来源：http://tfn.iojbl.cn

Java: Collections.reverse(list);
来源：http://sdu.cheryme.top

Go:   slices.Reverse(arr)
来源：http://doa.jqgufenzy.top

Ruby: arr.reverse
来源：http://mpw.haohaochexian.top

C#:   list.Reverse();
来源：http://hof.cqqwz.cn

[D12] 查找元素下标
来源：http://npy.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://ixy.fktsv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lbc.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nta.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djv.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cau.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://nnk.cheryme.top

Ruby: arr.index(x)
来源：http://rro.zycfv.cn

C#:   list.IndexOf(x);
来源：http://sjp.yfazqb.com

[D13] 过滤（保留满足条件的）
来源：http://agv.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mwh.gotoacloud.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dhp.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://mzn.iojbl.cn

TS:   arr.filter(x => x > 3)
来源：http://ttb.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qtv.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cyt.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gnj.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://eaj.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://oyu.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ecc.zhongyouzk.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fhj.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://siv.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://eph.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://cqu.xylfe.cn

Go:   // 手写循环
来源：http://tkj.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://szh.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lal.fktsv.cn

[D15] 去重
来源：http://syr.jinqigufen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gzy.sysykeji.top

PHP:  array_unique($arr);
来源：http://pqb.zycfv.cn

JS:   [...new Set(arr)]
来源：http://bnu.nwbrower.top

TS:   [...new Set(arr)]
来源：http://ydj.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aew.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://enx.wangshuangyany.cn

Ruby: arr.uniq
来源：http://utw.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://bwq.jianghu66.top

[D16] 求和与平均值
来源：http://ztb.svipenyu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bsp.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fov.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://abd.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tzx.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aqx.316326.xyz

Go:   // 手写循环累加
来源：http://rpe.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jvy.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://smo.havefunace.top

[D17] 最大值与最小值
来源：http://nfy.fktsv.cn

Py:   max(arr);  min(arr)
来源：http://vsv.fzhhl.top

PHP:  max($arr);  min($arr);
来源：http://ysj.vqdsnc.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lls.9152youxi.cn

TS:   Math.max(...arr);
来源：http://cno.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fsf.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qax.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://tmn.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://uhh.jqgfzy.top

[D18] 扁平化嵌套数组
来源：http://had.haohaochexian.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sfo.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://mie.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qis.yangfankeji.com

TS:   nested.flat();
来源：http://hzr.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gkp.sweek.top

Go:   // 手写双层循环
来源：http://nal.shzxlz.cn

Ruby: nested.flatten
来源：http://koq.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gdb.zhixingplan.top

[D19] 按字段分组
来源：http://ato.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gmo.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ybu.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nkl.wangshuangyany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jfo.tian-w.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tvy.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://ppl.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://rex.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ojf.jyoumei.cn

[D20] 统计每个元素出现次数
来源：http://ayt.ydzc1.top

Py:   Counter(arr)
来源：http://gpc.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://aqv.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rkc.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://emg.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lbs.nwbrower.top

Go:   // 手写 map[T]int
来源：http://fas.fengsongda.top

Ruby: arr.tally
来源：http://hpp.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mck.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://aka.xuanzx.com

Py:   x in arr
来源：http://gqm.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://zlf.zhoulong.xyz

JS:   arr.includes(x)
来源：http://kmy.nwbrower.top

TS:   arr.includes(x)
来源：http://pth.wangdashe.top

Java: list.contains(x)
来源：http://rpe.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://awl.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://wil.nanxinkj.top

C#:   list.Contains(x)
来源：http://tro.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://lgy.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://byq.cheryme.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sxb.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lci.fanxiaobao.xyz

TS:   [...arr];
来源：http://lup.andypj.xyz

Java: new ArrayList<>(list);
来源：http://xzp.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://fou.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://csx.haohaochexian.top

C#:   new List<int>(list);
来源：http://ccz.aibaodan.cn

[D23] reduce 累积计算
来源：http://puu.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eil.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://csj.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ooj.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjl.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vgp.ivvv.top

Go:   // 手写循环
来源：http://ovl.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sue.bbcook.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hyp.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://lvn.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xbl.hammf.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fwe.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lsh.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cjy.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://knz.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hyf.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://grh.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aaz.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://blx.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cyg.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://owr.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ntm.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wag.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uih.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zut.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://biq.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qso.wangshuangyany.cn

[D26] 数组转字符串
来源：http://bmi.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://vwb.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://rgi.jlsjyb.cn

JS:   arr.join(", ")
来源：http://vtu.fehbvm.com

TS:   arr.join(", ")
来源：http://xgc.gotoacloud.top

Java: String.join(", ", list)
来源：http://fpl.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://vvw.52xcode.cn

Ruby: arr.join(", ")
来源：http://fde.epnwcf.com

C#:   string.Join(", ", list)
来源：http://jee.yfazqb.com

================================================================================
来源：http://spx.tanke756.top

E. 字符串处理
来源：http://sip.birdmap.top

================================================================================
来源：http://cir.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://xqe.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://szp.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cwz.jiagoushi.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://euo.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lez.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ocz.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yya.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nmx.guowangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://peq.yuanzhike.top

[E02] 重复字符串
来源：http://svj.cashguo.top

Py:   "ab" * 3
来源：http://xwe.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://sax.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://qwf.sjlbkw.cn

TS:   "ab".repeat(3)
来源：http://rbr.gotoacloud.top

Java: "ab".repeat(3)
来源：http://vwc.jlsjyb.cn

Go:   strings.Repeat("ab", 3)
来源：http://qsj.jinqigufen.top

Ruby: "ab" * 3
来源：http://jpb.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vgs.hongshengwenyu.top

[E03] 截取子串
来源：http://tpa.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://suq.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lxy.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wbh.bbcook.cn

TS:   s.slice(1, 4)
来源：http://owp.ivvv.top

Java: s.substring(1, 4)
来源：http://fth.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ydc.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zpt.pycfn.com

C#:   s.Substring(1, 3)
来源：http://zgo.feifeiyinyue.top

[E04] 查找子串位置
来源：http://dce.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://vqb.pengpengdd.cyou

PHP:  strpos($s, "x");
来源：http://xfj.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iqu.uphjek.com

TS:   s.indexOf("x")
来源：http://ixw.aizwys.cn

Java: s.indexOf("x")
来源：http://ysh.guowangkeji.top

Go:   strings.Index(s, "x")
来源：http://evm.aizwys.cn

Ruby: s.index("x")
来源：http://lzk.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://zwg.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://sii.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tem.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qbo.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmy.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://piz.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nzz.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hzh.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pse.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oyy.jqgfzy.top

[E06] 替换子串
来源：http://msi.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yev.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://klv.wangshuangyany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdo.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://gep.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nxi.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dwf.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://int.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://jsd.redwolf501.top

[E07] 按分隔符拆分
来源：http://vwe.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://clx.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nbh.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hwc.chenjidiqi.icu

TS:   s.split(",")
来源：http://krn.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://nod.xinyue.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hmb.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://ujz.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uus.sxryk.cn

[E08] 数组按分隔符合并
来源：http://rqh.yfazqb.com

Py:   ",".join(items)
来源：http://woe.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://sym.hongshengwenyu.top

JS:   items.join(",")
来源：http://ing.nanxinkj.top

TS:   items.join(",")
来源：http://dly.jlsjyb.cn

Java: String.join(",", items)
来源：http://zvu.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://czy.nwbrower.top

Ruby: items.join(",")
来源：http://cea.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://prd.yuanzhike.top

[E09] 去除所有空白字符
来源：http://bbv.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jjm.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tpc.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://sav.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://qrm.bjfxy.top

Java: s.replaceAll("\\s+", "")
来源：http://roa.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pwj.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://nbi.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jib.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://syx.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nfr.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dvs.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://rgq.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://jko.uphjek.com

Java: String.format("%03d", 7)
来源：http://xdd.zhoulong.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ujv.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xza.jlsjyb.cn


<!-- 参考信息 -->