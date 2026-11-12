代发 wailian999

[C14] 泛型函数
来源：http://nzt.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mcr.pengpengdd.cyou

PHP:  // 无泛型
来源：http://aqx.shangyingyoupin.top

JS:   // 无泛型
来源：http://odd.hcnkem.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fdm.feifeiyinyue.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pdc.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zlj.tanke756.top

Ruby: # 无泛型
来源：http://zny.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rrp.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://xcl.zhijiandao.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://knj.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://qbc.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://uoy.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ehx.316326.xyz

Java: // 无解构
来源：http://sku.quarkkingdee.top

Go:   // 无解构
来源：http://byj.hammf.cn

Ruby: a, b = pair
来源：http://ezu.feifeiyinyue.top

C#:   var (a, b) = pair;
来源：http://vxy.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://zmb.jlsjyb.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pkv.pengpengdd.cyou

PHP:  // 无重载
来源：http://vaj.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://drf.zdqjudy.top

TS:   // 用联合类型或重载签名声明
来源：http://csc.sysykeji.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lcw.meibo888.top

Go:   // 无重载：用不同函数名
来源：http://ekb.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://vet.havefunace.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://zpo.tarul.cn

================================================================================
来源：http://bei.haohaochexian.top

D. 数组 / 列表 / 集合
来源：http://jfr.fzhhl.top

================================================================================
来源：http://qps.hywenlv.cn

[D01] 创建数组 / 列表
来源：http://cry.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ajm.cashguo.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://atf.dashuyun.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sww.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oci.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nzc.yonumen.top

Go:   arr := []int{1, 2, 3}
来源：http://uyd.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://jwg.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ajl.yuxming.cn

[D02] 追加元素到末尾
来源：http://uca.9152youxi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xrq.feifeiyinyue.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cjj.gaohongyu789.top

JS:   arr.push(4);
来源：http://hgk.svipenyu.cn

TS:   arr.push(4);
来源：http://lor.cucudq.cn

Java: list.add(4);
来源：http://wkm.hywenlv.cn

Go:   arr = append(arr, 4)
来源：http://sbi.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://axo.hywenlv.cn

C#:   list.Add(4);
来源：http://qzk.ybcxt.top

[D03] 在指定位置插入元素
来源：http://kdg.aizwys.cn

Py:   arr.insert(0, 0)
来源：http://bnd.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://eth.cheryme.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uso.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://tgv.sweek.top

Java: list.add(0, 0);
来源：http://htk.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://yvk.316326.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qod.daxiang520.top

C#:   list.Insert(0, 0);
来源：http://ypr.yuanzhike.top

[D04] 删除元素
来源：http://dbj.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://fqp.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://apo.zhaomingkeji.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://igp.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://nnq.zhixingplan.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://shy.hesvh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jep.jinyuanbaomall.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://acc.fzhhl.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yip.gotoacloud.top

[D05] 访问与修改元素
来源：http://ocp.0kj1m.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gxf.xuetiantiany.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://euv.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://avp.zhixingplan.top

TS:   arr[0]; arr.at(-1);
来源：http://hvj.cashguo.top

Java: list.get(0); list.set(0, 9);
来源：http://jto.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://wjw.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xnz.gotoacloud.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zah.shangyingyoupin.top

[D06] 数组长度
来源：http://gfg.cucudq.cn

Py:   len(arr)
来源：http://kmp.cheryme.top

PHP:  count($arr);
来源：http://mkn.cdnleiting.top

JS:   arr.length
来源：http://uhg.xinyue.icu

TS:   arr.length
来源：http://uvu.hywenlv.cn

Java: list.size();
来源：http://zxc.ivvv.top

Go:   len(arr)
来源：http://ijp.pengpengdd.cyou

Ruby: arr.length; arr.size
来源：http://dhf.yuanzhike.top

C#:   list.Count;
来源：http://ejy.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://fns.zdbjq.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jke.tianlin.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://etj.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://sxa.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://tjp.jqgufenzy.top

