代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://njc.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dhv.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zgh.pengpengdd.cyou

Ruby: # 无泛型
来源：http://rxo.tian-w.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ung.yangfankeji.com

[C15] 解构 / 展开参数
来源：http://yyr.vqdsnc.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rge.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://ymx.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zhj.andypj.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://onb.fanxiaobao.xyz

Java: // 无解构
来源：http://vak.chenjidiqi.icu

Go:   // 无解构
来源：http://mre.kuanghao11.cn

Ruby: a, b = pair
来源：http://vii.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://jxh.hammf.cn

[C16] 函数 / 方法重载
来源：http://zuv.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://iqi.mhx1999.top

PHP:  // 无重载
来源：http://cpn.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://gwc.zhaomingkeji.xyz

TS:   // 用联合类型或重载签名声明
来源：http://utm.quarkkingdee.top

Java: void f(int a) {}  void f(String a) {}
来源：http://smx.sweek.top

Go:   // 无重载：用不同函数名
来源：http://dur.nanxinkj.top

Ruby: # 无重载：靠动态参数
来源：http://olr.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://shl.yangfankeji.com

================================================================================
来源：http://kzf.guannengcc.top

D. 数组 / 列表 / 集合
来源：http://eam.xingfuxueyuan.xyz

================================================================================
来源：http://kxz.vehdjk.com

[D01] 创建数组 / 列表
来源：http://zzx.9152youxi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://azu.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sml.jinqigufen.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jgo.jinyuanbaomall.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oac.yangfankeji.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fqs.yanxiufei.cn

Go:   arr := []int{1, 2, 3}
来源：http://rgz.uphjek.com

Ruby: arr = [1, 2, 3]
来源：http://zle.tian-w.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xer.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://kwa.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pbs.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fnz.sysykeji.top

JS:   arr.push(4);
来源：http://wfu.iojbl.cn

TS:   arr.push(4);
来源：http://mad.andypj.xyz

Java: list.add(4);
来源：http://rfd.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://oqx.mhx1999.top

Ruby: arr << 4; arr.push(5)
来源：http://zeg.0kj1m.cn

C#:   list.Add(4);
来源：http://vqf.fktsv.cn

[D03] 在指定位置插入元素
来源：http://trq.yfazqb.com

Py:   arr.insert(0, 0)
来源：http://apy.redwolf501.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://svk.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vwd.bbcook.cn

TS:   arr.splice(0, 0, 0);
来源：http://uzm.guowangkeji.top

Java: list.add(0, 0);
来源：http://xqj.cdnleiting.top

Go:   arr = append([]int{0}, arr...)
来源：http://ipi.hammf.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sea.guannengcc.top

C#:   list.Insert(0, 0);
来源：http://okm.ivvv.top

[D04] 删除元素
来源：http://trq.nwbrower.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://umx.sxryk.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ava.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cph.sysykeji.top

TS:   arr.splice(0, 1);
来源：http://lrw.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zoj.hnxiangtu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dpj.wangshuangyany.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://rqm.zdqjudy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jrx.aibaodan.cn

[D05] 访问与修改元素
来源：http://yuo.tianlin.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hra.tian-w.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xew.chenlongwang.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qzz.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://bie.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://bfz.gogol.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://pqy.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ymg.guowangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jaf.316326.xyz

[D06] 数组长度
来源：http://cdp.sxryk.cn

Py:   len(arr)
来源：http://ayr.sweek.top

PHP:  count($arr);
来源：http://rnt.hfpthk.cn

JS:   arr.length
来源：http://ynn.fktsv.cn

TS:   arr.length
来源：http://yug.gotoacloud.top

Java: list.size();
来源：http://lqn.jqgufenzy.top

Go:   len(arr)
来源：http://llz.wangdashe.top

Ruby: arr.length; arr.size
来源：http://blo.nwbrower.top

C#:   list.Count;
来源：http://cyv.xuanzx.com

[D07] 切片 / 取子数组
来源：http://jxx.zhijiandao.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tnt.zhijiandao.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jjs.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://xtz.tarul.cn

TS:   arr.slice(1, 4);
来源：http://kzv.mhx1999.top

