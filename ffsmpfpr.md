代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fdq.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dsb.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vht.yfazqb.com

Ruby: # 无泛型
来源：http://whu.hammf.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dej.tian-w.cn

[C15] 解构 / 展开参数
来源：http://gkl.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gvs.aizwys.cn

PHP:  [$a, $b] = $pair;
来源：http://bdo.yj20258.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nzo.yongpay.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rri.jlsjyb.cn

Java: // 无解构
来源：http://mlm.daxiang520.top

Go:   // 无解构
来源：http://fds.guannengcc.top

Ruby: a, b = pair
来源：http://zel.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://agx.uphjek.com

[C16] 函数 / 方法重载
来源：http://via.yj20258.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lhw.yangfankeji.com

PHP:  // 无重载
来源：http://lcu.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://sdb.hammf.cn

TS:   // 用联合类型或重载签名声明
来源：http://qxk.yvedp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lml.ydjk.org.cn

Go:   // 无重载：用不同函数名
来源：http://dmm.yj20258.top

Ruby: # 无重载：靠动态参数
来源：http://znq.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://syl.aibaodan.cn

================================================================================
来源：http://zdq.havefunace.top

D. 数组 / 列表 / 集合
来源：http://jmq.shanyushiyangkeji.top

================================================================================
来源：http://noa.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://jka.c1oappe.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://crh.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bga.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tjk.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://skb.dianchejie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wsa.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://tip.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://dys.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jtx.guowangkeji.top

[D02] 追加元素到末尾
来源：http://axk.svipenyu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wfp.xylfe.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lua.gzhubu.top

JS:   arr.push(4);
来源：http://zes.zhiwuduotai.top

TS:   arr.push(4);
来源：http://txi.bbcook.cn

Java: list.add(4);
来源：http://wut.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://lqm.nanxinkj.top

Ruby: arr << 4; arr.push(5)
来源：http://yru.uphjek.com

C#:   list.Add(4);
来源：http://euy.jyoumei.cn

[D03] 在指定位置插入元素
来源：http://uno.hnqzz.top

Py:   arr.insert(0, 0)
来源：http://grn.sweek.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tvh.fzhhl.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ayy.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://feq.hcnkem.com

Java: list.add(0, 0);
来源：http://qvo.sjlbkw.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wtu.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sob.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://voc.ydzc1.top

[D04] 删除元素
来源：http://val.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xzg.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fmu.svipenyu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://imx.cashguo.top

TS:   arr.splice(0, 1);
来源：http://jgq.yongpay.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vjb.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mla.sufxvd.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bfs.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ldq.ydzc1.top

[D05] 访问与修改元素
来源：http://fpz.fengsongda.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ylh.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://trz.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fqj.cdnleiting.top

TS:   arr[0]; arr.at(-1);
来源：http://agj.c1oappe.top

Java: list.get(0); list.set(0, 9);
来源：http://ozj.yvedp.cn

Go:   arr[0]; arr[0] = 9
来源：http://azk.yonumen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://juy.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kea.cqqwz.cn

[D06] 数组长度
来源：http://qkm.yj202588.top

Py:   len(arr)
来源：http://jwa.tarul.cn

PHP:  count($arr);
来源：http://mtm.ydjk.org.cn

JS:   arr.length
来源：http://ugl.cqqwz.cn

TS:   arr.length
来源：http://xre.zhiwuduotai.top

Java: list.size();
来源：http://ayv.jlsjyb.cn

Go:   len(arr)
来源：http://dvx.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://ppn.ywan-chungtsiang.top

C#:   list.Count;
来源：http://jvq.nwbrower.top

[D07] 切片 / 取子数组
来源：http://noh.nanxuanxn.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bcq.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://wab.yangfankeji.com

JS:   arr.slice(1, 4);
来源：http://dyz.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://mvq.ppjwa.cn

Java: list.subList(1, 4);
来源：http://iun.ywan-chungtsiang.top

Go:   arr[1:4]
来源：http://jih.fehbvm.com

Ruby: arr[1, 3]
来源：http://nce.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://euh.ydjk.org.cn

