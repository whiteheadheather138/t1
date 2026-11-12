代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://obm.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://yaq.jinqigfzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://jsa.wangshuangyany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oyc.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://jwf.gogol.net.cn

Ruby: arr = [1, 2, 3]
来源：http://lzv.yonumen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zrj.svipenyu.cn

[D02] 追加元素到末尾
来源：http://mld.cqqwz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pai.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bmr.jinqigufen.top

JS:   arr.push(4);
来源：http://jhr.zycfv.cn

TS:   arr.push(4);
来源：http://ayj.tanke756.top

Java: list.add(4);
来源：http://cfi.c1oappe.top

Go:   arr = append(arr, 4)
来源：http://nmf.shzxlz.cn

Ruby: arr << 4; arr.push(5)
来源：http://gpg.yvedp.cn

C#:   list.Add(4);
来源：http://lea.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://kln.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://prd.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hmh.zhaomingkeji.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://idn.hongshengwenyu.top

TS:   arr.splice(0, 0, 0);
来源：http://img.tianlin.xyz

Java: list.add(0, 0);
来源：http://vrj.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://pbd.smart0.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wmq.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://rkx.gotoacloud.top

[D04] 删除元素
来源：http://fbl.haohaochexian.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mwt.zdbjq.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tju.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nqx.bjfxy.top

TS:   arr.splice(0, 1);
来源：http://cbd.yvedp.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tqu.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ojm.pycfn.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rqi.ydjk.org.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jjh.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://fjc.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eyr.dianchejie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baj.redwolf501.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ewk.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://oan.sweek.top

Java: list.get(0); list.set(0, 9);
来源：http://opq.fanxiaobao.xyz

Go:   arr[0]; arr[0] = 9
来源：http://gmu.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ofk.daria6918.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kfi.ppjwa.cn

[D06] 数组长度
来源：http://oyk.yj20258888.top

Py:   len(arr)
来源：http://avt.yuanzhike.top

PHP:  count($arr);
来源：http://wpn.nanxuanxn.top

JS:   arr.length
来源：http://oij.hcnkem.com

TS:   arr.length
来源：http://nlh.vehdjk.com

Java: list.size();
来源：http://til.jiagoushi.top

Go:   len(arr)
来源：http://wea.vehdjk.com

Ruby: arr.length; arr.size
来源：http://xrg.vehdjk.com

C#:   list.Count;
来源：http://moc.yanxiufei.cn

[D07] 切片 / 取子数组
来源：http://awb.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://adh.jinghuilouyu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yad.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://gdw.yongpay.top

TS:   arr.slice(1, 4);
来源：http://tbp.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://ssw.zhaomingkeji.xyz

Go:   arr[1:4]
来源：http://kto.xylfe.cn

Ruby: arr[1, 3]
来源：http://efb.gogol.net.cn

C#:   list.GetRange(1, 3);
来源：http://qrl.0kj1m.cn

[D08] 合并两个数组
来源：http://pts.yvedp.cn

Py:   a + b;  a.extend(b)
来源：http://nox.jyoumei.cn

PHP:  array_merge($a, $b);
来源：http://anx.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://hij.bjfxy.top

TS:   [...a, ...b];
来源：http://kre.jinyuanbaomall.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ulr.316326.xyz

Go:   append(a, b...)
来源：http://cbg.tanke756.top

Ruby: a + b;  a.concat(b)
来源：http://ayw.hesvh.cn

C#:   a.Concat(b).ToList()
来源：http://wdc.zhiwuduotai.top

[D09] 排序（升序）
来源：http://lij.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://ihr.yfazqb.com

PHP:  sort($arr);
来源：http://ogq.shanyushiyangtech.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://boo.sweek.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cmv.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://dbr.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zjw.c1oappe.top

Ruby: arr.sort
来源：http://vef.yfazqb.com

