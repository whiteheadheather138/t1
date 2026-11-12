代发 wailian999

[C14] 泛型函数
来源：http://wsq.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://npj.xinyue.icu

PHP:  // 无泛型
来源：http://wdt.hnqzz.top

JS:   // 无泛型
来源：http://bvo.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jsm.52xcode.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rzx.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eyr.iojbl.cn

Ruby: # 无泛型
来源：http://qdm.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ctt.jinqigufen.top

[C15] 解构 / 展开参数
来源：http://twx.fktsv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xzd.hesvh.cn

PHP:  [$a, $b] = $pair;
来源：http://ojx.jyoumei.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rvn.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://guy.jinghuilouyu.cn

Java: // 无解构
来源：http://wxf.jinqigfzy.top

Go:   // 无解构
来源：http://kfc.tian-w.cn

Ruby: a, b = pair
来源：http://djc.bbcook.cn

C#:   var (a, b) = pair;
来源：http://fnb.xinyue.icu

[C16] 函数 / 方法重载
来源：http://tug.hongshengwenyu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zmg.shangyingyoupin.top

PHP:  // 无重载
来源：http://kdr.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vre.shzxlz.cn

TS:   // 用联合类型或重载签名声明
来源：http://wvf.wangshuangyany.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sty.kuanghao11.cn

Go:   // 无重载：用不同函数名
来源：http://qpn.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://kio.cheryme.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ggs.yj202588.top

================================================================================
来源：http://idt.cashguo.top

D. 数组 / 列表 / 集合
来源：http://dak.meibo888.top

================================================================================
来源：http://sjt.aizwys.cn

[D01] 创建数组 / 列表
来源：http://ovh.dianchejie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ksn.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vch.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iob.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mcw.zycfv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gzd.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://lpk.0kj1m.cn

Ruby: arr = [1, 2, 3]
来源：http://xum.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://poq.nanxuanxn.top

[D02] 追加元素到末尾
来源：http://fux.fengsongda.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dky.yongpay.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dfe.cashguo.top

JS:   arr.push(4);
来源：http://spl.ivvv.top

TS:   arr.push(4);
来源：http://ljl.xylfe.cn

Java: list.add(4);
来源：http://rdw.guowangkeji.top

Go:   arr = append(arr, 4)
来源：http://xoo.yueranfly.top

Ruby: arr << 4; arr.push(5)
来源：http://lna.svipenyu.cn

C#:   list.Add(4);
来源：http://yvk.xziqi.cn

[D03] 在指定位置插入元素
来源：http://qcw.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://clg.zdqjudy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zca.zdqjudy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blm.nanxuanxn.top

TS:   arr.splice(0, 0, 0);
来源：http://ldg.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://nzu.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://vzi.sxryk.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gag.xuetiantiany.cn

C#:   list.Insert(0, 0);
来源：http://glv.zhiwuduotai.top

[D04] 删除元素
来源：http://xfp.yfazqb.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hup.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://znd.nanxinkj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nug.cqqwz.cn

TS:   arr.splice(0, 1);
来源：http://gkb.yuanzhike.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://flf.yongpay.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rvc.svipenyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://csf.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rln.zhaomingkeji.xyz

[D05] 访问与修改元素
来源：http://tee.sufxvd.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gzv.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ecp.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://odj.tianlin.xyz

TS:   arr[0]; arr.at(-1);
来源：http://xmm.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://msa.snrcjt.cn

Go:   arr[0]; arr[0] = 9
来源：http://jan.316326.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vyb.cdnleiting.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lgs.yanxiufei.cn

[D06] 数组长度
来源：http://nre.316326.xyz

Py:   len(arr)
来源：http://ofg.vqdsnc.cn

PHP:  count($arr);
来源：http://nls.sxryk.cn

JS:   arr.length
来源：http://unm.hongshengwenyu.top

TS:   arr.length
来源：http://trd.yuanzhike.top

Java: list.size();
来源：http://shn.jinyuanbaomall.cn

Go:   len(arr)
来源：http://oyf.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://kkd.ydzc1.top

C#:   list.Count;
来源：http://hde.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://otj.cqqwz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rwf.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gjj.nwbrower.top

