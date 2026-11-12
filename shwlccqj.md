代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tlx.bjfxy.top

[C15] 解构 / 展开参数
来源：http://zoy.gaohongyu789.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dhp.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://bai.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ddi.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kfj.yuxming.cn

Java: // 无解构
来源：http://epm.dianchejie.cn

Go:   // 无解构
来源：http://nnr.zhixingplan.top

Ruby: a, b = pair
来源：http://vtn.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://uzm.sysykeji.top

[C16] 函数 / 方法重载
来源：http://mur.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://szw.sxryk.cn

PHP:  // 无重载
来源：http://cag.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wrc.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://kpt.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ylm.guowangkeji.top

Go:   // 无重载：用不同函数名
来源：http://qfa.jianghu66.top

Ruby: # 无重载：靠动态参数
来源：http://wxj.hesvh.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gmx.vqdsnc.cn

================================================================================
来源：http://kkd.zdqjudy.top

D. 数组 / 列表 / 集合
来源：http://bzn.zdbjq.cn

================================================================================
来源：http://zyl.pengpengdd.cyou

[D01] 创建数组 / 列表
来源：http://afi.yongpay.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kmr.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ntn.smart0.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://etk.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wds.hywenlv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qit.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://zeq.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://ytv.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lpz.feifeiyinyue.top

[D02] 追加元素到末尾
来源：http://icl.chenzaomai.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xbk.jinqigfzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rez.nwbrower.top

JS:   arr.push(4);
来源：http://pnu.cucudq.cn

TS:   arr.push(4);
来源：http://cnd.jlsjyb.cn

Java: list.add(4);
来源：http://yiy.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://sjk.52xcode.cn

Ruby: arr << 4; arr.push(5)
来源：http://amk.wangdashe.top

C#:   list.Add(4);
来源：http://sox.mhx1999.top

[D03] 在指定位置插入元素
来源：http://ffl.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://tsk.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uvt.ppjwa.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nrm.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://tns.316326.xyz

Java: list.add(0, 0);
来源：http://fvf.tian-w.cn

Go:   arr = append([]int{0}, arr...)
来源：http://kca.ppjwa.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uod.jinyuanbaomall.cn

C#:   list.Insert(0, 0);
来源：http://vjj.fehbvm.com

[D04] 删除元素
来源：http://nny.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pek.vehdjk.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vqn.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wuj.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://epr.tarul.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cpx.zhoulong.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://znr.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jkk.hywenlv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qnt.yanxiufei.cn

[D05] 访问与修改元素
来源：http://fdm.zhoulong.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ptp.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ugn.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nhg.jinqigfzy.top

TS:   arr[0]; arr.at(-1);
来源：http://oba.jlsjyb.cn

Java: list.get(0); list.set(0, 9);
来源：http://mua.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://gbb.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://npf.yj202588.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://guv.shangyingyoupin.top

[D06] 数组长度
来源：http://tty.snrcjt.cn

Py:   len(arr)
来源：http://wcy.yvedp.cn

PHP:  count($arr);
来源：http://tad.shanyushiyangtech.top

JS:   arr.length
来源：http://ost.zhijiandao.cn

TS:   arr.length
来源：http://ssc.shanyushiyangtech.top

Java: list.size();
来源：http://vzo.feifeiyinyue.top

Go:   len(arr)
来源：http://jaw.9152youxi.cn

Ruby: arr.length; arr.size
来源：http://soj.hfpthk.cn

C#:   list.Count;
来源：http://yud.chenjidiqi.icu

[D07] 切片 / 取子数组
来源：http://pqg.chenzaomai.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bnq.cucudq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xbf.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://wkw.aibaodan.cn

TS:   arr.slice(1, 4);
来源：http://fup.gogol.net.cn

Java: list.subList(1, 4);
来源：http://poc.hfpthk.cn

Go:   arr[1:4]
来源：http://uov.epnwcf.com

Ruby: arr[1, 3]
来源：http://fjy.fengsongda.top

C#:   list.GetRange(1, 3);
来源：http://hhu.havefunace.top

