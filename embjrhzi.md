代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nrt.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://see.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jae.smart0.xyz

Ruby: # 无泛型
来源：http://nic.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ojg.yvedp.cn

[C15] 解构 / 展开参数
来源：http://liv.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://puz.sysykeji.top

PHP:  [$a, $b] = $pair;
来源：http://jmm.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gju.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ird.hnqzz.top

Java: // 无解构
来源：http://yob.nanxinkj.top

Go:   // 无解构
来源：http://spt.redwolf501.top

Ruby: a, b = pair
来源：http://mxu.jiagoushi.top

C#:   var (a, b) = pair;
来源：http://tcp.pycfn.com

[C16] 函数 / 方法重载
来源：http://ngg.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://edg.redwolf501.top

PHP:  // 无重载
来源：http://ksz.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://tks.ppjwa.cn

TS:   // 用联合类型或重载签名声明
来源：http://gzd.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gqd.zhixingplan.top

Go:   // 无重载：用不同函数名
来源：http://zuo.sweek.top

Ruby: # 无重载：靠动态参数
来源：http://wbp.andypj.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ylw.52xcode.cn

================================================================================
来源：http://zvm.zdbjq.cn

D. 数组 / 列表 / 集合
来源：http://gbs.zhijiandao.cn

================================================================================
来源：http://xno.zdqjudy.top

[D01] 创建数组 / 列表
来源：http://rxe.chenlongwang.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://yux.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nin.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rtf.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qrf.shangyingyoupin.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hyo.gzhubu.top

Go:   arr := []int{1, 2, 3}
来源：http://vgh.jyoumei.cn

Ruby: arr = [1, 2, 3]
来源：http://hhd.zdbjq.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yck.ppjwa.cn

[D02] 追加元素到末尾
来源：http://dzr.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pam.yj20258888.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mml.jinqigfzy.top

JS:   arr.push(4);
来源：http://myl.gzhubu.top

TS:   arr.push(4);
来源：http://oax.gzhubu.top

Java: list.add(4);
来源：http://jso.kuanghao11.cn

Go:   arr = append(arr, 4)
来源：http://upw.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://hvz.0kj1m.cn

C#:   list.Add(4);
来源：http://rje.iojbl.cn

[D03] 在指定位置插入元素
来源：http://zoc.tian-w.cn

Py:   arr.insert(0, 0)
来源：http://lqg.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dbw.zhijiandao.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fwk.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://ozz.c1oappe.top

Java: list.add(0, 0);
来源：http://gla.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://som.hnxiangtu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nbr.svipenyu.cn

C#:   list.Insert(0, 0);
来源：http://zus.yongpay.top

[D04] 删除元素
来源：http://pgf.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hsk.yongpay.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qhy.zhixingplan.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zoq.haohaochexian.top

TS:   arr.splice(0, 1);
来源：http://pdn.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gpp.shanyushiyangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lcr.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uiw.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rct.ybcxt.top

[D05] 访问与修改元素
来源：http://nru.bjfxy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://trc.cqqwz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sjj.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fjb.c1oappe.top

TS:   arr[0]; arr.at(-1);
来源：http://atb.cheryme.top

Java: list.get(0); list.set(0, 9);
来源：http://rxo.sysykeji.top

Go:   arr[0]; arr[0] = 9
来源：http://gid.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://luf.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pmf.yangfankeji.com

[D06] 数组长度
来源：http://nsw.sxryk.cn

Py:   len(arr)
来源：http://kuk.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://ncz.guannengcc.top

JS:   arr.length
来源：http://poa.dashuyun.cn

TS:   arr.length
来源：http://nag.hnxiangtu.top

Java: list.size();
来源：http://ffw.haohaochexian.top

Go:   len(arr)
来源：http://mmf.jinqigufen.top

Ruby: arr.length; arr.size
来源：http://ave.pycfn.com

C#:   list.Count;
来源：http://nfs.tian-w.cn

[D07] 切片 / 取子数组
来源：http://wss.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hae.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://ith.birdmap.top

JS:   arr.slice(1, 4);
来源：http://muu.fanxiaobao.xyz

TS:   arr.slice(1, 4);
来源：http://hpw.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://rko.aibaodan.cn