JS:   arr.slice(1, 4);
来源：http://jao.hammf.cn

TS:   arr.slice(1, 4);
来源：http://doy.yj20258888.top

Java: list.subList(1, 4);
来源：http://ctp.yonumen.top

Go:   arr[1:4]
来源：http://jsh.yfazqb.com

Ruby: arr[1, 3]
来源：http://ajj.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://cgd.tianlin.xyz

[D08] 合并两个数组
来源：http://uqj.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://xyq.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://rmf.yonumen.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wjz.tanke756.top

TS:   [...a, ...b];
来源：http://zrn.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gga.zhijiandao.cn

Go:   append(a, b...)
来源：http://ljl.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://nqd.gaohongyu789.top

C#:   a.Concat(b).ToList()
来源：http://ujj.sysykeji.top

[D09] 排序（升序）
来源：http://mig.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://plv.shzxlz.cn

PHP:  sort($arr);
来源：http://bzk.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://upz.havefunace.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://nef.cheryme.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wet.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://duj.sysykeji.top

Ruby: arr.sort
来源：http://niz.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://eum.andypj.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://epx.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xoq.zdbjq.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vin.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cuu.guowangkeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zit.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iff.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nrh.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cei.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tqr.hywenlv.cn

[D11] 反转数组
来源：http://ojq.yj20258888.top

Py:   arr[::-1];  arr.reverse()
来源：http://qum.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://lxi.ywan-chungtsiang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nxu.kuanghao11.cn

TS:   [...arr].reverse();
来源：http://rzr.pycfn.com

Java: Collections.reverse(list);
来源：http://stn.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://zsl.9152youxi.cn

Ruby: arr.reverse
来源：http://mat.wangshuangyany.cn

C#:   list.Reverse();
来源：http://knl.tian-w.cn

[D12] 查找元素下标
来源：http://nyr.shzxlz.cn

Py:   arr.index(x);  x in arr
来源：http://uqg.cucudq.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zgo.daria6918.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nav.xinyue.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zlv.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gqf.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://asp.andypj.xyz

Ruby: arr.index(x)
来源：http://ell.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://uiu.hnqzz.top

[D13] 过滤（保留满足条件的）
来源：http://nta.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iop.hnqzz.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://emz.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://hyg.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://xot.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fex.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eby.cucudq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zvh.xinyue.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://odv.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://nye.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dft.pengpengdd.cyou

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hzg.yvedp.cn

JS:   arr.map(x => x * 2)
来源：http://coe.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://gar.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sty.iojbl.cn

Go:   // 手写循环
来源：http://kdl.fengsongda.top

Ruby: arr.map { |x| x * 2 }
来源：http://cjj.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jmc.cdnleiting.top

[D15] 去重
来源：http://vek.wangshuangyany.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cro.yfazqb.com

PHP:  array_unique($arr);
来源：http://hub.uphjek.com

JS:   [...new Set(arr)]
来源：http://zcp.jqgufenzy.top

TS:   [...new Set(arr)]
来源：http://jec.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ktz.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://gke.epnwcf.com

Ruby: arr.uniq
来源：http://qpk.tianlin.xyz

C#:   list.Distinct().ToList()
来源：http://zui.cqqwz.cn

[D16] 求和与平均值
来源：http://jrp.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hsw.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kkf.sjlbkw.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aqy.shuidangran.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vch.yueranfly.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://krs.svipenyu.cn

Go:   // 手写循环累加
来源：http://mcl.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qgo.ydjk.org.cn

C#:   list.Sum();  list.Average()
来源：http://gqy.haohaochexian.top

[D17] 最大值与最小值
来源：http://uvi.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://tej.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://fpq.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cjs.bjfxy.top

TS:   Math.max(...arr);
来源：http://gks.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ooo.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://udj.316326.xyz

Ruby: arr.max;  arr.min
来源：http://clq.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://nzn.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://ghc.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rjc.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://ypn.sweek.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uvo.feifeiyinyue.top

TS:   nested.flat();
来源：http://mwe.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nuz.zhixingplan.top

Go:   // 手写双层循环
来源：http://uej.tian-w.cn