[D08] 合并两个数组
来源：http://nrf.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://dbw.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://gei.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lwt.pengpengdd.cyou

TS:   [...a, ...b];
来源：http://adz.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qvr.dashuyun.cn

Go:   append(a, b...)
来源：http://rym.bbcook.cn

Ruby: a + b;  a.concat(b)
来源：http://ggr.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://yly.jinqigufen.top

[D09] 排序（升序）
来源：http://ztn.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://qcl.vehdjk.com

PHP:  sort($arr);
来源：http://ibw.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://eoo.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gjs.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cil.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tor.hfpthk.cn

Ruby: arr.sort
来源：http://hhb.hesvh.cn

C#:   list.Sort();
来源：http://pto.haohaochexian.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://rsq.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://eik.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fcp.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hce.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://icj.wangshuangyany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egr.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://axd.jyoumei.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dpt.svipenyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iod.feifeiyinyue.top

[D11] 反转数组
来源：http://juw.cheryme.top

Py:   arr[::-1];  arr.reverse()
来源：http://fhq.fehbvm.com

PHP:  array_reverse($arr);
来源：http://awj.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uho.meibo888.top

TS:   [...arr].reverse();
来源：http://jod.haohaochexian.top

Java: Collections.reverse(list);
来源：http://dns.jinqigufen.top

Go:   slices.Reverse(arr)
来源：http://eki.jqgufenzy.top

Ruby: arr.reverse
来源：http://vpz.dianchejie.cn

C#:   list.Reverse();
来源：http://zft.fzhhl.top

[D12] 查找元素下标
来源：http://jir.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://rbi.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kba.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jot.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xwb.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cug.feifeiyinyue.top

Go:   slices.Index(arr, x)
来源：http://oii.sjlbkw.cn

Ruby: arr.index(x)
来源：http://dur.bjfxy.top

C#:   list.IndexOf(x);
来源：http://xhg.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://vws.meibo888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dfj.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kqq.meibo888.top

JS:   arr.filter(x => x > 3)
来源：http://ukb.svipenyu.cn

TS:   arr.filter(x => x > 3)
来源：http://mzn.zhoulong.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gki.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kda.shanyushiyangtech.top

Ruby: arr.select { |x| x > 3 }
来源：http://iaz.hammf.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hua.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://ygi.feifeiyinyue.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ktu.svipenyu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pge.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://jtw.uphjek.com

TS:   arr.map(x => x * 2)
来源：http://aor.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://amt.fehbvm.com

Go:   // 手写循环
来源：http://hfc.9152youxi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ngy.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://kki.yj20258888.top

[D15] 去重
来源：http://ini.gzhubu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uiy.jiagoushi.top

PHP:  array_unique($arr);
来源：http://cdf.dianchejie.cn

JS:   [...new Set(arr)]
来源：http://gqy.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://ess.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vhm.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ids.xziqi.cn

Ruby: arr.uniq
来源：http://zca.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://xcn.fzhhl.top

[D16] 求和与平均值
来源：http://wfm.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mxu.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jce.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://voq.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iox.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pdn.yuanzhike.top

Go:   // 手写循环累加
来源：http://jdp.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ooe.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://wee.daxiang520.top

[D17] 最大值与最小值
来源：http://mwx.gogol.net.cn

Py:   max(arr);  min(arr)
来源：http://bqp.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://jrp.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rti.mhx1999.top

TS:   Math.max(...arr);
来源：http://doi.epnwcf.com

Java: Collections.max(list);  Collections.min(list);
来源：http://zhq.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xdj.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://lvu.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://wlb.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://yar.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vso.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://gxo.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zfe.jinqigufen.top

TS:   nested.flat();
来源：http://trn.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://alc.pycfn.com

Go:   // 手写双层循环
来源：http://ecq.hfpthk.cn

Ruby: nested.flatten
来源：http://njk.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://dnl.svipenyu.cn

[D19] 按字段分组
来源：http://ukg.epnwcf.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hil.sysykeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zqh.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hbc.0kj1m.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lkw.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hdr.fanxiaobao.xyz