[D08] 合并两个数组
来源：http://ker.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://xjb.guannengcc.top

PHP:  array_merge($a, $b);
来源：http://jsc.epnwcf.com

JS:   [...a, ...b];  a.concat(b);
来源：http://cfd.wangdashe.top

TS:   [...a, ...b];
来源：http://ifl.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://roj.yfazqb.com

Go:   append(a, b...)
来源：http://jku.pengpengdd.cyou

Ruby: a + b;  a.concat(b)
来源：http://xgp.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://rht.0kj1m.cn

[D09] 排序（升序）
来源：http://uog.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://mho.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://szq.epnwcf.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zvk.aibaodan.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fyk.ywan-chungtsiang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pcb.nanxuanxn.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rfb.vqdsnc.cn

Ruby: arr.sort
来源：http://uzv.ppjwa.cn

C#:   list.Sort();
来源：http://xkq.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wdc.shzxlz.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qiy.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://khr.shangyingyoupin.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jhn.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xnr.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pkp.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://njr.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eat.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://caq.hywenlv.cn

[D11] 反转数组
来源：http://lad.yuxming.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ejy.havefunace.top

PHP:  array_reverse($arr);
来源：http://aky.jianghu66.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://aqs.wangshuangyany.cn

TS:   [...arr].reverse();
来源：http://edx.52xcode.cn

Java: Collections.reverse(list);
来源：http://zcb.pycfn.com

Go:   slices.Reverse(arr)
来源：http://tjl.yj20258888.top

Ruby: arr.reverse
来源：http://zmq.ehwqpu.com

C#:   list.Reverse();
来源：http://cln.9152youxi.cn

[D12] 查找元素下标
来源：http://jtc.yvedp.cn

Py:   arr.index(x);  x in arr
来源：http://jeh.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://esd.zhongyouzk.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lyn.jqgfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://srz.jinqigfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yen.uphjek.com

Go:   slices.Index(arr, x)
来源：http://ask.ivvv.top

Ruby: arr.index(x)
来源：http://pjw.guannengcc.top

C#:   list.IndexOf(x);
来源：http://olz.quarkkingdee.top

[D13] 过滤（保留满足条件的）
来源：http://bjx.jinqigfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fiz.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gmv.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://ovr.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://gwf.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blp.zhongyouzk.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://szb.yanxiufei.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zbb.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gpz.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://eko.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vln.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dkf.zhengqikj.top

JS:   arr.map(x => x * 2)
来源：http://hpk.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://kfy.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jwl.wangshuangyany.cn

Go:   // 手写循环
来源：http://doh.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jjf.uphjek.com

C#:   list.Select(x => x * 2).ToList()
来源：http://aab.zdqjudy.top

[D15] 去重
来源：http://kkq.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pgz.hnqzz.top

PHP:  array_unique($arr);
来源：http://dbp.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://gvw.fehbvm.com

TS:   [...new Set(arr)]
来源：http://isz.sufxvd.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eeq.bjfxy.top

Go:   // 用 map[T]struct{} 手写
来源：http://xzy.hongshengwenyu.top

Ruby: arr.uniq
来源：http://dcw.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://jlh.jinqigufen.top

[D16] 求和与平均值
来源：http://qkw.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yli.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yfo.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fkn.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lee.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dms.dashuyun.cn

Go:   // 手写循环累加
来源：http://hwn.zhengqikj.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uag.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://whq.uphjek.com

[D17] 最大值与最小值
来源：http://par.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://dcu.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://zdh.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tpk.smart0.xyz

TS:   Math.max(...arr);
来源：http://tfg.shuidangran.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iwo.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wgh.shuidangran.top

Ruby: arr.max;  arr.min
来源：http://dcl.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://asx.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://aey.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ywf.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://ehc.redwolf501.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://avj.daria6918.cn

TS:   nested.flat();
来源：http://isa.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jsr.smart0.xyz

Go:   // 手写双层循环
来源：http://kei.nwbrower.top

Ruby: nested.flatten
来源：http://qol.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xri.yangfankeji.com

