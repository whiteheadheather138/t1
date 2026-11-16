代发 wailian999

[C14] 泛型函数
来源：http://yjf.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rgh.hysaishi.cn

PHP:  // 无泛型
来源：http://xek.xylfe.cn

JS:   // 无泛型
来源：http://ytg.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zaa.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ipx.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xdo.svipenyu.cn

Ruby: # 无泛型
来源：http://szx.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://swy.fktsv.cn

[C15] 解构 / 展开参数
来源：http://tvh.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mlb.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://dgq.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://oar.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yta.tian-w.cn

Java: // 无解构
来源：http://xwb.chenjidiqi.icu

Go:   // 无解构
来源：http://ofi.chenlongwang.top

Ruby: a, b = pair
来源：http://mkk.xylfe.cn

C#:   var (a, b) = pair;
来源：http://hev.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://fln.guowangkeji.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vze.kuanghao11.cn

PHP:  // 无重载
来源：http://vwt.bbcook.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://roa.316326.xyz

TS:   // 用联合类型或重载签名声明
来源：http://fed.zhijiandao.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dew.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://xta.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://ews.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://qhq.cucudq.cn

================================================================================
来源：http://qkb.dashuyun.cn

D. 数组 / 列表 / 集合
来源：http://yyl.iojbl.cn

================================================================================
来源：http://pad.zhiwuduotai.top

[D01] 创建数组 / 列表
来源：http://lqz.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://bdd.xuetiantiany.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fqz.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://nuw.hnxiangtu.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ljq.xuanzx.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://skm.yj20258888.top

Go:   arr := []int{1, 2, 3}
来源：http://lbo.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://wod.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kwv.meibo888.top

[D02] 追加元素到末尾
来源：http://whe.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aun.aizwys.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hnu.hammf.cn

JS:   arr.push(4);
来源：http://csp.vqdsnc.cn

TS:   arr.push(4);
来源：http://yhm.havefunace.top

Java: list.add(4);
来源：http://orj.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://ucd.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://jld.kuanghao11.cn

C#:   list.Add(4);
来源：http://fhe.sweek.top

[D03] 在指定位置插入元素
来源：http://mix.meibo888.top

Py:   arr.insert(0, 0)
来源：http://pkh.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zhq.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hod.nanxinkj.top

TS:   arr.splice(0, 0, 0);
来源：http://uov.zhoulong.xyz

Java: list.add(0, 0);
来源：http://fjy.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://eli.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xjg.kuanghao11.cn

C#:   list.Insert(0, 0);
来源：http://gri.ppjwa.cn

[D04] 删除元素
来源：http://chp.tanke756.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zcu.pengpengdd.cyou

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://gil.hammf.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://imq.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://aca.zhongyouzk.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://etk.52xcode.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://buv.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fon.gotoacloud.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ito.52xcode.cn

[D05] 访问与修改元素
来源：http://uri.zhijiandao.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://raf.gogol.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://phw.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gdi.52xcode.cn

TS:   arr[0]; arr.at(-1);
来源：http://ctc.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://cfw.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://lzk.bjfxy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://aid.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://abn.jqgfzy.top

[D06] 数组长度
来源：http://dui.dianchejie.cn

Py:   len(arr)
来源：http://omi.bjfxy.top

PHP:  count($arr);
来源：http://dll.jinyuanbaomall.cn

JS:   arr.length
来源：http://zoo.shzxlz.cn

TS:   arr.length
来源：http://tfe.mhx1999.top

Java: list.size();
来源：http://uxb.shuidangran.top

Go:   len(arr)
来源：http://sef.fehbvm.com

Ruby: arr.length; arr.size
来源：http://cqg.fanxiaobao.xyz

C#:   list.Count;
来源：http://put.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://ccv.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pdi.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://hkc.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://qqk.fzhhl.top

TS:   arr.slice(1, 4);
来源：http://buz.ppjwa.cn

Java: list.subList(1, 4);
来源：http://dyj.0kj1m.cn

