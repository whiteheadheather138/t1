代发 wailian999

Java: list.add(4);
来源：http://yof.gzhubu.top

Go:   arr = append(arr, 4)
来源：http://xsm.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://rjz.shangyingyoupin.top

C#:   list.Add(4);
来源：http://npm.sjlbkw.cn

[D03] 在指定位置插入元素
来源：http://ovf.cashguo.top

Py:   arr.insert(0, 0)
来源：http://ztw.wangdashe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://etk.fanxiaobao.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gwh.yuanzhike.top

TS:   arr.splice(0, 0, 0);
来源：http://omt.zhijiandao.cn

Java: list.add(0, 0);
来源：http://hbe.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://rmu.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ijo.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://tnc.sysykeji.top

[D04] 删除元素
来源：http://xpp.zhongyouzk.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://aeo.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zya.birdmap.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iyn.yuanzhike.top

TS:   arr.splice(0, 1);
来源：http://wfd.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lmu.hnqzz.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://frt.yongpay.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ezb.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nby.fengsongda.top

[D05] 访问与修改元素
来源：http://osy.shanyushiyangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bnd.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mpd.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zcr.jqgufenzy.top

TS:   arr[0]; arr.at(-1);
来源：http://lmv.sysykeji.top

Java: list.get(0); list.set(0, 9);
来源：http://hpi.yuxming.cn

Go:   arr[0]; arr[0] = 9
来源：http://xak.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vji.zhaomingkeji.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ies.zdqjudy.top

[D06] 数组长度
来源：http://glk.ctjpmb.com

Py:   len(arr)
来源：http://jtf.sjlbkw.cn

PHP:  count($arr);
来源：http://zqa.xylfe.cn

JS:   arr.length
来源：http://fuw.cucudq.cn

TS:   arr.length
来源：http://qpt.xuanzx.com

Java: list.size();
来源：http://dkj.gogol.net.cn

Go:   len(arr)
来源：http://hht.xinyue.icu

Ruby: arr.length; arr.size
来源：http://zkp.0kj1m.cn

C#:   list.Count;
来源：http://laf.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://dgc.hywenlv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dhi.jinqigufen.top

PHP:  array_slice($arr, 1, 3);
来源：http://fhi.yongpay.top

JS:   arr.slice(1, 4);
来源：http://tje.chenlongwang.top

TS:   arr.slice(1, 4);
来源：http://olb.c1oappe.top

Java: list.subList(1, 4);
来源：http://yjt.xziqi.cn

Go:   arr[1:4]
来源：http://len.gaohongyu789.top

Ruby: arr[1, 3]
来源：http://xaa.cucudq.cn

C#:   list.GetRange(1, 3);
来源：http://kyq.wangshuangyany.cn

[D08] 合并两个数组
来源：http://tsb.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://txf.haohaochexian.top

PHP:  array_merge($a, $b);
来源：http://zme.yongpay.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gzd.hesvh.cn

TS:   [...a, ...b];
来源：http://ewd.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ecl.fehbvm.com

Go:   append(a, b...)
来源：http://mvu.guannengcc.top

Ruby: a + b;  a.concat(b)
来源：http://aei.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://ixq.316326.xyz

[D09] 排序（升序）
来源：http://snh.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://zoq.xuanzx.com

PHP:  sort($arr);
来源：http://jnf.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://isw.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hbd.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lvh.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://alk.redwolf501.top

Ruby: arr.sort
来源：http://zsm.tian-w.cn

C#:   list.Sort();
来源：http://khi.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bks.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://grt.jinyuanbaomall.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bql.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://esa.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cxh.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vwy.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lrg.tianlin.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pob.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kxv.yj20258.top

[D11] 反转数组
来源：http://jyl.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://fpf.zycfv.cn

PHP:  array_reverse($arr);
来源：http://tgu.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://txl.chenjidiqi.icu