Ruby: nested.flatten
来源：http://frd.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sge.yfazqb.com

[D19] 按字段分组
来源：http://ukh.ywan-chungtsiang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xvc.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://odo.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qgn.yuxming.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lwg.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cps.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://ebj.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://que.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gph.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://cqe.dianchejie.cn

Py:   Counter(arr)
来源：http://sej.jinghuilouyu.cn

PHP:  array_count_values($arr);
来源：http://rbw.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cok.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kie.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xra.sxryk.cn

Go:   // 手写 map[T]int
来源：http://xbw.hcnkem.com

Ruby: arr.tally
来源：http://mkj.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://emu.fzhhl.top

[D21] 判断是否包含某元素
来源：http://fak.vqdsnc.cn

Py:   x in arr
来源：http://skn.9152youxi.cn

PHP:  in_array($x, $arr, true);
来源：http://cmu.zhiwuduotai.top

JS:   arr.includes(x)
来源：http://wxx.ywan-chungtsiang.top

TS:   arr.includes(x)
来源：http://kmo.xinyue.icu

Java: list.contains(x)
来源：http://uxf.jqgfzy.top

Go:   slices.Contains(arr, x)
来源：http://epi.hcnkem.com

Ruby: arr.include?(x)
来源：http://qrb.jinghuilouyu.cn

C#:   list.Contains(x)
来源：http://pge.gogol.net.cn

[D22] 复制数组（避免共享引用）
来源：http://zue.chenjidiqi.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://apk.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nlw.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hyl.bbcook.cn

TS:   [...arr];
来源：http://nmt.sweek.top

Java: new ArrayList<>(list);
来源：http://xvi.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://zzg.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://dxd.52xcode.cn

C#:   new List<int>(list);
来源：http://guc.yongpay.top

[D23] reduce 累积计算
来源：http://szd.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oze.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tlr.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vjf.epnwcf.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ywx.hnqzz.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cul.jinqigufen.top

Go:   // 手写循环
来源：http://pax.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oyu.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nyz.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://ggp.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ssk.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pho.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xgo.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cut.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wzb.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lvu.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://van.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nst.tanke756.top

[D25] Set 集合去重与交并差
来源：http://yll.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://avo.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qse.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iwu.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mtw.jiagoushi.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jol.hcnkem.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://unf.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lrs.xylfe.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sri.yuxming.cn

[D26] 数组转字符串
来源：http://sxa.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://nbg.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://hvt.zhoulong.xyz

JS:   arr.join(", ")
来源：http://dxb.zhengqikj.top

TS:   arr.join(", ")
来源：http://xgf.redwolf501.top

Java: String.join(", ", list)
来源：http://yar.zhijiandao.cn

Go:   strings.Join(strs, ", ")
来源：http://wjx.cashguo.top

Ruby: arr.join(", ")
来源：http://qfj.ivvv.top

C#:   string.Join(", ", list)
来源：http://jop.cucudq.cn

================================================================================
来源：http://sfk.ybcxt.top

E. 字符串处理
来源：http://ady.havefunace.top

================================================================================
来源：http://rhe.ivvv.top

[E01] 拼接字符串
来源：http://twc.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ypj.kuanghao11.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://drs.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ckh.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwr.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mju.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sqc.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cys.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pfb.jyoumei.cn

[E02] 重复字符串
来源：http://qnz.316326.xyz

Py:   "ab" * 3
来源：http://yno.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://piv.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://dra.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://vyn.jinqigufen.top

Java: "ab".repeat(3)
来源：http://xtp.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://akn.xuetiantiany.cn

Ruby: "ab" * 3
来源：http://idg.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zzh.aibaodan.cn

[E03] 截取子串
来源：http://xam.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dnk.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uyh.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://egw.havefunace.top

TS:   s.slice(1, 4)
来源：http://tuv.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://ubk.sweek.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lsa.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sdp.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://dgh.hysaishi.cn

[E04] 查找子串位置
来源：http://rcq.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://lec.yj20258.top

PHP:  strpos($s, "x");
来源：http://awr.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://egb.guowangkeji.top

TS:   s.indexOf("x")
来源：http://mvv.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://yvu.meibo888.top


<!-- 参考信息 -->