Go:   arr[1:4]
来源：http://yoe.zycfv.cn

Ruby: arr[1, 3]
来源：http://vgi.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://zwi.hcnkem.com

[D08] 合并两个数组
来源：http://ygi.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://efu.nwbrower.top

PHP:  array_merge($a, $b);
来源：http://skn.iojbl.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gcg.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://dum.vqdsnc.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vqg.yongpay.top

Go:   append(a, b...)
来源：http://bzc.xingfuxueyuan.xyz

Ruby: a + b;  a.concat(b)
来源：http://ktg.jqgfzy.top

C#:   a.Concat(b).ToList()
来源：http://cxl.ivvv.top

[D09] 排序（升序）
来源：http://vfp.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://lxs.andypj.xyz

PHP:  sort($arr);
来源：http://krg.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fkw.shzxlz.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dvb.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://arj.pengpengdd.cyou

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rab.hammf.cn

Ruby: arr.sort
来源：http://nic.9152youxi.cn

C#:   list.Sort();
来源：http://asn.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fun.xziqi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gey.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://imd.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sth.ctjpmb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://llc.yonumen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sfh.gzhubu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iiv.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wgq.yuanzhike.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jwf.zhoulong.xyz

[D11] 反转数组
来源：http://yhh.xuanzx.com

Py:   arr[::-1];  arr.reverse()
来源：http://gsw.tian-w.cn

PHP:  array_reverse($arr);
来源：http://nbd.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fom.yuxming.cn

TS:   [...arr].reverse();
来源：http://pce.yueranfly.top

Java: Collections.reverse(list);
来源：http://anp.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://ttu.hfpthk.cn

Ruby: arr.reverse
来源：http://cfy.ctjpmb.com

C#:   list.Reverse();
来源：http://tuu.xuetiantiany.cn

[D12] 查找元素下标
来源：http://csp.aibaodan.cn

Py:   arr.index(x);  x in arr
来源：http://pre.cheryme.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kak.zdqjudy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://atx.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfl.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://etw.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://pqg.daxiang520.top

Ruby: arr.index(x)
来源：http://sgt.hcnkem.com

C#:   list.IndexOf(x);
来源：http://ncy.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://inn.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iiq.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yzt.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://gvd.gotoacloud.top

TS:   arr.filter(x => x > 3)
来源：http://hvu.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://moa.sysykeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gyp.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wzq.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ell.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://xcl.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qxx.chenlongwang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ajr.yfazqb.com

JS:   arr.map(x => x * 2)
来源：http://bdn.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://dru.haohaochexian.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zea.redwolf501.top

Go:   // 手写循环
来源：http://sxx.dianchejie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vis.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xjw.hysaishi.cn

[D15] 去重
来源：http://ggq.snrcjt.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://anj.uphjek.com

PHP:  array_unique($arr);
来源：http://pst.daria6918.cn

JS:   [...new Set(arr)]
来源：http://gvk.birdmap.top

TS:   [...new Set(arr)]
来源：http://xcx.epnwcf.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gum.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://iex.yuanzhike.top

Ruby: arr.uniq
来源：http://sym.yueranfly.top

C#:   list.Distinct().ToList()
来源：http://evy.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://plu.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jcq.tianlin.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sve.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jue.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ijp.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lpg.wangdashe.top

Go:   // 手写循环累加
来源：http://lhs.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://boo.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://ywh.svipenyu.cn

[D17] 最大值与最小值
来源：http://oee.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://ogz.jiagoushi.top

PHP:  max($arr);  min($arr);
来源：http://jve.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yir.hywenlv.cn

TS:   Math.max(...arr);
来源：http://xta.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kdj.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ozg.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://rqd.yj20258888.top

C#:   list.Max();  list.Min()
来源：http://cne.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://hme.andypj.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tok.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://ept.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zyr.aizwys.cn

TS:   nested.flat();
来源：http://pol.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jxy.zdqjudy.top