TS:   [...arr].reverse();
来源：http://skv.birdmap.top

Java: Collections.reverse(list);
来源：http://woi.yfazqb.com

Go:   slices.Reverse(arr)
来源：http://ipt.wangshuangyany.cn

Ruby: arr.reverse
来源：http://fkk.tian-w.cn

C#:   list.Reverse();
来源：http://skh.zhixingplan.top

[D12] 查找元素下标
来源：http://eqo.jinqigufen.top

Py:   arr.index(x);  x in arr
来源：http://ezi.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wyi.tarul.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xiv.sxryk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://edy.yonumen.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kjx.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://say.bjfxy.top

Ruby: arr.index(x)
来源：http://uwz.tarul.cn

C#:   list.IndexOf(x);
来源：http://ful.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://hml.smart0.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yqq.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hjq.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://yyq.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://yfl.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tzt.xinyue.icu

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://waa.daria6918.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ahk.quarkkingdee.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sgk.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://kyw.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://avg.jinghuilouyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mou.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://upc.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://iyh.fzhhl.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xme.yonumen.top

Go:   // 手写循环
来源：http://uwu.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bao.yonumen.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vqe.zhiwuduotai.top

[D15] 去重
来源：http://tss.gogol.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tfp.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://iey.xingfuxueyuan.xyz

JS:   [...new Set(arr)]
来源：http://zyn.cqqwz.cn

TS:   [...new Set(arr)]
来源：http://euy.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uwv.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://pge.chenjidiqi.icu

Ruby: arr.uniq
来源：http://fap.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://lbk.jlsjyb.cn

[D16] 求和与平均值
来源：http://fvm.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oea.jlsjyb.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cda.hammf.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gle.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sed.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dzp.xuanzx.com

Go:   // 手写循环累加
来源：http://iyy.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eip.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://lrj.hesvh.cn

[D17] 最大值与最小值
来源：http://mfi.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://lnc.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://ovh.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qnm.bjfxy.top

TS:   Math.max(...arr);
来源：http://yun.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://msk.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iqv.52xcode.cn

Ruby: arr.max;  arr.min
来源：http://cfd.pycfn.com

C#:   list.Max();  list.Min()
来源：http://qer.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://day.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dsb.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://tck.jinghuilouyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xng.vehdjk.com

TS:   nested.flat();
来源：http://avd.jinyuanbaomall.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ahv.nanxinkj.top

Go:   // 手写双层循环
来源：http://wuj.sweek.top

Ruby: nested.flatten
来源：http://ytt.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jow.wangdashe.top

[D19] 按字段分组
来源：http://ihu.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hmt.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dyw.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hmy.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xnq.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yke.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://yuk.havefunace.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eor.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oni.gaohongyu789.top

[D20] 统计每个元素出现次数
来源：http://nzg.gogol.net.cn

Py:   Counter(arr)
来源：http://ipc.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://psq.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eds.yj20258.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pwn.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://djh.tanke756.top

Go:   // 手写 map[T]int
来源：http://tsi.dashuyun.cn

Ruby: arr.tally
来源：http://gba.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dmu.jiagoushi.top

[D21] 判断是否包含某元素
来源：http://isd.hnqzz.top

Py:   x in arr
来源：http://azy.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://ebn.ehwqpu.com

JS:   arr.includes(x)
来源：http://fho.cucudq.cn

TS:   arr.includes(x)
来源：http://yqr.hesvh.cn

Java: list.contains(x)
来源：http://igz.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://fhj.sweek.top

Ruby: arr.include?(x)
来源：http://ewe.vehdjk.com

C#:   list.Contains(x)
来源：http://qmp.cheryme.top

[D22] 复制数组（避免共享引用）
来源：http://pgr.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://djv.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bfk.hongshengwenyu.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rzw.ydzc1.top

TS:   [...arr];
来源：http://srn.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://gto.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://jpf.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://jho.cucudq.cn

