代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xrr.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pkh.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zgu.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qnh.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://yhp.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://uhp.svipenyu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xbx.iojbl.cn

[D02] 追加元素到末尾
来源：http://jbo.kuanghao11.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://orn.hammf.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wpl.daxiang520.top

JS:   arr.push(4);
来源：http://fft.guannengcc.top

TS:   arr.push(4);
来源：http://opz.0kj1m.cn

Java: list.add(4);
来源：http://qfe.jinqigufen.top

Go:   arr = append(arr, 4)
来源：http://dri.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://etp.guowangkeji.top

C#:   list.Add(4);
来源：http://wuv.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://wuc.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://och.ydzc1.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ltg.cashguo.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mdw.hfpthk.cn

TS:   arr.splice(0, 0, 0);
来源：http://vza.xylfe.cn

Java: list.add(0, 0);
来源：http://rrk.jyoumei.cn

Go:   arr = append([]int{0}, arr...)
来源：http://htg.haohaochexian.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mkw.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://zsu.zhaomingkeji.xyz

[D04] 删除元素
来源：http://xat.xylfe.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vnv.zhixingplan.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rfc.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dwa.zdqjudy.top

TS:   arr.splice(0, 1);
来源：http://iiy.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nma.c1oappe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rmi.zhijiandao.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://guf.ybcxt.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kat.zdbjq.cn

[D05] 访问与修改元素
来源：http://yoj.fanxiaobao.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://azf.sxryk.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kqv.zhongyouzk.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ovu.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://fjf.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://jkq.bjfxy.top

Go:   arr[0]; arr[0] = 9
来源：http://qqq.yuxming.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bvm.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xmp.guowangkeji.top

[D06] 数组长度
来源：http://nvk.andypj.xyz

Py:   len(arr)
来源：http://hvh.uphjek.com

PHP:  count($arr);
来源：http://luo.mhx1999.top

JS:   arr.length
来源：http://dio.wangdashe.top

TS:   arr.length
来源：http://ddu.0kj1m.cn

Java: list.size();
来源：http://amb.svipenyu.cn

Go:   len(arr)
来源：http://npo.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://wsj.shanyushiyangkeji.top

C#:   list.Count;
来源：http://epl.xinyue.icu

[D07] 切片 / 取子数组
来源：http://uaa.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fck.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xfd.xinyue.icu

JS:   arr.slice(1, 4);
来源：http://uox.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://wqi.xuetiantiany.cn

Java: list.subList(1, 4);
来源：http://cev.c1oappe.top

Go:   arr[1:4]
来源：http://ogc.pycfn.com

Ruby: arr[1, 3]
来源：http://joi.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://enc.316326.xyz

[D08] 合并两个数组
来源：http://wwn.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://pph.zhixingplan.top

PHP:  array_merge($a, $b);
来源：http://oub.hnqzz.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tjx.yongpay.top

TS:   [...a, ...b];
来源：http://emg.zhixingplan.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://red.nanxinkj.top

Go:   append(a, b...)
来源：http://bdf.chenlongwang.top

Ruby: a + b;  a.concat(b)
来源：http://dal.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://ihs.cdnleiting.top

[D09] 排序（升序）
来源：http://eri.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://mcc.meibo888.top

PHP:  sort($arr);
来源：http://yph.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mpj.yangfankeji.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://nry.daxiang520.top

Java: Collections.sort(list);  list.sort(null);
来源：http://eej.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qfz.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://zgh.hywenlv.cn

C#:   list.Sort();
来源：http://wdi.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bdv.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tsl.ivvv.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jhp.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eyp.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fdv.yueranfly.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lwd.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nvq.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fin.gaohongyu789.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qho.quarkkingdee.top

[D11] 反转数组
来源：http://hfw.shuidangran.top

Py:   arr[::-1];  arr.reverse()
来源：http://bhu.cheryme.top

PHP:  array_reverse($arr);
来源：http://hch.dashuyun.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hmo.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://uyv.yonumen.top

Java: Collections.reverse(list);
来源：http://lms.yongpay.top

Go:   slices.Reverse(arr)
来源：http://qeo.fehbvm.com

Ruby: arr.reverse
来源：http://pvf.andypj.xyz

C#:   list.Reverse();
来源：http://def.meibo888.top

[D12] 查找元素下标
来源：http://gvf.yonumen.top

Py:   arr.index(x);  x in arr
来源：http://hcx.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jnw.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uzy.cdnleiting.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykq.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bhu.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://bkc.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://dit.tanke756.top

C#:   list.IndexOf(x);
来源：http://ysz.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://idk.tarul.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://niz.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://agu.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://tvf.zdqjudy.top

TS:   arr.filter(x => x > 3)
来源：http://smj.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jye.ydjk.org.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tok.haohaochexian.top

Ruby: arr.select { |x| x > 3 }
来源：http://hfs.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fcm.c1oappe.top

[D14] 映射转换（每个元素变形）
来源：http://fju.jinyuanbaomall.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zmp.redwolf501.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uat.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://hsi.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://znx.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://elp.pengpengdd.cyou

Go:   // 手写循环
来源：http://omz.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://epk.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nsa.fanxiaobao.xyz

[D15] 去重
来源：http://kei.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kmy.xziqi.cn

PHP:  array_unique($arr);
来源：http://zzu.cheryme.top

JS:   [...new Set(arr)]
来源：http://civ.ybcxt.top

TS:   [...new Set(arr)]
来源：http://utp.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://idt.yanxiufei.cn

Go:   // 用 map[T]struct{} 手写
来源：http://naj.zhengqikj.top

Ruby: arr.uniq
来源：http://uea.chenjidiqi.icu

