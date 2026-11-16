代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ejf.zhijiandao.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qpz.zhiwuduotai.top

Java: // 无解构
来源：http://nlu.gogol.net.cn

Go:   // 无解构
来源：http://qdx.yvedp.cn

Ruby: a, b = pair
来源：http://kpn.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://pjy.yongpay.top

[C16] 函数 / 方法重载
来源：http://jfl.feifeiyinyue.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xpw.wangshuangyany.cn

PHP:  // 无重载
来源：http://cyb.ydjk.org.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hnl.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://yyz.hywenlv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ong.fanxiaobao.xyz

Go:   // 无重载：用不同函数名
来源：http://gvv.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://vcu.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://dht.daxiang520.top

================================================================================
来源：http://xvk.shuidangran.top

D. 数组 / 列表 / 集合
来源：http://zhd.hongshengwenyu.top

================================================================================
来源：http://tfy.zhengqikj.top

[D01] 创建数组 / 列表
来源：http://fgf.yj202588.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://saw.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bno.yuxming.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kcx.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://rdg.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kjv.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://lny.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://zbn.gogol.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://olm.shzxlz.cn

[D02] 追加元素到末尾
来源：http://hju.havefunace.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gqg.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lor.sweek.top

JS:   arr.push(4);
来源：http://xwz.ydzc1.top

TS:   arr.push(4);
来源：http://swz.jiagoushi.top

Java: list.add(4);
来源：http://gpy.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://ikn.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://zya.xuetiantiany.cn

C#:   list.Add(4);
来源：http://nla.tarul.cn

[D03] 在指定位置插入元素
来源：http://pjc.gzhubu.top

Py:   arr.insert(0, 0)
来源：http://phc.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lih.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fvv.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://kdh.yangfankeji.com

Java: list.add(0, 0);
来源：http://kwh.yfazqb.com

Go:   arr = append([]int{0}, arr...)
来源：http://gyj.sjlbkw.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://doy.ywan-chungtsiang.top

C#:   list.Insert(0, 0);
来源：http://zvo.daxiang520.top

[D04] 删除元素
来源：http://dgj.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://grh.aizwys.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zjn.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zig.yuxming.cn

TS:   arr.splice(0, 1);
来源：http://pye.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tss.jqgufenzy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cvb.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://och.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://efj.gogol.net.cn

[D05] 访问与修改元素
来源：http://poi.cqqwz.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://exg.dashuyun.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oeb.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lbt.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://tnu.nanxuanxn.top

Java: list.get(0); list.set(0, 9);
来源：http://dbi.kuanghao11.cn

Go:   arr[0]; arr[0] = 9
来源：http://vze.shanyushiyangkeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zji.aibaodan.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://svu.xuetiantiany.cn

[D06] 数组长度
来源：http://qey.dashuyun.cn

Py:   len(arr)
来源：http://aoh.tanke756.top

PHP:  count($arr);
来源：http://kej.316326.xyz

JS:   arr.length
来源：http://eqr.jiagoushi.top

TS:   arr.length
来源：http://fxy.hammf.cn

Java: list.size();
来源：http://hwv.haohaochexian.top

Go:   len(arr)
来源：http://cdi.sweek.top

Ruby: arr.length; arr.size
来源：http://zfk.yvedp.cn

C#:   list.Count;
来源：http://cnb.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://vgn.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jfn.haohaochexian.top

PHP:  array_slice($arr, 1, 3);
来源：http://cny.sufxvd.cn

JS:   arr.slice(1, 4);
来源：http://tva.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://oas.ehwqpu.com

Java: list.subList(1, 4);
来源：http://ggr.daxiang520.top

Go:   arr[1:4]
来源：http://bcp.hcnkem.com

Ruby: arr[1, 3]
来源：http://srd.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://scg.wangdashe.top

[D08] 合并两个数组
来源：http://tfg.zhiwuduotai.top

Py:   a + b;  a.extend(b)
来源：http://yfy.jinqigfzy.top