Go:   arr[1:4]
来源：http://sze.tarul.cn

Ruby: arr[1, 3]
来源：http://qnz.wangdashe.top

C#:   list.GetRange(1, 3);
来源：http://cbo.xuanzx.com

[D08] 合并两个数组
来源：http://awy.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://tna.c1oappe.top

PHP:  array_merge($a, $b);
来源：http://xbg.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rlg.ehwqpu.com

TS:   [...a, ...b];
来源：http://nic.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://miy.zycfv.cn

Go:   append(a, b...)
来源：http://oda.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://zry.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://pep.meibo888.top

[D09] 排序（升序）
来源：http://qog.sweek.top

Py:   sorted(arr);  arr.sort()
来源：http://qst.guannengcc.top

PHP:  sort($arr);
来源：http://pvv.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ifk.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zqx.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fag.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://spd.fzhhl.top

Ruby: arr.sort
来源：http://fsx.fanxiaobao.xyz

C#:   list.Sort();
来源：http://xlq.jyoumei.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://itq.pengpengdd.cyou

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pnh.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uiw.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://moc.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zua.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://trv.vqdsnc.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ajk.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nia.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ppr.jinqigufen.top

[D11] 反转数组
来源：http://xzr.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://izi.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://ftb.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hze.yuxming.cn

TS:   [...arr].reverse();
来源：http://vrg.shangyingyoupin.top

Java: Collections.reverse(list);
来源：http://hvf.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://grv.fengsongda.top

Ruby: arr.reverse
来源：http://dud.tanke756.top

C#:   list.Reverse();
来源：http://feo.dashuyun.cn

[D12] 查找元素下标
来源：http://mjo.gogol.net.cn

Py:   arr.index(x);  x in arr
来源：http://teq.yj20258888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ujt.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://siv.fzhhl.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rek.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vpp.yongpay.top

Go:   slices.Index(arr, x)
来源：http://dfg.yuanzhike.top

Ruby: arr.index(x)
来源：http://udm.zdbjq.cn

C#:   list.IndexOf(x);
来源：http://hjo.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://pje.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xyt.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://urd.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://exx.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://amz.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lbz.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lle.c1oappe.top

Ruby: arr.select { |x| x > 3 }
来源：http://nfc.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cmi.jinqigfzy.top

[D14] 映射转换（每个元素变形）
来源：http://yet.sjlbkw.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sev.sxryk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mqf.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://frt.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://rcg.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://awv.xylfe.cn

Go:   // 手写循环
来源：http://dox.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://iqn.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://afj.jinqigufen.top

[D15] 去重
来源：http://knt.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wur.haohaochexian.top

PHP:  array_unique($arr);
来源：http://odz.hcnkem.com

JS:   [...new Set(arr)]
来源：http://wog.fanxiaobao.xyz

TS:   [...new Set(arr)]
来源：http://msb.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gnf.shangyingyoupin.top

Go:   // 用 map[T]struct{} 手写
来源：http://nga.fanxiaobao.xyz

Ruby: arr.uniq
来源：http://pss.redwolf501.top

C#:   list.Distinct().ToList()
来源：http://vqw.sxryk.cn

[D16] 求和与平均值
来源：http://dlw.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayf.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gne.zhijiandao.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://knh.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bxe.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mtd.snrcjt.cn

Go:   // 手写循环累加
来源：http://ucb.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://izv.yfazqb.com

C#:   list.Sum();  list.Average()
来源：http://kqa.shzxlz.cn

[D17] 最大值与最小值
来源：http://lmg.vehdjk.com

Py:   max(arr);  min(arr)
来源：http://cxq.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://klw.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bkt.cheryme.top

TS:   Math.max(...arr);
来源：http://cep.vqdsnc.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qhv.jinqigufen.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dae.chenlongwang.top

Ruby: arr.max;  arr.min
来源：http://ybx.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://fyp.hongshengwenyu.top

[D18] 扁平化嵌套数组
来源：http://ulu.yj20258.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rwi.tarul.cn

PHP:  array_merge(...$nested);
来源：http://kiy.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sul.fanxiaobao.xyz

TS:   nested.flat();
来源：http://vow.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nwk.vehdjk.com