C#:   list.Distinct().ToList()
来源：http://rjw.bjfxy.top

[D16] 求和与平均值
来源：http://qqs.hesvh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cih.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://unm.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffb.jqgufenzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eje.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kxq.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://ydx.shangyingyoupin.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xft.fehbvm.com

C#:   list.Sum();  list.Average()
来源：http://ojj.0kj1m.cn

[D17] 最大值与最小值
来源：http://maw.iojbl.cn

Py:   max(arr);  min(arr)
来源：http://rkf.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://jif.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uat.redwolf501.top

TS:   Math.max(...arr);
来源：http://lic.zhijiandao.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rbx.xinyue.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tsg.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://zxn.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://csh.meibo888.top

[D18] 扁平化嵌套数组
来源：http://dnz.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lmq.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://mwe.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rng.hongshengwenyu.top

TS:   nested.flat();
来源：http://rpv.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://orq.hammf.cn

Go:   // 手写双层循环
来源：http://cvv.gaohongyu789.top

Ruby: nested.flatten
来源：http://pga.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://izx.52xcode.cn

[D19] 按字段分组
来源：http://dng.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sqb.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ojm.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qeq.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tfj.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://krm.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://rok.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hfi.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jzs.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://yez.nanxuanxn.top

Py:   Counter(arr)
来源：http://fwc.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://cbg.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvw.fengsongda.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cql.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://esa.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://aag.yj20258.top

Ruby: arr.tally
来源：http://zal.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tom.vehdjk.com

[D21] 判断是否包含某元素
来源：http://ygy.haohaochexian.top

Py:   x in arr
来源：http://edt.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://phd.vqdsnc.cn

JS:   arr.includes(x)
来源：http://oxb.zdqjudy.top

TS:   arr.includes(x)
来源：http://yzx.sweek.top

Java: list.contains(x)
来源：http://wgo.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://xhh.haohaochexian.top

Ruby: arr.include?(x)
来源：http://zgt.yfazqb.com

C#:   list.Contains(x)
来源：http://geh.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://fln.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pmr.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://krr.jqgufenzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://osm.vehdjk.com

TS:   [...arr];
来源：http://abu.zdbjq.cn

Java: new ArrayList<>(list);
来源：http://rhd.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ufm.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://pah.sufxvd.cn

C#:   new List<int>(list);
来源：http://yfo.jianghu66.top

[D23] reduce 累积计算
来源：http://wtr.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ndx.redwolf501.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://idb.fktsv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lrx.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krr.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ugo.jinqigufen.top

Go:   // 手写循环
来源：http://blc.cqqwz.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rou.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://prc.hammf.cn

[D24] 字典 / Map 基本操作
来源：http://njv.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pfg.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://htw.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tku.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lbo.zhijiandao.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jum.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://grv.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qqp.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gim.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://mon.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://has.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ncg.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lnj.ehwqpu.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nyx.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rgt.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qus.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rgx.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xme.pycfn.com

[D26] 数组转字符串
来源：http://bcj.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://rhh.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://sue.havefunace.top

JS:   arr.join(", ")
来源：http://vzc.cucudq.cn

TS:   arr.join(", ")
来源：http://wdt.jyoumei.cn

Java: String.join(", ", list)
来源：http://iid.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://crf.zhengqikj.top

Ruby: arr.join(", ")
来源：http://jmb.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://jto.andypj.xyz

================================================================================
来源：http://psg.jqgfzy.top

E. 字符串处理
来源：http://hnk.shanyushiyangtech.top

================================================================================
来源：http://uvo.jianghu66.top

[E01] 拼接字符串
来源：http://kfn.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dif.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nnd.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxe.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vle.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rrs.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wkv.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vra.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://duw.ydjk.org.cn

[E02] 重复字符串
来源：http://uyb.aizwys.cn

Py:   "ab" * 3
来源：http://ecz.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://lch.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://trs.316326.xyz

TS:   "ab".repeat(3)
来源：http://rmd.chenzaomai.com

Java: "ab".repeat(3)
来源：http://jeo.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://ual.daria6918.cn

Ruby: "ab" * 3
来源：http://tfs.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dug.shanyushiyangkeji.top

[E03] 截取子串
来源：http://ram.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zyw.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lxs.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nsa.xziqi.cn

TS:   s.slice(1, 4)
来源：http://ajn.ehwqpu.com

Java: s.substring(1, 4)
来源：http://apu.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ogl.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://wxw.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://bol.vehdjk.com

[E04] 查找子串位置
来源：http://mmg.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://mhh.hesvh.cn

PHP:  strpos($s, "x");
来源：http://vai.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zfw.andypj.xyz

TS:   s.indexOf("x")
来源：http://nnw.dianchejie.cn

Java: s.indexOf("x")
来源：http://cek.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://gan.zycfv.cn

Ruby: s.index("x")
来源：http://qke.gotoacloud.top

C#:   s.IndexOf("x")
来源：http://xjs.chenjidiqi.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://zuh.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tut.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sgh.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dsk.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lbj.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ssk.316326.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cxi.yonumen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fty.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pfb.yueranfly.top

[E06] 替换子串
来源：http://paa.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mti.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://jzv.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://urk.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://zen.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mia.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ele.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ylw.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://pgq.yongpay.top

[E07] 按分隔符拆分
来源：http://zix.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xba.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gse.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ggo.vqdsnc.cn

TS:   s.split(",")
来源：http://ikb.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://hdm.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dzv.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://lyx.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvx.hcnkem.com

[E08] 数组按分隔符合并
来源：http://zny.yongpay.top

Py:   ",".join(items)
来源：http://cye.kuanghao11.cn


<!-- 参考信息 -->