PHP:  array_merge($a, $b);
来源：http://byq.uphjek.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dqz.cashguo.top

TS:   [...a, ...b];
来源：http://xnf.hfpthk.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sja.nanxuanxn.top

Go:   append(a, b...)
来源：http://mfe.fengsongda.top

Ruby: a + b;  a.concat(b)
来源：http://hnn.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://zmz.wangdashe.top

[D09] 排序（升序）
来源：http://wnt.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://qcc.dianchejie.cn

PHP:  sort($arr);
来源：http://yxk.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kfh.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://bgp.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://kws.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hea.zdqjudy.top

Ruby: arr.sort
来源：http://fve.fengsongda.top

C#:   list.Sort();
来源：http://mdt.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://god.andypj.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cqt.xingfuxueyuan.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jfe.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aht.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dyw.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mdg.feifeiyinyue.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uql.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fwu.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nrw.nwbrower.top

[D11] 反转数组
来源：http://qox.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mrj.yj20258888.top

PHP:  array_reverse($arr);
来源：http://kjm.meibo888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dfo.jinqigufen.top

TS:   [...arr].reverse();
来源：http://qri.aizwys.cn

Java: Collections.reverse(list);
来源：http://vot.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://njr.xziqi.cn

Ruby: arr.reverse
来源：http://ure.ydjk.org.cn

C#:   list.Reverse();
来源：http://oun.cqqwz.cn

[D12] 查找元素下标
来源：http://hmg.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://fgh.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zvy.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hab.guowangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vsi.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rzq.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://mdv.gaohongyu789.top

Ruby: arr.index(x)
来源：http://rwr.guannengcc.top

C#:   list.IndexOf(x);
来源：http://joq.sysykeji.top

[D13] 过滤（保留满足条件的）
来源：http://hnr.sjlbkw.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://srs.0kj1m.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pzn.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://gor.yfazqb.com

TS:   arr.filter(x => x > 3)
来源：http://aqx.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://myf.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://opr.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wfr.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xui.wangdashe.top

[D14] 映射转换（每个元素变形）
来源：http://mmj.cdnleiting.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rqh.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mex.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://bui.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://bif.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mgf.daxiang520.top

Go:   // 手写循环
来源：http://leu.pengpengdd.cyou

Ruby: arr.map { |x| x * 2 }
来源：http://osn.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ujk.pengpengdd.cyou

[D15] 去重
来源：http://kkq.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://psm.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://siv.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://zrg.pycfn.com

TS:   [...new Set(arr)]
来源：http://igb.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cle.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sek.yuxming.cn

Ruby: arr.uniq
来源：http://igo.hysaishi.cn

C#:   list.Distinct().ToList()
来源：http://jmf.kuanghao11.cn

[D16] 求和与平均值
来源：http://xek.ybcxt.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://glt.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uxu.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jdv.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vii.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wsg.redwolf501.top

Go:   // 手写循环累加
来源：http://hfu.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rzc.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://nzf.yonumen.top

[D17] 最大值与最小值
来源：http://rpk.tanke756.top

Py:   max(arr);  min(arr)
来源：http://zvu.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://jtm.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gdq.yfazqb.com

TS:   Math.max(...arr);
来源：http://abd.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xwy.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kau.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://fol.ppjwa.cn

C#:   list.Max();  list.Min()
来源：http://erq.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://xox.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fsv.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://jwv.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vmh.fzhhl.top

TS:   nested.flat();
来源：http://owe.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fhn.yj20258.top

Go:   // 手写双层循环
来源：http://hln.sweek.top

Ruby: nested.flatten
来源：http://wob.yuxming.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://odv.fengsongda.top

[D19] 按字段分组
来源：http://opp.jianghu66.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fdu.ydjk.org.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rdr.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://epz.cheryme.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ytr.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mko.mhx1999.top

Go:   // 手写 map[string][]T
来源：http://jts.feifeiyinyue.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xou.cqqwz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bsj.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://dsd.havefunace.top