[D19] 按字段分组
来源：http://wjw.zhengqikj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lot.tanke756.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bju.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nmw.sxryk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wrs.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mbb.hammf.cn

Go:   // 手写 map[string][]T
来源：http://ssv.ybcxt.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://npp.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qvk.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://ilk.aizwys.cn

Py:   Counter(arr)
来源：http://wuy.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://ahu.cheryme.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvc.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://njt.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kbg.xziqi.cn

Go:   // 手写 map[T]int
来源：http://hey.shanyushiyangtech.top

Ruby: arr.tally
来源：http://dpg.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jpu.hcnkem.com

[D21] 判断是否包含某元素
来源：http://ptj.xuanzx.com

Py:   x in arr
来源：http://lhk.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://nkh.yj202588.top

JS:   arr.includes(x)
来源：http://mig.52xcode.cn

TS:   arr.includes(x)
来源：http://vge.aibaodan.cn

Java: list.contains(x)
来源：http://hdj.aibaodan.cn

Go:   slices.Contains(arr, x)
来源：http://ylj.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://peh.chenzaomai.com

C#:   list.Contains(x)
来源：http://wos.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://ptf.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oje.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://you.yanxiufei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://isq.uphjek.com

TS:   [...arr];
来源：http://aou.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://hfb.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://uyw.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://utn.c1oappe.top

C#:   new List<int>(list);
来源：http://hjc.jqgufenzy.top

[D23] reduce 累积计算
来源：http://tey.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gli.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rds.cheryme.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rhe.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gbg.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tmk.shzxlz.cn

Go:   // 手写循环
来源：http://tqx.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dgl.gotoacloud.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rtw.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://btp.zhijiandao.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lve.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lsz.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zfd.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tiz.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hgz.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wig.fengsongda.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tsu.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jqq.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://lhe.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://knn.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bjz.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zcr.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cjg.tanke756.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rlx.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xhd.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lhm.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqw.gaohongyu789.top

[D26] 数组转字符串
来源：http://oar.sxryk.cn

Py:   ", ".join(map(str, arr))
来源：http://csj.yonumen.top

PHP:  implode(", ", $arr);
来源：http://ari.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://qja.nwbrower.top

TS:   arr.join(", ")
来源：http://msg.yj20258888.top

Java: String.join(", ", list)
来源：http://isk.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://cbi.xylfe.cn

Ruby: arr.join(", ")
来源：http://dzi.yj202588.top

C#:   string.Join(", ", list)
来源：http://jqm.zhijiandao.cn

================================================================================
来源：http://mpa.pycfn.com

E. 字符串处理
来源：http://nqn.chenjidiqi.icu

================================================================================
来源：http://gwp.jinqigfzy.top

[E01] 拼接字符串
来源：http://cuz.ydzc1.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://exr.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bel.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofr.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wef.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ypa.birdmap.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://enr.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fuz.yj20258.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://spc.xylfe.cn

[E02] 重复字符串
来源：http://cxb.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://siq.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://klo.wangdashe.top

JS:   "ab".repeat(3)
来源：http://kfx.fehbvm.com

TS:   "ab".repeat(3)
来源：http://odf.52xcode.cn

Java: "ab".repeat(3)
来源：http://pwb.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://kht.jinqigufen.top

Ruby: "ab" * 3
来源：http://ljy.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sjp.xuanzx.com

[E03] 截取子串
来源：http://cuy.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fcz.tianlin.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fbp.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dvn.epnwcf.com

TS:   s.slice(1, 4)
来源：http://mdt.gogol.net.cn

Java: s.substring(1, 4)
来源：http://poq.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pml.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bwg.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://hun.daxiang520.top

[E04] 查找子串位置
来源：http://bru.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://dom.shanyushiyangkeji.top

PHP:  strpos($s, "x");
来源：http://jet.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://occ.yj20258.top

TS:   s.indexOf("x")
来源：http://qqg.zycfv.cn

Java: s.indexOf("x")
来源：http://pko.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://drf.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://nmt.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://ooc.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://own.yongpay.top


<!-- 参考信息 -->