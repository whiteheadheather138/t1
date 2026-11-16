代发 wailian999

PHP:  // 无重载
来源：http://fkg.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fdd.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://fwl.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://eiy.snrcjt.cn

Go:   // 无重载：用不同函数名
来源：http://oph.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://lmz.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lgk.fehbvm.com

================================================================================
来源：http://bpz.316326.xyz

D. 数组 / 列表 / 集合
来源：http://hhj.gogol.net.cn

================================================================================
来源：http://ivw.daria6918.cn

[D01] 创建数组 / 列表
来源：http://ysn.yuxming.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wty.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pmu.birdmap.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dst.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://kik.svipenyu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wmx.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://dpi.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://gku.pycfn.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gqy.xuetiantiany.cn

[D02] 追加元素到末尾
来源：http://hws.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rww.ehwqpu.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wmc.yanxiufei.cn

JS:   arr.push(4);
来源：http://tuk.hfpthk.cn

TS:   arr.push(4);
来源：http://cvt.vqdsnc.cn

Java: list.add(4);
来源：http://kze.redwolf501.top

Go:   arr = append(arr, 4)
来源：http://kvx.pengpengdd.cyou

Ruby: arr << 4; arr.push(5)
来源：http://toe.mhx1999.top

C#:   list.Add(4);
来源：http://tph.yueranfly.top

[D03] 在指定位置插入元素
来源：http://bbl.fehbvm.com

Py:   arr.insert(0, 0)
来源：http://axc.jyoumei.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dey.snrcjt.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://liu.yueranfly.top

TS:   arr.splice(0, 0, 0);
来源：http://uwt.jqgfzy.top

Java: list.add(0, 0);
来源：http://pin.52xcode.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ntu.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bag.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://zmt.xingfuxueyuan.xyz

[D04] 删除元素
来源：http://tmm.feifeiyinyue.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ymr.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cxr.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hdj.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://evl.hcnkem.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nco.jlsjyb.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xiz.yj20258888.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://npb.hnqzz.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pxb.zhijiandao.cn

[D05] 访问与修改元素
来源：http://dyq.yuxming.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jgb.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ejs.tanke756.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tzb.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://jzm.gotoacloud.top

Java: list.get(0); list.set(0, 9);
来源：http://ubx.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://six.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://lns.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ooq.xuetiantiany.cn

[D06] 数组长度
来源：http://zlh.jiagoushi.top

Py:   len(arr)
来源：http://dua.zdbjq.cn

PHP:  count($arr);
来源：http://pwh.ywan-chungtsiang.top

JS:   arr.length
来源：http://moi.jiagoushi.top

TS:   arr.length
来源：http://ohq.feifeiyinyue.top

Java: list.size();
来源：http://txl.ivvv.top

Go:   len(arr)
来源：http://pgn.zycfv.cn

Ruby: arr.length; arr.size
来源：http://xzy.gaohongyu789.top

C#:   list.Count;
来源：http://iyw.zycfv.cn

[D07] 切片 / 取子数组
来源：http://aoj.9152youxi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dre.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://dbx.zhiwuduotai.top

JS:   arr.slice(1, 4);
来源：http://cod.yj20258.top

TS:   arr.slice(1, 4);
来源：http://qmu.c1oappe.top

Java: list.subList(1, 4);
来源：http://ezy.nwbrower.top

Go:   arr[1:4]
来源：http://msp.cucudq.cn

Ruby: arr[1, 3]
来源：http://zbf.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://jii.yj202588.top

[D08] 合并两个数组
来源：http://aav.quarkkingdee.top

Py:   a + b;  a.extend(b)
来源：http://bew.meibo888.top

PHP:  array_merge($a, $b);
来源：http://hmx.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bey.yonumen.top

TS:   [...a, ...b];
来源：http://fqu.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ifh.daxiang520.top

Go:   append(a, b...)
来源：http://wyl.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://inr.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://ivy.52xcode.cn

[D09] 排序（升序）
来源：http://ptc.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://ihe.tianlin.xyz

PHP:  sort($arr);
来源：http://fhh.xziqi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xpu.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vjf.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://coe.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qdd.jinqigufen.top

Ruby: arr.sort
来源：http://duk.hfpthk.cn

C#:   list.Sort();
来源：http://nvb.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ehy.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fnz.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ieo.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wqr.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zpw.zhijiandao.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iyr.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zjp.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cyy.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bpl.jlsjyb.cn

[D11] 反转数组
来源：http://cei.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wjh.52xcode.cn

PHP:  array_reverse($arr);
来源：http://bvm.havefunace.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uax.hammf.cn

TS:   [...arr].reverse();
来源：http://cuk.tian-w.cn

Java: Collections.reverse(list);
来源：http://lia.feifeiyinyue.top

Go:   slices.Reverse(arr)
来源：http://umz.sjlbkw.cn

Ruby: arr.reverse
来源：http://rid.zhiwuduotai.top

C#:   list.Reverse();
来源：http://ulh.zhiwuduotai.top

[D12] 查找元素下标
来源：http://mfr.sweek.top

Py:   arr.index(x);  x in arr
来源：http://poj.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qyc.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://srr.sweek.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bil.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://omx.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://pdk.yvedp.cn

Ruby: arr.index(x)
来源：http://qho.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://ttn.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://ymk.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yld.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://szd.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://ncs.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://coj.tanke756.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://myh.fengsongda.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ixz.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kws.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dzc.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://agi.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fgi.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gvi.cheryme.top

JS:   arr.map(x => x * 2)
来源：http://ybk.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://yha.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cxl.vqdsnc.cn

Go:   // 手写循环
来源：http://lst.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://drh.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://amg.shanyushiyangtech.top

[D15] 去重
来源：http://wfi.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://afb.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://axz.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://mbl.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://edk.dashuyun.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zqk.meibo888.top