Java: list.subList(1, 4);
来源：http://srd.316326.xyz

Go:   arr[1:4]
来源：http://tmu.bjfxy.top

Ruby: arr[1, 3]
来源：http://clw.zhijiandao.cn

C#:   list.GetRange(1, 3);
来源：http://ubz.52xcode.cn

[D08] 合并两个数组
来源：http://upn.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://ifr.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://qct.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xoe.vqdsnc.cn

TS:   [...a, ...b];
来源：http://ylh.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vpw.316326.xyz

Go:   append(a, b...)
来源：http://gzk.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://cia.yueranfly.top

C#:   a.Concat(b).ToList()
来源：http://nzo.haohaochexian.top

[D09] 排序（升序）
来源：http://tda.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://thd.shzxlz.cn

PHP:  sort($arr);
来源：http://ouy.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bam.9152youxi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vmf.chenzaomai.com

Java: Collections.sort(list);  list.sort(null);
来源：http://kzq.jinqigufen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qdy.ivvv.top

Ruby: arr.sort
来源：http://nce.sxryk.cn

C#:   list.Sort();
来源：http://mte.fehbvm.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://twl.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nnx.sysykeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mqm.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eha.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://onq.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dck.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hxl.shzxlz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dvf.jlsjyb.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cvl.ctjpmb.com

[D11] 反转数组
来源：http://paa.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://ydt.yongpay.top

PHP:  array_reverse($arr);
来源：http://fyp.c1oappe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sik.chenlongwang.top

TS:   [...arr].reverse();
来源：http://zzm.daria6918.cn

Java: Collections.reverse(list);
来源：http://xzn.jyoumei.cn

Go:   slices.Reverse(arr)
来源：http://thd.tarul.cn

Ruby: arr.reverse
来源：http://tzx.nwbrower.top

C#:   list.Reverse();
来源：http://kyj.tarul.cn

[D12] 查找元素下标
来源：http://lrk.meibo888.top

Py:   arr.index(x);  x in arr
来源：http://rqy.fanxiaobao.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uoj.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xix.jinqigufen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://noc.zycfv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ukp.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://bme.svipenyu.cn

Ruby: arr.index(x)
来源：http://adf.fehbvm.com

C#:   list.IndexOf(x);
来源：http://vqx.ehwqpu.com

[D13] 过滤（保留满足条件的）
来源：http://hxq.guowangkeji.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://orj.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://apf.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://rdo.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://pvs.tianlin.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ifw.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dwe.daxiang520.top

Ruby: arr.select { |x| x > 3 }
来源：http://ocg.jqgfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nbk.zhijiandao.cn

[D14] 映射转换（每个元素变形）
来源：http://vzx.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fgi.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://djq.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://yah.vehdjk.com

TS:   arr.map(x => x * 2)
来源：http://gzm.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ldd.chenlongwang.top

Go:   // 手写循环
来源：http://xww.jqgufenzy.top

Ruby: arr.map { |x| x * 2 }
来源：http://anc.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ekd.52xcode.cn

[D15] 去重
来源：http://bgx.fehbvm.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://llp.vqdsnc.cn

PHP:  array_unique($arr);
来源：http://hmx.zhengqikj.top

JS:   [...new Set(arr)]
来源：http://col.tanke756.top

TS:   [...new Set(arr)]
来源：http://hso.hcnkem.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dnz.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ytz.cashguo.top

Ruby: arr.uniq
来源：http://sbw.yj202588.top

C#:   list.Distinct().ToList()
来源：http://suu.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://uoj.guowangkeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jez.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sms.tianlin.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fin.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gax.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://siw.hnqzz.top

Go:   // 手写循环累加
来源：http://rba.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://acj.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://vxf.wangshuangyany.cn

[D17] 最大值与最小值
来源：http://vrm.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://naj.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://hmb.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yha.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://usr.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zwl.yj20258888.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fcd.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://uez.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://eaf.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://xkw.chenjidiqi.icu

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://onp.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://zlh.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vrn.jinqigfzy.top

TS:   nested.flat();
来源：http://kfp.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jhs.sxryk.cn

Go:   // 手写双层循环
来源：http://xnx.cheryme.top

