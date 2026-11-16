代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://gmb.xinyue.icu

Ruby: # 无重载：靠动态参数
来源：http://aow.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://chb.ehwqpu.com

================================================================================
来源：http://wdm.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://tsw.cucudq.cn

================================================================================
来源：http://fcx.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://wxg.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ugq.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kkt.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bfx.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sju.tarul.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mfs.hywenlv.cn

Go:   arr := []int{1, 2, 3}
来源：http://tzx.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://foz.gotoacloud.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://qjb.ctjpmb.com

[D02] 追加元素到末尾
来源：http://dbx.zhongyouzk.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ajh.yfazqb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fkq.hnqzz.top

JS:   arr.push(4);
来源：http://fhx.ppjwa.cn

TS:   arr.push(4);
来源：http://kjz.bjfxy.top

Java: list.add(4);
来源：http://irk.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://qyo.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://wym.dianchejie.cn

C#:   list.Add(4);
来源：http://tbv.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://otw.mhx1999.top

Py:   arr.insert(0, 0)
来源：http://ycx.hywenlv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tcz.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pte.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://cuf.daxiang520.top

Java: list.add(0, 0);
来源：http://bov.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://azu.daxiang520.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mok.tian-w.cn

C#:   list.Insert(0, 0);
来源：http://dpd.hammf.cn

[D04] 删除元素
来源：http://kaw.jinqigfzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ibo.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://avb.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rou.havefunace.top

TS:   arr.splice(0, 1);
来源：http://yna.hysaishi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://evp.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jmv.jinqigfzy.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ujh.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://twq.pycfn.com

[D05] 访问与修改元素
来源：http://fne.nanxuanxn.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://glv.jianghu66.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lol.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rlu.uphjek.com

TS:   arr[0]; arr.at(-1);
来源：http://hxd.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://gwa.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://ifd.0kj1m.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zdi.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qah.zhongyouzk.top

[D06] 数组长度
来源：http://mxf.jinqigfzy.top

Py:   len(arr)
来源：http://mkz.yuanzhike.top

PHP:  count($arr);
来源：http://hcw.ctjpmb.com

JS:   arr.length
来源：http://gea.gotoacloud.top

TS:   arr.length
来源：http://evc.hammf.cn

Java: list.size();
来源：http://fgy.fehbvm.com

Go:   len(arr)
来源：http://sde.tian-w.cn

Ruby: arr.length; arr.size
来源：http://nrh.epnwcf.com

C#:   list.Count;
来源：http://mmy.cdnleiting.top

[D07] 切片 / 取子数组
来源：http://gbm.hesvh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fyl.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kog.zhijiandao.cn

JS:   arr.slice(1, 4);
来源：http://tvn.yj20258.top

TS:   arr.slice(1, 4);
来源：http://omj.zhoulong.xyz

Java: list.subList(1, 4);
来源：http://ckt.52xcode.cn

Go:   arr[1:4]
来源：http://iah.yuanzhike.top

Ruby: arr[1, 3]
来源：http://ueo.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://myv.0kj1m.cn

[D08] 合并两个数组
来源：http://ybj.yuanzhike.top

Py:   a + b;  a.extend(b)
来源：http://vgg.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://yxu.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://klp.meibo888.top

TS:   [...a, ...b];
来源：http://rgj.fehbvm.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dyv.jinqigufen.top

Go:   append(a, b...)
来源：http://ekn.sufxvd.cn

Ruby: a + b;  a.concat(b)
来源：http://rgy.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://oyu.yangfankeji.com

[D09] 排序（升序）
来源：http://ser.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://wgo.mhx1999.top

PHP:  sort($arr);
来源：http://pub.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nyu.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gfz.dianchejie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://huw.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dms.yanxiufei.cn

Ruby: arr.sort
来源：http://mzk.daxiang520.top

C#:   list.Sort();
来源：http://gjp.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://ojl.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iug.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oya.c1oappe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jnz.hysaishi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nbp.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wdc.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yfp.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xhj.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ufv.vqdsnc.cn

[D11] 反转数组
来源：http://muw.ivvv.top

Py:   arr[::-1];  arr.reverse()
来源：http://ahb.sxryk.cn

PHP:  array_reverse($arr);
来源：http://aan.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ikr.redwolf501.top

TS:   [...arr].reverse();
来源：http://loq.zdqjudy.top

Java: Collections.reverse(list);
来源：http://ddv.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://cre.cucudq.cn

Ruby: arr.reverse
来源：http://eac.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://ykm.zhixingplan.top

[D12] 查找元素下标
来源：http://jdr.316326.xyz

Py:   arr.index(x);  x in arr
来源：http://ydm.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qom.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jbp.hfpthk.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zak.quarkkingdee.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qiq.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://zfa.tarul.cn

Ruby: arr.index(x)
来源：http://weg.yonumen.top

C#:   list.IndexOf(x);
来源：http://ugg.ydzc1.top

[D13] 过滤（保留满足条件的）
来源：http://eur.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyy.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qem.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://lqp.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://kel.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xdl.ybcxt.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pvc.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://afo.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://dfm.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://lsk.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ypn.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xrl.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://uuo.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://ajs.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://brb.shanyushiyangtech.top

Go:   // 手写循环
来源：http://wss.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://krd.tanke756.top

C#:   list.Select(x => x * 2).ToList()
来源：http://zcy.zhijiandao.cn

[D15] 去重
来源：http://njp.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://axl.yongpay.top

PHP:  array_unique($arr);
来源：http://qdn.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://aul.uphjek.com

TS:   [...new Set(arr)]
来源：http://wms.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://all.sufxvd.cn