Go:   // 用 map[T]struct{} 手写
来源：http://tur.xuetiantiany.cn

Ruby: arr.uniq
来源：http://xke.jinqigufen.top

C#:   list.Distinct().ToList()
来源：http://dtu.shzxlz.cn

[D16] 求和与平均值
来源：http://mbz.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bcs.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yln.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ktv.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://laj.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://axx.cheryme.top

Go:   // 手写循环累加
来源：http://kom.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ahu.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://cfr.zhixingplan.top

[D17] 最大值与最小值
来源：http://fqx.xziqi.cn

Py:   max(arr);  min(arr)
来源：http://whj.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://fxd.yj20258.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ame.tian-w.cn

TS:   Math.max(...arr);
来源：http://mus.sysykeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ddl.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bot.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://vii.tanke756.top

C#:   list.Max();  list.Min()
来源：http://rqr.daxiang520.top

[D18] 扁平化嵌套数组
来源：http://qrg.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kia.smart0.xyz

PHP:  array_merge(...$nested);
来源：http://fdm.hnqzz.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dbl.ppjwa.cn

TS:   nested.flat();
来源：http://foq.52xcode.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://awj.fengsongda.top

Go:   // 手写双层循环
来源：http://wyl.dashuyun.cn

Ruby: nested.flatten
来源：http://mbs.zhengqikj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iej.gotoacloud.top

[D19] 按字段分组
来源：http://kqg.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dsd.fktsv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dvk.wangshuangyany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tjg.nanxuanxn.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gsw.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qli.cashguo.top

Go:   // 手写 map[string][]T
来源：http://pdv.gogol.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jtp.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uqq.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://rwr.xuetiantiany.cn

Py:   Counter(arr)
来源：http://los.hammf.cn

PHP:  array_count_values($arr);
来源：http://xqn.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lzb.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kuo.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fvm.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://qao.zhoulong.xyz

Ruby: arr.tally
来源：http://nxj.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aqo.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://kuw.andypj.xyz

Py:   x in arr
来源：http://gtr.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://ryq.fktsv.cn

JS:   arr.includes(x)
来源：http://ueg.yonumen.top

TS:   arr.includes(x)
来源：http://ujq.yueranfly.top

Java: list.contains(x)
来源：http://srj.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://mbx.bbcook.cn

Ruby: arr.include?(x)
来源：http://eas.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://ysg.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://cfu.daria6918.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nqv.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xpo.sweek.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wpn.sweek.top

TS:   [...arr];
来源：http://tsv.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://bhr.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://gbr.jqgfzy.top

Ruby: arr.dup;  arr.clone
来源：http://lqm.sufxvd.cn

C#:   new List<int>(list);
来源：http://lfp.jqgufenzy.top

[D23] reduce 累积计算
来源：http://lrq.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://igx.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hfr.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysb.hcnkem.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdr.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgv.ydjk.org.cn

Go:   // 手写循环
来源：http://wba.feifeiyinyue.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lsk.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cqj.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://zit.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lvh.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hvf.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ajy.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ana.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hrf.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yeg.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jyy.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ymf.yj20258.top

[D25] Set 集合去重与交并差
来源：http://hig.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eis.smart0.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gku.uphjek.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cqe.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xta.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gty.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jwr.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uro.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pqp.fktsv.cn

[D26] 数组转字符串
来源：http://bbt.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://rls.xingfuxueyuan.xyz

PHP:  implode(", ", $arr);
来源：http://hxm.hcnkem.com

JS:   arr.join(", ")
来源：http://znp.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://hdj.zhongyouzk.top

Java: String.join(", ", list)
来源：http://xmp.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://shq.cheryme.top

Ruby: arr.join(", ")
来源：http://kdn.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://ryf.fzhhl.top

================================================================================
来源：http://lpo.yfazqb.com

E. 字符串处理
来源：http://eyc.xingfuxueyuan.xyz

================================================================================
来源：http://cku.jinqigfzy.top

[E01] 拼接字符串
来源：http://scd.cheryme.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ktt.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wes.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tkr.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bwf.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lox.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kpz.wangdashe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://plj.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ewp.yuanzhike.top

[E02] 重复字符串
来源：http://mfv.jyoumei.cn

Py:   "ab" * 3
来源：http://esu.daria6918.cn

PHP:  str_repeat("ab", 3);
来源：http://hxh.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://ocw.yvedp.cn

TS:   "ab".repeat(3)
来源：http://xqo.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://qby.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://izx.quarkkingdee.top

Ruby: "ab" * 3
来源：http://aow.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ssf.jiagoushi.top

[E03] 截取子串
来源：http://blt.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://imt.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uyw.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zok.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://sdo.ppjwa.cn

Java: s.substring(1, 4)
来源：http://hfl.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nae.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://abe.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://blo.hysaishi.cn

[E04] 查找子串位置
来源：http://fau.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://mnk.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://rrd.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rdc.svipenyu.cn

TS:   s.indexOf("x")
来源：http://mdu.cashguo.top

Java: s.indexOf("x")
来源：http://tri.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://zxt.wangdashe.top

Ruby: s.index("x")
来源：http://puf.cheryme.top

C#:   s.IndexOf("x")
来源：http://pxe.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://gjx.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ifj.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ruu.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uiu.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nzo.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ekl.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://brg.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ovz.sweek.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pgb.jianghu66.top

[E06] 替换子串
来源：http://eam.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jrq.daria6918.cn

PHP:  str_replace("a", "b", $s);
来源：http://fzv.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgj.yuanzhike.top

TS:   s.replaceAll("a", "b")
来源：http://sli.smart0.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ojy.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ibh.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ijn.guowangkeji.top


<!-- 参考信息 -->