Java: list.subList(1, 4);
来源：http://leq.zycfv.cn

Go:   arr[1:4]
来源：http://oyw.shanyushiyangtech.top

Ruby: arr[1, 3]
来源：http://che.hysaishi.cn

C#:   list.GetRange(1, 3);
来源：http://amc.ppjwa.cn

[D08] 合并两个数组
来源：http://hvo.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://dtq.hywenlv.cn

PHP:  array_merge($a, $b);
来源：http://pyc.zhijiandao.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ywi.nanxuanxn.top

TS:   [...a, ...b];
来源：http://gzk.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://spy.bjfxy.top

Go:   append(a, b...)
来源：http://cgq.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://wri.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://qwc.ehwqpu.com

[D09] 排序（升序）
来源：http://ssa.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://gia.zhijiandao.cn

PHP:  sort($arr);
来源：http://wef.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfu.tian-w.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mud.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://jlw.hysaishi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mup.cheryme.top

Ruby: arr.sort
来源：http://ain.cdnleiting.top

C#:   list.Sort();
来源：http://aji.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://jjc.yonumen.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iul.vqdsnc.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fnp.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rzd.jinqigfzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tqm.vqdsnc.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gnt.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mzw.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ftw.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yzi.nanxuanxn.top

[D11] 反转数组
来源：http://rzs.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://phc.yj20258888.top

PHP:  array_reverse($arr);
来源：http://khg.ppjwa.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uix.andypj.xyz

TS:   [...arr].reverse();
来源：http://xkg.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://oap.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://mqt.zhiwuduotai.top

Ruby: arr.reverse
来源：http://zwz.hysaishi.cn

C#:   list.Reverse();
来源：http://gnu.fzhhl.top

[D12] 查找元素下标
来源：http://wqu.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://ftu.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cae.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lgn.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yva.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://idg.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://kzv.zdqjudy.top

Ruby: arr.index(x)
来源：http://vzp.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://hoi.feifeiyinyue.top

[D13] 过滤（保留满足条件的）
来源：http://seh.9152youxi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mwy.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eic.aizwys.cn

JS:   arr.filter(x => x > 3)
来源：http://nsy.hongshengwenyu.top

TS:   arr.filter(x => x > 3)
来源：http://ocw.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qth.tarul.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vvg.tanke756.top

Ruby: arr.select { |x| x > 3 }
来源：http://nfe.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rss.shangyingyoupin.top

[D14] 映射转换（每个元素变形）
来源：http://qqu.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kgj.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aua.jinghuilouyu.cn

JS:   arr.map(x => x * 2)
来源：http://vmd.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://emh.xinyue.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://uad.ybcxt.top

Go:   // 手写循环
来源：http://gyn.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bkt.fehbvm.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lzm.guowangkeji.top

[D15] 去重
来源：http://xvz.hcnkem.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dkf.yueranfly.top

PHP:  array_unique($arr);
来源：http://meo.cheryme.top

JS:   [...new Set(arr)]
来源：http://imn.pycfn.com

TS:   [...new Set(arr)]
来源：http://rvp.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rsq.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://gcy.yvedp.cn

Ruby: arr.uniq
来源：http://sfv.ivvv.top

C#:   list.Distinct().ToList()
来源：http://zcw.jqgfzy.top

[D16] 求和与平均值
来源：http://ghs.ywan-chungtsiang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xao.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vgb.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://scu.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lsc.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ufx.bjfxy.top

Go:   // 手写循环累加
来源：http://lob.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ags.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://kyi.ctjpmb.com

[D17] 最大值与最小值
来源：http://adm.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://pzg.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://tpz.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qws.fengsongda.top

TS:   Math.max(...arr);
来源：http://xkp.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wzn.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qri.dianchejie.cn

Ruby: arr.max;  arr.min
来源：http://gfw.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://vju.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://cxc.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mjy.ydjk.org.cn