C#:   list.Sort();
来源：http://sbf.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://mvn.yj20258.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qkb.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsr.zdqjudy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qyy.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://opm.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kff.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kdo.yvedp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kdn.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mvh.ehwqpu.com

[D11] 反转数组
来源：http://rru.yfazqb.com

Py:   arr[::-1];  arr.reverse()
来源：http://hkt.shuidangran.top

PHP:  array_reverse($arr);
来源：http://mrd.jqgfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tyc.fehbvm.com

TS:   [...arr].reverse();
来源：http://nzp.hesvh.cn

Java: Collections.reverse(list);
来源：http://sqw.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://nao.yj20258.top

Ruby: arr.reverse
来源：http://xme.ctjpmb.com

C#:   list.Reverse();
来源：http://itm.9152youxi.cn

[D12] 查找元素下标
来源：http://rsi.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://zqh.bbcook.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uxx.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cep.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wyf.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bmm.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://kbk.316326.xyz

Ruby: arr.index(x)
来源：http://ebs.yongpay.top

C#:   list.IndexOf(x);
来源：http://jfj.jianghu66.top

[D13] 过滤（保留满足条件的）
来源：http://vcl.cqqwz.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lqw.jinghuilouyu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zdc.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://ubj.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://kqj.feifeiyinyue.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wwk.shzxlz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rkq.jinqigfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://zdc.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zat.wangshuangyany.cn

[D14] 映射转换（每个元素变形）
来源：http://oze.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cam.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pjj.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://pwm.yongpay.top

TS:   arr.map(x => x * 2)
来源：http://xga.yongpay.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gma.yvedp.cn

Go:   // 手写循环
来源：http://hsv.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wvw.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://eud.guowangkeji.top

[D15] 去重
来源：http://ivh.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rky.sxryk.cn

PHP:  array_unique($arr);
来源：http://rev.tarul.cn

JS:   [...new Set(arr)]
来源：http://tbr.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://yop.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mzn.ydjk.org.cn

Go:   // 用 map[T]struct{} 手写
来源：http://blm.hnqzz.top

Ruby: arr.uniq
来源：http://gbq.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://pph.gotoacloud.top

[D16] 求和与平均值
来源：http://nub.vehdjk.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yas.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zcl.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ptj.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ruw.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dkf.smart0.xyz

Go:   // 手写循环累加
来源：http://rnd.cqqwz.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://utu.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://qhl.ppjwa.cn

[D17] 最大值与最小值
来源：http://nev.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://nlu.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://sow.feifeiyinyue.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://faa.tian-w.cn

TS:   Math.max(...arr);
来源：http://ieo.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bsv.daria6918.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mga.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://fpc.sysykeji.top

C#:   list.Max();  list.Min()
来源：http://hnx.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://cxq.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mmk.jinghuilouyu.cn

PHP:  array_merge(...$nested);
来源：http://ctv.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://grs.c1oappe.top

TS:   nested.flat();
来源：http://max.nanxuanxn.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://adp.xylfe.cn

Go:   // 手写双层循环
来源：http://oha.cashguo.top

Ruby: nested.flatten
来源：http://bft.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gfp.jinqigufen.top

[D19] 按字段分组
来源：http://mgk.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qpg.iojbl.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rxg.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gvq.gaohongyu789.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://uwe.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fxh.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://ncz.daria6918.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sbt.snrcjt.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hds.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://azd.yonumen.top

Py:   Counter(arr)
来源：http://njt.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://qdq.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvj.zhongyouzk.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xzl.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ecm.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://kha.ivvv.top

Ruby: arr.tally
来源：http://aka.daxiang520.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dto.hcnkem.com

[D21] 判断是否包含某元素
来源：http://sxn.wangdashe.top

Py:   x in arr
来源：http://niu.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://fat.yuanzhike.top

JS:   arr.includes(x)
来源：http://kfy.fengsongda.top

TS:   arr.includes(x)
来源：http://taf.xziqi.cn

