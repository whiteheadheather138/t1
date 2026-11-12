代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bmd.cucudq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uks.kuanghao11.cn

Java: // 无解构
来源：http://plj.zdbjq.cn

Go:   // 无解构
来源：http://vmy.316326.xyz

Ruby: a, b = pair
来源：http://scu.yueranfly.top

C#:   var (a, b) = pair;
来源：http://fjn.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://tdh.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://rqj.jiagoushi.top

PHP:  // 无重载
来源：http://nox.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xmi.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://efw.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lgt.cheryme.top

Go:   // 无重载：用不同函数名
来源：http://gns.tarul.cn

Ruby: # 无重载：靠动态参数
来源：http://buk.quarkkingdee.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://clu.daria6918.cn

================================================================================
来源：http://qru.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://uhc.tianlin.xyz

================================================================================
来源：http://tff.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://why.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tcs.guowangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oyd.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kwu.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://sel.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://icn.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://qvt.hysaishi.cn

Ruby: arr = [1, 2, 3]
来源：http://vej.shanyushiyangkeji.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://udh.jqgufenzy.top

[D02] 追加元素到末尾
来源：http://lkt.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hjt.aibaodan.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tre.jlsjyb.cn

JS:   arr.push(4);
来源：http://kvr.kuanghao11.cn

TS:   arr.push(4);
来源：http://trl.hammf.cn

Java: list.add(4);
来源：http://ryl.shuidangran.top

Go:   arr = append(arr, 4)
来源：http://ifr.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://tvr.dashuyun.cn

C#:   list.Add(4);
来源：http://erb.shanyushiyangkeji.top

[D03] 在指定位置插入元素
来源：http://kza.pycfn.com

Py:   arr.insert(0, 0)
来源：http://rty.yonumen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jru.shanyushiyangtech.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wpq.snrcjt.cn

TS:   arr.splice(0, 0, 0);
来源：http://pbv.dianchejie.cn

Java: list.add(0, 0);
来源：http://czn.dashuyun.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vqv.cqqwz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qny.sysykeji.top

C#:   list.Insert(0, 0);
来源：http://zvo.cqqwz.cn

[D04] 删除元素
来源：http://vyn.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vhf.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gwc.dianchejie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bxs.hongshengwenyu.top

TS:   arr.splice(0, 1);
来源：http://qvt.pengpengdd.cyou

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gmy.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ybv.ywan-chungtsiang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jtw.tianlin.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dts.nanxuanxn.top

[D05] 访问与修改元素
来源：http://dkh.hysaishi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kmg.hongshengwenyu.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://obv.zhixingplan.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gyn.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://wkm.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://fgn.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://egb.chenzaomai.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xei.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aed.vehdjk.com

[D06] 数组长度
来源：http://smy.cucudq.cn

Py:   len(arr)
来源：http://gcc.chenlongwang.top

PHP:  count($arr);
来源：http://hbr.yonumen.top

JS:   arr.length
来源：http://oyt.cqqwz.cn

TS:   arr.length
来源：http://vbg.zhiwuduotai.top

Java: list.size();
来源：http://kca.jianghu66.top

Go:   len(arr)
来源：http://kky.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://wfk.zhengqikj.top

C#:   list.Count;
来源：http://yqk.tian-w.cn

[D07] 切片 / 取子数组
来源：http://rnk.cheryme.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://czj.ybcxt.top

PHP:  array_slice($arr, 1, 3);
来源：http://eqk.hysaishi.cn

JS:   arr.slice(1, 4);
来源：http://nxk.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://bps.tarul.cn

Java: list.subList(1, 4);
来源：http://liz.zhijiandao.cn

Go:   arr[1:4]
来源：http://fyf.wangdashe.top

Ruby: arr[1, 3]
来源：http://vhb.hongshengwenyu.top

C#:   list.GetRange(1, 3);
来源：http://cya.yonumen.top

[D08] 合并两个数组
来源：http://wue.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://jry.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://eym.hfpthk.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sqz.dianchejie.cn