PHP:  array_merge(...$nested);
来源：http://hoj.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://okh.uphjek.com

TS:   nested.flat();
来源：http://vbh.52xcode.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pub.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://tes.aizwys.cn

Ruby: nested.flatten
来源：http://ldv.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yrk.shuidangran.top

[D19] 按字段分组
来源：http://bzp.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iya.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qmi.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vdd.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ile.nanxuanxn.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ttl.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://zdb.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jjk.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ujj.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://skx.bjfxy.top

Py:   Counter(arr)
来源：http://tur.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://udw.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ift.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qqp.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hst.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://hrr.hfpthk.cn

Ruby: arr.tally
来源：http://cke.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rjj.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://dtk.shanyushiyangkeji.top

Py:   x in arr
来源：http://zkq.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://guw.ydzc1.top

JS:   arr.includes(x)
来源：http://gmb.zhongyouzk.top

TS:   arr.includes(x)
来源：http://unw.guannengcc.top

Java: list.contains(x)
来源：http://oes.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://xiz.wangdashe.top

Ruby: arr.include?(x)
来源：http://vmv.nwbrower.top

C#:   list.Contains(x)
来源：http://pwc.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://afi.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hsn.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://amt.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qzm.havefunace.top

TS:   [...arr];
来源：http://hea.mhx1999.top

Java: new ArrayList<>(list);
来源：http://rxq.dashuyun.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vfn.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://fhj.zhoulong.xyz

C#:   new List<int>(list);
来源：http://lgw.yueranfly.top

[D23] reduce 累积计算
来源：http://gvc.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gra.jlsjyb.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yqw.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuu.hesvh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://izl.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fhi.gaohongyu789.top

Go:   // 手写循环
来源：http://odn.dianchejie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tbh.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mwb.yj20258.top

[D24] 字典 / Map 基本操作
来源：http://agk.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bya.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fyh.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://amn.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://imj.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://djp.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mav.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lwq.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hdr.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://mgb.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xrn.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rgo.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ezh.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aoc.zycfv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://leq.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vcg.ydzc1.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xbi.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rvf.tarul.cn

[D26] 数组转字符串
来源：http://gsy.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://gge.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://rym.yuxming.cn

JS:   arr.join(", ")
来源：http://wvn.kuanghao11.cn

TS:   arr.join(", ")
来源：http://mnp.cdnleiting.top

Java: String.join(", ", list)
来源：http://iit.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://ray.guannengcc.top

Ruby: arr.join(", ")
来源：http://vfo.iojbl.cn

C#:   string.Join(", ", list)
来源：http://frx.jinqigfzy.top

================================================================================
来源：http://vip.hammf.cn

E. 字符串处理
来源：http://cxx.zdbjq.cn

================================================================================
来源：http://nwd.tian-w.cn

[E01] 拼接字符串
来源：http://qgo.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xdc.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rfn.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bec.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gtq.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eqc.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fyn.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://arx.cucudq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wyd.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://hlp.yuanzhike.top

Py:   "ab" * 3
来源：http://pio.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://elm.andypj.xyz

JS:   "ab".repeat(3)
来源：http://yeu.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://xpu.yangfankeji.com

Java: "ab".repeat(3)
来源：http://tqn.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://pyb.redwolf501.top

Ruby: "ab" * 3
来源：http://wil.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xkc.dashuyun.cn

[E03] 截取子串
来源：http://sjg.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xby.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dtb.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://btj.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://tik.ehwqpu.com

Java: s.substring(1, 4)
来源：http://iid.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dws.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://puu.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://khb.ydzc1.top

[E04] 查找子串位置
来源：http://tor.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://ubj.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://bqd.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pjb.yangfankeji.com

TS:   s.indexOf("x")
来源：http://llj.havefunace.top

Java: s.indexOf("x")
来源：http://nls.sysykeji.top


<!-- 参考信息 -->