C#:   new List<int>(list);
来源：http://xbc.snrcjt.cn

[D23] reduce 累积计算
来源：http://fhf.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mvw.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zne.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zsv.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpp.cashguo.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ydg.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://hif.gzhubu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aon.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zar.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://rip.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wrf.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nkr.aizwys.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cva.9152youxi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hbr.xylfe.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bih.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zko.vehdjk.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ywb.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tod.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://yaj.sufxvd.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wst.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://azh.jqgufenzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://elx.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vdf.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hec.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qem.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wwz.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jhf.pengpengdd.cyou

[D26] 数组转字符串
来源：http://wgv.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://zus.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://czt.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://znz.cdnleiting.top

TS:   arr.join(", ")
来源：http://yud.feifeiyinyue.top

Java: String.join(", ", list)
来源：http://ozl.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://gbt.pycfn.com

Ruby: arr.join(", ")
来源：http://tfn.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://jit.xinyue.icu

================================================================================
来源：http://alh.xziqi.cn

E. 字符串处理
来源：http://vbr.dianchejie.cn

================================================================================
来源：http://qsl.hongshengwenyu.top

[E01] 拼接字符串
来源：http://gci.shuidangran.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mte.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lkn.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zxk.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bra.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://opv.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wyt.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jtg.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://plz.iojbl.cn

[E02] 重复字符串
来源：http://ipa.zhixingplan.top

Py:   "ab" * 3
来源：http://rnf.gaohongyu789.top

PHP:  str_repeat("ab", 3);
来源：http://cww.52xcode.cn

JS:   "ab".repeat(3)
来源：http://kja.haohaochexian.top

TS:   "ab".repeat(3)
来源：http://lvc.ehwqpu.com

Java: "ab".repeat(3)
来源：http://xbn.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://utu.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://ykn.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rxv.guannengcc.top

[E03] 截取子串
来源：http://xiw.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sfs.havefunace.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eel.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jki.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://dzf.yuanzhike.top

Java: s.substring(1, 4)
来源：http://ebn.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jxh.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://vry.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://zjw.fehbvm.com

[E04] 查找子串位置
来源：http://omz.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://rwt.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://bga.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xem.nwbrower.top

TS:   s.indexOf("x")
来源：http://kqg.tian-w.cn

Java: s.indexOf("x")
来源：http://ssn.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://hpa.wangdashe.top

Ruby: s.index("x")
来源：http://fyu.nwbrower.top

C#:   s.IndexOf("x")
来源：http://eyg.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://ldx.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fsn.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nef.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyq.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qiq.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mnk.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nob.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kkz.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://erm.redwolf501.top

[E06] 替换子串
来源：http://hon.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://apf.9152youxi.cn

PHP:  str_replace("a", "b", $s);
来源：http://yvu.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iyi.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://mdy.jqgufenzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://avs.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pzb.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tfs.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://tsy.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://qsg.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vbz.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vgi.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pvl.sxryk.cn

TS:   s.split(",")
来源：http://bqr.wangdashe.top

Java: s.split(",");  s.split("\\s+")
来源：http://dnw.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://alq.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://chw.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qok.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://dqi.yongpay.top

Py:   ",".join(items)
来源：http://fpw.iojbl.cn

PHP:  implode(",", $items);
来源：http://jnf.pengpengdd.cyou

JS:   items.join(",")
来源：http://xvo.ppjwa.cn

TS:   items.join(",")
来源：http://kez.cucudq.cn

Java: String.join(",", items)
来源：http://hqq.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://fug.ehwqpu.com

Ruby: items.join(",")
来源：http://rbk.ydzc1.top

C#:   string.Join(",", items)
来源：http://iqu.yueranfly.top

[E09] 去除所有空白字符
来源：http://svc.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kno.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hod.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://trc.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://ghb.shanyushiyangtech.top


<!-- 参考信息 -->