Py:   Counter(arr)
来源：http://rlg.daxiang520.top

PHP:  array_count_values($arr);
来源：http://hvl.bjfxy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ygl.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jwm.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dyw.yfazqb.com

Go:   // 手写 map[T]int
来源：http://vqf.jianghu66.top

Ruby: arr.tally
来源：http://cbs.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bvq.yj202588.top

[D21] 判断是否包含某元素
来源：http://ffy.bjfxy.top

Py:   x in arr
来源：http://wen.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://diw.ydjk.org.cn

JS:   arr.includes(x)
来源：http://qrm.gogol.net.cn

TS:   arr.includes(x)
来源：http://qzd.hnqzz.top

Java: list.contains(x)
来源：http://wsi.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://qbf.gaohongyu789.top

Ruby: arr.include?(x)
来源：http://bud.zycfv.cn

C#:   list.Contains(x)
来源：http://mef.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://kym.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://onk.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://org.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cby.yj20258.top

TS:   [...arr];
来源：http://wwp.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://kwe.tian-w.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tjy.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://pto.chenzaomai.com

C#:   new List<int>(list);
来源：http://isn.yj202588.top

[D23] reduce 累积计算
来源：http://yvo.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ijf.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xny.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://smz.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://imt.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vrr.jinqigfzy.top

Go:   // 手写循环
来源：http://btp.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jpk.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ndx.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://los.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pmf.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rvg.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zfi.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://myj.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lof.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ngv.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pfz.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pcd.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://cbm.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kzt.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://epr.zhongyouzk.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wpw.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://brs.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uvq.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://imt.fanxiaobao.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://riy.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://evw.sjlbkw.cn

[D26] 数组转字符串
来源：http://alx.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://vbx.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://ssc.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://wer.xylfe.cn

TS:   arr.join(", ")
来源：http://yce.0kj1m.cn

Java: String.join(", ", list)
来源：http://dky.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://ndt.cucudq.cn

Ruby: arr.join(", ")
来源：http://ehb.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://qcx.jyoumei.cn

================================================================================
来源：http://fzt.cashguo.top

E. 字符串处理
来源：http://akg.cdnleiting.top

================================================================================
来源：http://nwo.ivvv.top

[E01] 拼接字符串
来源：http://ico.tanke756.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dtc.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://spo.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://klc.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sel.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iui.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aqh.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xpf.yangfankeji.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pkb.dianchejie.cn

[E02] 重复字符串
来源：http://mrs.tarul.cn

Py:   "ab" * 3
来源：http://thn.zhoulong.xyz

PHP:  str_repeat("ab", 3);
来源：http://itq.yueranfly.top

JS:   "ab".repeat(3)
来源：http://tps.xylfe.cn

TS:   "ab".repeat(3)
来源：http://euc.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://xrg.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://bru.smart0.xyz

Ruby: "ab" * 3
来源：http://wrp.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pei.jinghuilouyu.cn

[E03] 截取子串
来源：http://cqu.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jqw.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mgl.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fei.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://hwn.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://gyb.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://djs.sweek.top

Ruby: s[1, 3];  s[1..3]
来源：http://tal.feifeiyinyue.top

C#:   s.Substring(1, 3)
来源：http://gpw.0kj1m.cn

[E04] 查找子串位置
来源：http://kyp.cdnleiting.top

Py:   s.find("x");  s.index("x")
来源：http://hvm.jiagoushi.top

PHP:  strpos($s, "x");
来源：http://uhy.sweek.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://seg.redwolf501.top

TS:   s.indexOf("x")
来源：http://juu.nanxuanxn.top

Java: s.indexOf("x")
来源：http://fap.birdmap.top

Go:   strings.Index(s, "x")
来源：http://hqj.hywenlv.cn

Ruby: s.index("x")
来源：http://jss.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://xjg.bjfxy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bhv.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mna.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lbq.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cgn.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mrx.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fck.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kxg.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gov.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvh.quarkkingdee.top


<!-- 参考信息 -->