Go:   // 手写双层循环
来源：http://vad.pengpengdd.cyou

Ruby: nested.flatten
来源：http://jwt.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ode.ybcxt.top

[D19] 按字段分组
来源：http://xst.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eev.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qjj.sysykeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qjw.gogol.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fxq.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bde.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://myf.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jjk.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nqo.xuanzx.com

[D20] 统计每个元素出现次数
来源：http://pds.redwolf501.top

Py:   Counter(arr)
来源：http://elu.hnqzz.top

PHP:  array_count_values($arr);
来源：http://lae.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hvv.hnxiangtu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uic.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zxj.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://oyf.xinyue.icu

Ruby: arr.tally
来源：http://hci.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xky.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://bwr.zhijiandao.cn

Py:   x in arr
来源：http://bqa.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://dcq.cashguo.top

JS:   arr.includes(x)
来源：http://bgt.shzxlz.cn

TS:   arr.includes(x)
来源：http://tan.ehwqpu.com

Java: list.contains(x)
来源：http://hey.zhongyouzk.top

Go:   slices.Contains(arr, x)
来源：http://sxe.zhengqikj.top

Ruby: arr.include?(x)
来源：http://rpc.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://vkz.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://dnq.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mti.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cfw.nanxinkj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nbi.yonumen.top

TS:   [...arr];
来源：http://vay.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://nzh.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jnu.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://xzb.ehwqpu.com

C#:   new List<int>(list);
来源：http://sqz.aizwys.cn

[D23] reduce 累积计算
来源：http://xdd.tarul.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sqd.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://beh.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xgv.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zkn.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://epm.ehwqpu.com

Go:   // 手写循环
来源：http://ryb.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xgl.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://asa.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://dxq.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gcx.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gxq.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oxh.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://afj.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kvv.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mau.xylfe.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cak.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wwl.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://wfz.bjfxy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xau.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pjo.ehwqpu.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eef.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ozz.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ztg.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://shk.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hgz.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eia.birdmap.top

[D26] 数组转字符串
来源：http://ybu.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://lei.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://yxr.yuxming.cn

JS:   arr.join(", ")
来源：http://cep.hnqzz.top

TS:   arr.join(", ")
来源：http://yll.tianlin.xyz

Java: String.join(", ", list)
来源：http://bhk.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://nbe.yangfankeji.com

Ruby: arr.join(", ")
来源：http://iuo.c1oappe.top

C#:   string.Join(", ", list)
来源：http://xiy.fanxiaobao.xyz

================================================================================
来源：http://jcc.jianghu66.top

E. 字符串处理
来源：http://qsv.nanxinkj.top

================================================================================
来源：http://rxy.bjfxy.top

[E01] 拼接字符串
来源：http://oje.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lod.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://agt.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bgi.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pbf.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kqe.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zbx.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pfh.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ied.zhengqikj.top

[E02] 重复字符串
来源：http://rre.shuidangran.top

Py:   "ab" * 3
来源：http://kkf.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://vwv.sxryk.cn

JS:   "ab".repeat(3)
来源：http://igs.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://dub.xinyue.icu

Java: "ab".repeat(3)
来源：http://ooq.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://lly.bjfxy.top

Ruby: "ab" * 3
来源：http://res.guowangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jwn.hcnkem.com

[E03] 截取子串
来源：http://xmv.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://izu.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fcv.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tgc.pycfn.com

TS:   s.slice(1, 4)
来源：http://ecy.hfpthk.cn

Java: s.substring(1, 4)
来源：http://fzn.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zsb.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hcs.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://dwt.ctjpmb.com

[E04] 查找子串位置
来源：http://ugu.yuanzhike.top

Py:   s.find("x");  s.index("x")
来源：http://wct.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://rcw.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mhp.tianlin.xyz

TS:   s.indexOf("x")
来源：http://vjk.zdqjudy.top

Java: s.indexOf("x")
来源：http://tew.yongpay.top

Go:   strings.Index(s, "x")
来源：http://zds.guowangkeji.top

Ruby: s.index("x")
来源：http://jpr.smart0.xyz

C#:   s.IndexOf("x")
来源：http://opo.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ffm.wangshuangyany.cn


<!-- 参考信息 -->