TS:   [...a, ...b];
来源：http://nwy.jqgfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lei.iojbl.cn

Go:   append(a, b...)
来源：http://doc.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://eng.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://kqm.0kj1m.cn

[D09] 排序（升序）
来源：http://fek.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://rrv.shangyingyoupin.top

PHP:  sort($arr);
来源：http://llh.zdqjudy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mbz.jqgufenzy.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lkl.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rfv.fanxiaobao.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yxo.zhengqikj.top

Ruby: arr.sort
来源：http://fmr.ehwqpu.com

C#:   list.Sort();
来源：http://rga.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nvw.chenzaomai.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pmp.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nsy.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jxb.ydjk.org.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qya.dianchejie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nuf.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yxw.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vkm.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iko.cdnleiting.top

[D11] 反转数组
来源：http://fkc.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://gey.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://cxv.ivvv.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ltb.hammf.cn

TS:   [...arr].reverse();
来源：http://jrp.hfpthk.cn

Java: Collections.reverse(list);
来源：http://gmd.316326.xyz

Go:   slices.Reverse(arr)
来源：http://pwl.zhoulong.xyz

Ruby: arr.reverse
来源：http://cxm.sysykeji.top

C#:   list.Reverse();
来源：http://sug.yvedp.cn

[D12] 查找元素下标
来源：http://fke.jyoumei.cn

Py:   arr.index(x);  x in arr
来源：http://myo.jinqigufen.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vqb.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cvo.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://grb.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://phx.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://rws.zhongyouzk.top

Ruby: arr.index(x)
来源：http://tge.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://gnm.wangshuangyany.cn

[D13] 过滤（保留满足条件的）
来源：http://thc.jqgufenzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fxy.sjlbkw.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dbe.fzhhl.top

JS:   arr.filter(x => x > 3)
来源：http://pby.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://icu.tarul.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cdt.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nbu.pengpengdd.cyou

Ruby: arr.select { |x| x > 3 }
来源：http://zzz.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tfz.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://mya.ppjwa.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sgk.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bph.andypj.xyz

JS:   arr.map(x => x * 2)
来源：http://lkf.snrcjt.cn

TS:   arr.map(x => x * 2)
来源：http://awk.jinqigfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://miq.jqgfzy.top

Go:   // 手写循环
来源：http://kgd.yangfankeji.com

Ruby: arr.map { |x| x * 2 }
来源：http://adr.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jeg.aibaodan.cn

[D15] 去重
来源：http://lxf.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://udg.ehwqpu.com

PHP:  array_unique($arr);
来源：http://mhu.fanxiaobao.xyz

JS:   [...new Set(arr)]
来源：http://cme.yvedp.cn

TS:   [...new Set(arr)]
来源：http://ike.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zdb.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sfw.yanxiufei.cn

Ruby: arr.uniq
来源：http://fed.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://fqj.xziqi.cn

[D16] 求和与平均值
来源：http://yio.0kj1m.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fes.gzhubu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mqe.pycfn.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://udx.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gae.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vtr.ydzc1.top

Go:   // 手写循环累加
来源：http://scu.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rnj.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://kjv.shuidangran.top

[D17] 最大值与最小值
来源：http://ynw.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://poo.jyoumei.cn

PHP:  max($arr);  min($arr);
来源：http://bgi.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uyz.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://wjq.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jik.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mpe.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://reb.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://bqw.pengpengdd.cyou

[D18] 扁平化嵌套数组
来源：http://ugn.cqqwz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://phj.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://lzp.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xol.sweek.top

TS:   nested.flat();
来源：http://weg.guannengcc.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vez.zdqjudy.top

Go:   // 手写双层循环
来源：http://hji.yj20258888.top

Ruby: nested.flatten
来源：http://rji.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://llh.cqqwz.cn

[D19] 按字段分组
来源：http://olj.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oby.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://obe.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cww.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uxs.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fex.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://gyi.uphjek.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zjh.c1oappe.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ycn.hnqzz.top