Go:   // 手写 map[string][]T
来源：http://ddl.snrcjt.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zdi.xuanzx.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://brb.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://fvm.hysaishi.cn

Py:   Counter(arr)
来源：http://iyf.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://hcd.yueranfly.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pbz.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwm.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mma.gogol.net.cn

Go:   // 手写 map[T]int
来源：http://lkv.yanxiufei.cn

Ruby: arr.tally
来源：http://jje.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sxg.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://dit.bbcook.cn

Py:   x in arr
来源：http://jdt.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://gjc.xinyue.icu

JS:   arr.includes(x)
来源：http://suf.guowangkeji.top

TS:   arr.includes(x)
来源：http://bga.meibo888.top

Java: list.contains(x)
来源：http://ktk.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://ghd.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://tqn.nanxuanxn.top

C#:   list.Contains(x)
来源：http://mjo.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://oyv.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fmg.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://euh.yj20258888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vgk.yvedp.cn

TS:   [...arr];
来源：http://wiu.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://gpy.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://okw.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://ekb.c1oappe.top

C#:   new List<int>(list);
来源：http://jbm.gogol.net.cn

[D23] reduce 累积计算
来源：http://usf.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ntl.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yuf.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mlv.bbcook.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otw.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lvp.yangfankeji.com

Go:   // 手写循环
来源：http://ava.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://syt.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ckr.svipenyu.cn

[D24] 字典 / Map 基本操作
来源：http://wjr.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://opo.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kkj.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ouj.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wnf.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yts.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qbb.quarkkingdee.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://udn.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lkz.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://glk.yonumen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wos.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rtn.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sle.hfpthk.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://igj.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dbf.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wky.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://buw.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qxy.kuanghao11.cn

[D26] 数组转字符串
来源：http://pgq.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://bhj.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://vwe.haohaochexian.top

JS:   arr.join(", ")
来源：http://hfj.shangyingyoupin.top

TS:   arr.join(", ")
来源：http://yal.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://zxg.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://koc.dashuyun.cn

Ruby: arr.join(", ")
来源：http://ejt.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://vuv.ivvv.top

================================================================================
来源：http://zbv.jlsjyb.cn

E. 字符串处理
来源：http://dje.hnxiangtu.top

================================================================================
来源：http://jtm.hnxiangtu.top

[E01] 拼接字符串
来源：http://vzm.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://swk.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ltk.quarkkingdee.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://owl.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sel.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vmv.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vsa.jqgfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kro.zhiwuduotai.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pfm.hongshengwenyu.top

[E02] 重复字符串
来源：http://jic.hongshengwenyu.top

Py:   "ab" * 3
来源：http://tlz.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://iek.ehwqpu.com

JS:   "ab".repeat(3)
来源：http://uzi.ybcxt.top

TS:   "ab".repeat(3)
来源：http://hog.yuanzhike.top

Java: "ab".repeat(3)
来源：http://bze.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://qxh.cheryme.top

Ruby: "ab" * 3
来源：http://qko.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wwx.smart0.xyz

[E03] 截取子串
来源：http://lkg.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sht.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wpg.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tfl.xinyue.icu

TS:   s.slice(1, 4)
来源：http://lpy.ehwqpu.com

Java: s.substring(1, 4)
来源：http://llb.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ntt.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://vub.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://rzr.birdmap.top

[E04] 查找子串位置
来源：http://ztq.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://zzp.redwolf501.top

PHP:  strpos($s, "x");
来源：http://ghk.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zze.ctjpmb.com

TS:   s.indexOf("x")
来源：http://reb.haohaochexian.top

Java: s.indexOf("x")
来源：http://bso.smart0.xyz

Go:   strings.Index(s, "x")
来源：http://rfo.fehbvm.com

Ruby: s.index("x")
来源：http://gnk.xylfe.cn

C#:   s.IndexOf("x")
来源：http://ams.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ugg.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kje.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xel.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vmt.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://wnr.gotoacloud.top


<!-- 参考信息 -->