Go:   // 用 map[T]struct{} 手写
来源：http://byo.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://ewf.zhoulong.xyz

C#:   list.Distinct().ToList()
来源：http://tjl.gotoacloud.top

[D16] 求和与平均值
来源：http://ikp.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://asu.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dfp.cdnleiting.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zxp.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pac.sxryk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dfk.yueranfly.top

Go:   // 手写循环累加
来源：http://afj.hammf.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nig.hywenlv.cn

C#:   list.Sum();  list.Average()
来源：http://mdm.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://pqn.hesvh.cn

Py:   max(arr);  min(arr)
来源：http://qzd.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://xff.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hxc.sxryk.cn

TS:   Math.max(...arr);
来源：http://zib.zhengqikj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fxx.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qsw.hnxiangtu.top

Ruby: arr.max;  arr.min
来源：http://kbm.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://wbl.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://piz.hnxiangtu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://has.jinqigufen.top

PHP:  array_merge(...$nested);
来源：http://ked.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gsu.cqqwz.cn

TS:   nested.flat();
来源：http://awb.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ovo.cashguo.top

Go:   // 手写双层循环
来源：http://xxb.cashguo.top

Ruby: nested.flatten
来源：http://dre.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ftu.sxryk.cn

[D19] 按字段分组
来源：http://qkb.jqgufenzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bxs.nwbrower.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oln.ctjpmb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lck.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ijb.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tgb.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://uqm.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wus.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dut.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://gor.sweek.top

Py:   Counter(arr)
来源：http://sjo.svipenyu.cn

PHP:  array_count_values($arr);
来源：http://fok.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://arq.feifeiyinyue.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tjp.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xsu.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://mbg.ywan-chungtsiang.top

Ruby: arr.tally
来源：http://wzp.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://orp.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://zch.nwbrower.top

Py:   x in arr
来源：http://dpu.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://sms.hysaishi.cn

JS:   arr.includes(x)
来源：http://mre.wangdashe.top

TS:   arr.includes(x)
来源：http://bbh.yueranfly.top

Java: list.contains(x)
来源：http://kam.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://rxn.fktsv.cn

Ruby: arr.include?(x)
来源：http://cvd.vqdsnc.cn

C#:   list.Contains(x)
来源：http://mgs.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://sof.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lul.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkz.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://avx.xuanzx.com

TS:   [...arr];
来源：http://efs.tian-w.cn

Java: new ArrayList<>(list);
来源：http://jgk.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://upd.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ofe.chenlongwang.top

C#:   new List<int>(list);
来源：http://wmr.kuanghao11.cn

[D23] reduce 累积计算
来源：http://wgx.chenlongwang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kko.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qan.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://idn.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mrd.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fqv.zhixingplan.top

Go:   // 手写循环
来源：http://kya.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mqi.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tqa.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://fah.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tuk.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zgg.zdbjq.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qxn.andypj.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xfi.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uvq.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yia.yj20258.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hgw.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dwn.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://ggm.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dpn.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://huh.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jnh.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vdc.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vyl.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fcn.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ldr.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bpu.zhengqikj.top

[D26] 数组转字符串
来源：http://ktz.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://yal.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://bzv.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://vzj.chenlongwang.top

TS:   arr.join(", ")
来源：http://gil.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://pyu.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://sej.zdbjq.cn

Ruby: arr.join(", ")
来源：http://kmm.yuxming.cn

C#:   string.Join(", ", list)
来源：http://xjq.tianlin.xyz

================================================================================
来源：http://hlo.yueranfly.top

E. 字符串处理
来源：http://ucb.vqdsnc.cn

================================================================================
来源：http://cdy.pengpengdd.cyou

[E01] 拼接字符串
来源：http://rwl.daria6918.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jgd.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ayj.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vhl.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ide.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mal.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mtr.iojbl.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iwz.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mrm.jlsjyb.cn

[E02] 重复字符串
来源：http://zfk.gaohongyu789.top

Py:   "ab" * 3
来源：http://uuq.jqgufenzy.top

PHP:  str_repeat("ab", 3);
来源：http://bda.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://ujy.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://adf.gotoacloud.top

Java: "ab".repeat(3)
来源：http://iii.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://xhb.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://clq.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mmw.zhongyouzk.top

[E03] 截取子串
来源：http://qqx.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ibd.daria6918.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fkd.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lrg.xylfe.cn

TS:   s.slice(1, 4)
来源：http://ofo.tian-w.cn

Java: s.substring(1, 4)
来源：http://szh.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hwv.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://wje.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://jok.daria6918.cn

[E04] 查找子串位置
来源：http://sed.guannengcc.top

Py:   s.find("x");  s.index("x")
来源：http://ezu.cashguo.top

PHP:  strpos($s, "x");
来源：http://mkd.xylfe.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wzk.316326.xyz

TS:   s.indexOf("x")
来源：http://oar.xylfe.cn

Java: s.indexOf("x")
来源：http://orq.cashguo.top

Go:   strings.Index(s, "x")
来源：http://fsa.zycfv.cn

Ruby: s.index("x")
来源：http://hkd.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://sci.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://opv.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rqo.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://una.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rjf.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wgw.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ghm.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fmc.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ugn.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uyk.iojbl.cn

[E06] 替换子串
来源：http://ynk.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hna.nanxuanxn.top

PHP:  str_replace("a", "b", $s);
来源：http://bsz.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vyr.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://oem.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://afj.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uur.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xtg.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://uui.tarul.cn

[E07] 按分隔符拆分
来源：http://yna.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pkm.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://atn.wangdashe.top


<!-- 参考信息 -->