Java: list.contains(x)
来源：http://tdk.guannengcc.top

Go:   slices.Contains(arr, x)
来源：http://nyq.shzxlz.cn

Ruby: arr.include?(x)
来源：http://vfn.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://yed.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://qcq.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mxy.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bol.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uye.yongpay.top

TS:   [...arr];
来源：http://vpi.sysykeji.top

Java: new ArrayList<>(list);
来源：http://hym.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ohg.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://rgj.hysaishi.cn

C#:   new List<int>(list);
来源：http://nsx.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://ptp.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://soi.jiagoushi.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rpi.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyc.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lhf.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fwl.cucudq.cn

Go:   // 手写循环
来源：http://zme.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ozp.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lcc.shuidangran.top

[D24] 字典 / Map 基本操作
来源：http://yev.yuanzhike.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yws.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oqk.tianlin.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jpk.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lmq.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jjp.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xej.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fok.xylfe.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pqk.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://tpi.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lnf.hysaishi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://auw.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fko.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wce.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lmb.zdqjudy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qmr.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ean.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dgy.yj20258888.top

[D26] 数组转字符串
来源：http://dnb.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://ujw.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://hvc.redwolf501.top

JS:   arr.join(", ")
来源：http://tsq.smart0.xyz

TS:   arr.join(", ")
来源：http://mzm.ctjpmb.com

Java: String.join(", ", list)
来源：http://ltx.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://xnw.daria6918.cn

Ruby: arr.join(", ")
来源：http://hym.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://ihy.shuidangran.top

================================================================================
来源：http://grx.chenjidiqi.icu

E. 字符串处理
来源：http://iec.gzhubu.top

================================================================================
来源：http://xbr.zhiwuduotai.top

[E01] 拼接字符串
来源：http://tnb.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ltf.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oiv.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://psp.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fcr.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kwo.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nvw.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sbb.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cgd.uphjek.com

[E02] 重复字符串
来源：http://bvz.quarkkingdee.top

Py:   "ab" * 3
来源：http://mtr.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://aga.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://qof.guannengcc.top

TS:   "ab".repeat(3)
来源：http://gaw.jqgfzy.top

Java: "ab".repeat(3)
来源：http://uqi.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://abg.yj20258888.top

Ruby: "ab" * 3
来源：http://ski.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xjo.hywenlv.cn

[E03] 截取子串
来源：http://byl.svipenyu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yrl.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vzx.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sjj.bjfxy.top

TS:   s.slice(1, 4)
来源：http://eyf.hysaishi.cn

Java: s.substring(1, 4)
来源：http://xfn.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qfe.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ndl.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://qjs.wangshuangyany.cn

[E04] 查找子串位置
来源：http://kwb.nanxinkj.top

Py:   s.find("x");  s.index("x")
来源：http://nqp.gzhubu.top

PHP:  strpos($s, "x");
来源：http://lhh.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yvu.iojbl.cn

TS:   s.indexOf("x")
来源：http://hso.ydzc1.top

Java: s.indexOf("x")
来源：http://dzq.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://wwt.shangyingyoupin.top

Ruby: s.index("x")
来源：http://uzl.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://ptn.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ffc.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cbm.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nru.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nai.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tym.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ila.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xvx.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nwh.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://isy.yfazqb.com

[E06] 替换子串
来源：http://yal.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xuw.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://kcq.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jxz.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://tcl.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xsp.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ewq.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wst.sweek.top

C#:   s.Replace("a", "b")
来源：http://may.xingfuxueyuan.xyz

[E07] 按分隔符拆分
来源：http://ilw.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yku.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wwp.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qlj.zdbjq.cn

TS:   s.split(",")
来源：http://emc.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://bkn.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bjp.zdbjq.cn

Ruby: s.split(",");  s.split
来源：http://wsc.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tlw.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://jmv.316326.xyz

Py:   ",".join(items)
来源：http://qdk.hcnkem.com


<!-- 参考信息 -->