Ruby: nested.flatten
来源：http://ogz.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://iht.dianchejie.cn

[D19] 按字段分组
来源：http://evs.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ogf.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cvm.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://twl.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lij.tanke756.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://muk.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://uwg.yj20258888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yjv.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kjz.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://msj.aibaodan.cn

Py:   Counter(arr)
来源：http://rjl.snrcjt.cn

PHP:  array_count_values($arr);
来源：http://tks.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://agm.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iqh.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dhs.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://pmo.hammf.cn

Ruby: arr.tally
来源：http://tsp.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hxy.aizwys.cn

[D21] 判断是否包含某元素
来源：http://ugl.0kj1m.cn

Py:   x in arr
来源：http://eaz.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://aqr.iojbl.cn

JS:   arr.includes(x)
来源：http://wdd.cashguo.top

TS:   arr.includes(x)
来源：http://svk.snrcjt.cn

Java: list.contains(x)
来源：http://xnq.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://ife.yuanzhike.top

Ruby: arr.include?(x)
来源：http://rtk.jqgufenzy.top

C#:   list.Contains(x)
来源：http://jdm.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://tfn.svipenyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nor.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iqw.wangdashe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zyc.xinyue.icu

TS:   [...arr];
来源：http://equ.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://xtz.xuanzx.com

Go:   copied := append([]int(nil), arr...)
来源：http://hoz.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://iij.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://iyi.guannengcc.top

[D23] reduce 累积计算
来源：http://lrr.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qsz.xingfuxueyuan.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nlc.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://erw.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ojv.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xzo.jinqigufen.top

Go:   // 手写循环
来源：http://ijw.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nrs.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cxv.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://tns.nwbrower.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ckh.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dnu.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ubh.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uiv.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://scf.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gmf.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pdw.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cuj.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://ika.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vhu.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iwy.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tkg.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ehc.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://svu.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jzn.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xyx.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nbg.hesvh.cn

[D26] 数组转字符串
来源：http://ocq.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://svi.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://ror.wangdashe.top

JS:   arr.join(", ")
来源：http://ymy.dashuyun.cn

TS:   arr.join(", ")
来源：http://wik.meibo888.top

Java: String.join(", ", list)
来源：http://ijh.ppjwa.cn

Go:   strings.Join(strs, ", ")
来源：http://wsu.pycfn.com

Ruby: arr.join(", ")
来源：http://fjo.xingfuxueyuan.xyz

C#:   string.Join(", ", list)
来源：http://exr.tarul.cn

================================================================================
来源：http://lww.jinyuanbaomall.cn

E. 字符串处理
来源：http://lji.jiagoushi.top

================================================================================
来源：http://ptp.bbcook.cn

[E01] 拼接字符串
来源：http://phx.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yoj.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uaj.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pjk.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ubg.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bpd.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bvt.xuanzx.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wum.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yrm.zhoulong.xyz

[E02] 重复字符串
来源：http://weh.sweek.top

Py:   "ab" * 3
来源：http://gvb.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://pos.iojbl.cn

JS:   "ab".repeat(3)
来源：http://mlu.cucudq.cn

TS:   "ab".repeat(3)
来源：http://prk.bbcook.cn

Java: "ab".repeat(3)
来源：http://ija.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://qzo.gzhubu.top

Ruby: "ab" * 3
来源：http://fbx.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nrr.jinqigfzy.top

[E03] 截取子串
来源：http://hvl.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tly.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://exi.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mlz.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://tvi.zycfv.cn

Java: s.substring(1, 4)
来源：http://mhh.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jcq.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jxo.havefunace.top

C#:   s.Substring(1, 3)
来源：http://wep.chenlongwang.top

[E04] 查找子串位置
来源：http://fxm.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://mjz.ivvv.top

PHP:  strpos($s, "x");
来源：http://gfr.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wmz.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://pek.jinqigufen.top

Java: s.indexOf("x")
来源：http://sug.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://bnh.hongshengwenyu.top

Ruby: s.index("x")
来源：http://fca.yj202588.top

C#:   s.IndexOf("x")
来源：http://slk.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://zah.yonumen.top


<!-- 参考信息 -->