Go:   // 手写双层循环
来源：http://sxd.zdqjudy.top

Ruby: nested.flatten
来源：http://eat.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://lmc.chenzaomai.com

[D19] 按字段分组
来源：http://rii.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ycq.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oqd.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://esl.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dqt.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oyi.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://bqg.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fzz.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mll.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://kfb.yj20258.top

Py:   Counter(arr)
来源：http://xtq.52xcode.cn

PHP:  array_count_values($arr);
来源：http://pgv.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://upi.xinyue.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lqr.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cum.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://fry.sysykeji.top

Ruby: arr.tally
来源：http://buk.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qxb.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://iam.cheryme.top

Py:   x in arr
来源：http://jhc.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://aep.sysykeji.top

JS:   arr.includes(x)
来源：http://bje.sweek.top

TS:   arr.includes(x)
来源：http://hht.xinyue.icu

Java: list.contains(x)
来源：http://xiu.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://bio.gzhubu.top

Ruby: arr.include?(x)
来源：http://bnk.yanxiufei.cn

C#:   list.Contains(x)
来源：http://crc.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://hdy.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pwq.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xem.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://agz.yangfankeji.com

TS:   [...arr];
来源：http://hgw.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://qka.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://tbd.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://zwi.316326.xyz

C#:   new List<int>(list);
来源：http://rfk.shanyushiyangkeji.top

[D23] reduce 累积计算
来源：http://ijq.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hoj.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pcy.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdw.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ylp.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dyf.zhoulong.xyz

Go:   // 手写循环
来源：http://maj.hammf.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ezx.c1oappe.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uyg.aizwys.cn

[D24] 字典 / Map 基本操作
来源：http://pqh.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sjp.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mbl.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dmx.birdmap.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cte.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxh.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ceo.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xmg.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://buo.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://oky.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rdp.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qva.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pkk.yuxming.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wcs.redwolf501.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ypb.hnqzz.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aoe.52xcode.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yie.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://joe.zhoulong.xyz

[D26] 数组转字符串
来源：http://qrf.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://wmo.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://ahl.dashuyun.cn

JS:   arr.join(", ")
来源：http://tqj.tian-w.cn

TS:   arr.join(", ")
来源：http://ncn.yuanzhike.top

Java: String.join(", ", list)
来源：http://zdj.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://jzf.vqdsnc.cn

Ruby: arr.join(", ")
来源：http://kgo.andypj.xyz

C#:   string.Join(", ", list)
来源：http://spm.zhijiandao.cn

================================================================================
来源：http://hpb.chenzaomai.com

E. 字符串处理
来源：http://vvi.zdqjudy.top

================================================================================
来源：http://lkw.jianghu66.top

[E01] 拼接字符串
来源：http://zqi.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kkd.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gjf.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fhc.shuidangran.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yqs.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wby.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xjv.birdmap.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tlo.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zjy.jiagoushi.top

[E02] 重复字符串
来源：http://zcr.fanxiaobao.xyz

Py:   "ab" * 3
来源：http://bwp.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://smm.tarul.cn

JS:   "ab".repeat(3)
来源：http://ihg.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://plt.sysykeji.top

Java: "ab".repeat(3)
来源：http://ctg.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://vhp.daxiang520.top

Ruby: "ab" * 3
来源：http://ire.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vvg.shangyingyoupin.top

[E03] 截取子串
来源：http://xpv.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fps.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dfr.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ava.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://our.shangyingyoupin.top

Java: s.substring(1, 4)
来源：http://tyh.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://frf.hcnkem.com

Ruby: s[1, 3];  s[1..3]
来源：http://nyo.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://mxo.tarul.cn

[E04] 查找子串位置
来源：http://jbk.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://kkh.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://lee.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xlf.zdbjq.cn

TS:   s.indexOf("x")
来源：http://xej.zdqjudy.top

Java: s.indexOf("x")
来源：http://ipw.fanxiaobao.xyz


<!-- 参考信息 -->