[D20] 统计每个元素出现次数
来源：http://olh.quarkkingdee.top

Py:   Counter(arr)
来源：http://oec.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://xhc.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qmr.zhoulong.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://omi.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://azm.chenzaomai.com

Go:   // 手写 map[T]int
来源：http://xhb.zycfv.cn

Ruby: arr.tally
来源：http://iff.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gam.fzhhl.top

[D21] 判断是否包含某元素
来源：http://xtg.redwolf501.top

Py:   x in arr
来源：http://apz.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://iae.fzhhl.top

JS:   arr.includes(x)
来源：http://jio.cucudq.cn

TS:   arr.includes(x)
来源：http://jtd.meibo888.top

Java: list.contains(x)
来源：http://fpe.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://uky.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://jjl.jinqigufen.top

C#:   list.Contains(x)
来源：http://swk.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://qnk.ydzc1.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qyn.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nfg.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bej.havefunace.top

TS:   [...arr];
来源：http://vym.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://sld.yuxming.cn

Go:   copied := append([]int(nil), arr...)
来源：http://obu.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://vbc.yuanzhike.top

C#:   new List<int>(list);
来源：http://jzr.ctjpmb.com

[D23] reduce 累积计算
来源：http://xfb.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kkc.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ppw.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qrm.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxi.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://udw.tianlin.xyz

Go:   // 手写循环
来源：http://ein.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://amy.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://plx.shangyingyoupin.top

[D24] 字典 / Map 基本操作
来源：http://ufz.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bks.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://meg.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://reu.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uxg.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zzz.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qfk.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sju.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fih.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://xce.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://txa.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gox.jinyuanbaomall.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yiz.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dmn.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pty.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rbk.aibaodan.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hyq.guowangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://whl.shanyushiyangtech.top

[D26] 数组转字符串
来源：http://mcl.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://sup.xinyue.icu

PHP:  implode(", ", $arr);
来源：http://fdo.9152youxi.cn

JS:   arr.join(", ")
来源：http://byh.xziqi.cn

TS:   arr.join(", ")
来源：http://tsr.cqqwz.cn

Java: String.join(", ", list)
来源：http://aps.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://yuo.hammf.cn

Ruby: arr.join(", ")
来源：http://url.iojbl.cn

C#:   string.Join(", ", list)
来源：http://qaj.gzhubu.top

================================================================================
来源：http://rrn.fktsv.cn

E. 字符串处理
来源：http://ofh.tian-w.cn

================================================================================
来源：http://qwn.ctjpmb.com

[E01] 拼接字符串
来源：http://czy.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tqv.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://usx.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rqr.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://odc.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://occ.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vzn.smart0.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mhg.uphjek.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jsm.vehdjk.com

[E02] 重复字符串
来源：http://afo.yj202588.top

Py:   "ab" * 3
来源：http://ymc.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://hok.epnwcf.com

JS:   "ab".repeat(3)
来源：http://aag.birdmap.top

TS:   "ab".repeat(3)
来源：http://jys.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://pun.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://jdi.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://dmq.smart0.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hmh.cdnleiting.top

[E03] 截取子串
来源：http://jct.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jhb.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nzx.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qxq.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://gmo.sufxvd.cn

Java: s.substring(1, 4)
来源：http://tdi.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fet.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://pxa.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://wgd.zhengqikj.top

[E04] 查找子串位置
来源：http://itr.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://njq.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://kqz.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qrk.zhixingplan.top

TS:   s.indexOf("x")
来源：http://mdq.cdnleiting.top

Java: s.indexOf("x")
来源：http://oou.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://dpm.hywenlv.cn

Ruby: s.index("x")
来源：http://jxw.hywenlv.cn

C#:   s.IndexOf("x")
来源：http://otz.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tux.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zih.birdmap.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lac.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gia.fzhhl.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://smg.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tqh.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ozz.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ksn.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bpf.aibaodan.cn


<!-- 参考信息 -->