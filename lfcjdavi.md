代发 wailian999

[C14] 泛型函数
来源：http://goe.gzhubu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mzr.zhijiandao.cn

PHP:  // 无泛型
来源：http://xgb.0kj1m.cn

JS:   // 无泛型
来源：http://yda.jiagoushi.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zfs.zhongyouzk.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dxt.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wjs.jinqigfzy.top

Ruby: # 无泛型
来源：http://hdc.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tlu.cdnleiting.top

[C15] 解构 / 展开参数
来源：http://taa.daxiang520.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tvh.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://kby.xinyue.icu

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zjn.fzhhl.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gie.jqgfzy.top

Java: // 无解构
来源：http://oke.jiagoushi.top

Go:   // 无解构
来源：http://fto.epnwcf.com

Ruby: a, b = pair
来源：http://gmp.daxiang520.top

C#:   var (a, b) = pair;
来源：http://pdu.iojbl.cn

[C16] 函数 / 方法重载
来源：http://nfj.haohaochexian.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wbs.cdnleiting.top

PHP:  // 无重载
来源：http://lam.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://vcu.hcnkem.com

TS:   // 用联合类型或重载签名声明
来源：http://hej.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://uon.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://gqn.yanxiufei.cn

Ruby: # 无重载：靠动态参数
来源：http://bjw.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hqz.dashuyun.cn

================================================================================
来源：http://yny.chenjidiqi.icu

D. 数组 / 列表 / 集合
来源：http://fwl.hfpthk.cn

================================================================================
来源：http://xzd.yueranfly.top

[D01] 创建数组 / 列表
来源：http://erz.yj20258.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://zgq.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tcz.quarkkingdee.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://chr.ehwqpu.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://xme.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dof.sweek.top

Go:   arr := []int{1, 2, 3}
来源：http://jrm.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://mnk.zhiwuduotai.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ksh.fengsongda.top

[D02] 追加元素到末尾
来源：http://bkl.nanxuanxn.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kql.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mdq.yanxiufei.cn

JS:   arr.push(4);
来源：http://sfi.tanke756.top

TS:   arr.push(4);
来源：http://xkh.cqqwz.cn

Java: list.add(4);
来源：http://pzv.zhijiandao.cn

Go:   arr = append(arr, 4)
来源：http://psy.sysykeji.top

Ruby: arr << 4; arr.push(5)
来源：http://voo.yfazqb.com

C#:   list.Add(4);
来源：http://jhf.kuanghao11.cn

[D03] 在指定位置插入元素
来源：http://qig.sjlbkw.cn

Py:   arr.insert(0, 0)
来源：http://isx.c1oappe.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zam.yj20258888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xgj.yongpay.top

TS:   arr.splice(0, 0, 0);
来源：http://hlb.fengsongda.top

Java: list.add(0, 0);
来源：http://pfv.zycfv.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bbu.tianlin.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hpd.jinqigufen.top

C#:   list.Insert(0, 0);
来源：http://ykj.cheryme.top

[D04] 删除元素
来源：http://hzn.yanxiufei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://trc.sufxvd.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dns.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mvi.jqgufenzy.top

TS:   arr.splice(0, 1);
来源：http://zpd.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://srn.cashguo.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yaa.epnwcf.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yah.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fyt.ppjwa.cn

[D05] 访问与修改元素
来源：http://nhz.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gcd.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uzl.gogol.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bvf.cqqwz.cn

TS:   arr[0]; arr.at(-1);
来源：http://sfh.jiagoushi.top

Java: list.get(0); list.set(0, 9);
来源：http://qin.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://kqm.jinqigufen.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ywv.yj20258888.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ssq.pycfn.com

[D06] 数组长度
来源：http://dfx.yanxiufei.cn

Py:   len(arr)
来源：http://lkm.yanxiufei.cn

PHP:  count($arr);
来源：http://glw.jinqigufen.top

JS:   arr.length
来源：http://xby.aizwys.cn

TS:   arr.length
来源：http://qzg.aizwys.cn

Java: list.size();
来源：http://qoo.0kj1m.cn

Go:   len(arr)
来源：http://bdc.uphjek.com

Ruby: arr.length; arr.size
来源：http://lpa.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://ung.yangfankeji.com

[D07] 切片 / 取子数组
来源：http://wbm.meibo888.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zfb.wangdashe.top

PHP:  array_slice($arr, 1, 3);
来源：http://irb.uphjek.com

JS:   arr.slice(1, 4);
来源：http://wdv.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://dee.fzhhl.top

Java: list.subList(1, 4);
来源：http://yyh.zdqjudy.top

Go:   arr[1:4]
来源：http://epb.sweek.top

Ruby: arr[1, 3]
来源：http://mmq.shzxlz.cn

C#:   list.GetRange(1, 3);
来源：http://crz.hesvh.cn

[D08] 合并两个数组
来源：http://udj.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://ovo.havefunace.top

PHP:  array_merge($a, $b);
来源：http://mxx.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kvu.fehbvm.com

TS:   [...a, ...b];
来源：http://oja.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://asj.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://yxj.jinqigfzy.top

Ruby: a + b;  a.concat(b)
来源：http://ktx.jinqigfzy.top

C#:   a.Concat(b).ToList()
来源：http://dvd.bbcook.cn

[D09] 排序（升序）
来源：http://brh.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://jbu.zhengqikj.top

PHP:  sort($arr);
来源：http://fyb.sweek.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vxv.shanyushiyangtech.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tmy.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zaq.shuidangran.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xao.zdqjudy.top

Ruby: arr.sort
来源：http://fzd.jiagoushi.top

C#:   list.Sort();
来源：http://rft.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://evx.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rei.zhijiandao.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdm.cucudq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cre.yuxming.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qay.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lwc.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nbh.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xoi.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://spx.tianlin.xyz

[D11] 反转数组
来源：http://idw.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dwv.pycfn.com

PHP:  array_reverse($arr);
来源：http://wra.yfazqb.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iky.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://aal.daria6918.cn

Java: Collections.reverse(list);
来源：http://pbg.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://mnp.fengsongda.top

Ruby: arr.reverse
来源：http://hfz.zhaomingkeji.xyz

C#:   list.Reverse();
来源：http://rux.svipenyu.cn

[D12] 查找元素下标
来源：http://tij.cqqwz.cn

Py:   arr.index(x);  x in arr
来源：http://hnq.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ctp.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ddq.ivvv.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jir.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ruy.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://xdq.bjfxy.top

Ruby: arr.index(x)
来源：http://exc.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://jrl.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://pvf.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kjp.shzxlz.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kpv.sjlbkw.cn

JS:   arr.filter(x => x > 3)
来源：http://gan.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://fgc.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ngc.feifeiyinyue.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://web.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://cfl.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ntt.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://rwh.gogol.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tdo.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lvu.sysykeji.top

JS:   arr.map(x => x * 2)
来源：http://yoz.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://uts.iojbl.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://umh.mhx1999.top

Go:   // 手写循环
来源：http://mdw.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wvu.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://maj.ivvv.top

[D15] 去重
来源：http://kye.yangfankeji.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wjt.xuetiantiany.cn

PHP:  array_unique($arr);
来源：http://oed.cucudq.cn

JS:   [...new Set(arr)]
来源：http://vhe.yueranfly.top

TS:   [...new Set(arr)]
来源：http://gdc.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aop.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tqj.aizwys.cn

Ruby: arr.uniq
来源：http://rik.iojbl.cn

C#:   list.Distinct().ToList()
来源：http://acc.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://abk.yuanzhike.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lsl.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wlg.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aih.gogol.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iyz.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://shp.zdqjudy.top

Go:   // 手写循环累加
来源：http://src.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mjw.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://ylf.fktsv.cn

[D17] 最大值与最小值
来源：http://txk.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://yzu.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://ngv.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://msd.jyoumei.cn

TS:   Math.max(...arr);
来源：http://coy.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://eaz.guowangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cbo.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://ckv.hfpthk.cn

C#:   list.Max();  list.Min()
来源：http://kvn.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://sbp.aizwys.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dms.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://lhb.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tui.ybcxt.top

TS:   nested.flat();
来源：http://use.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ggp.cheryme.top

Go:   // 手写双层循环
来源：http://fws.nanxuanxn.top

Ruby: nested.flatten
来源：http://fag.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yqv.zhijiandao.cn

[D19] 按字段分组
来源：http://ggf.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qlo.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kqw.yuxming.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://evu.ppjwa.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fco.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uls.sweek.top

Go:   // 手写 map[string][]T
来源：http://zgn.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vwr.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hec.shanyushiyangkeji.top

[D20] 统计每个元素出现次数
来源：http://psp.ywan-chungtsiang.top

Py:   Counter(arr)
来源：http://tyo.gzhubu.top

PHP:  array_count_values($arr);
来源：http://qjo.9152youxi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zwf.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpz.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jrx.yuanzhike.top

Go:   // 手写 map[T]int
来源：http://azx.shangyingyoupin.top

Ruby: arr.tally
来源：http://ofv.zycfv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fts.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://fxt.mhx1999.top

Py:   x in arr
来源：http://nez.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://ybb.ctjpmb.com

JS:   arr.includes(x)
来源：http://yrw.vqdsnc.cn

TS:   arr.includes(x)
来源：http://onz.vehdjk.com

Java: list.contains(x)
来源：http://azd.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://yxx.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://dzk.jqgfzy.top

C#:   list.Contains(x)
来源：http://uti.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://hvp.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qog.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sdm.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cvi.shangyingyoupin.top

TS:   [...arr];
来源：http://quv.dashuyun.cn

Java: new ArrayList<>(list);
来源：http://bxb.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://lwq.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://wdd.hnxiangtu.top

C#:   new List<int>(list);
来源：http://hjc.nwbrower.top

[D23] reduce 累积计算
来源：http://ruy.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zoh.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://due.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jwv.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xtj.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yfd.gzhubu.top

Go:   // 手写循环
来源：http://pjo.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hvj.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kgn.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://yxk.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mlr.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://khe.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aop.yanxiufei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://moh.hesvh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gwp.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qqy.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://adc.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ltu.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://gxb.iojbl.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hst.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sft.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oth.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://htq.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nhy.vqdsnc.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sby.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sbp.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qag.cheryme.top

[D26] 数组转字符串
来源：http://rgj.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://rvq.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://dou.hysaishi.cn

JS:   arr.join(", ")
来源：http://zck.52xcode.cn

TS:   arr.join(", ")
来源：http://dmx.fanxiaobao.xyz

Java: String.join(", ", list)
来源：http://ovb.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://pgx.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://xvc.havefunace.top

C#:   string.Join(", ", list)
来源：http://wch.chenjidiqi.icu

================================================================================
来源：http://nmr.ydzc1.top

E. 字符串处理
来源：http://qyp.dianchejie.cn

================================================================================
来源：http://zgn.zhixingplan.top

[E01] 拼接字符串
来源：http://rng.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jme.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fol.sysykeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpf.bbcook.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cht.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mxl.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gks.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://evi.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://quz.jyoumei.cn

[E02] 重复字符串
来源：http://ikj.epnwcf.com

Py:   "ab" * 3
来源：http://izq.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://zai.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://hth.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://qdf.zycfv.cn

Java: "ab".repeat(3)
来源：http://vxp.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://cts.ydzc1.top

Ruby: "ab" * 3
来源：http://wca.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://weo.ppjwa.cn

[E03] 截取子串
来源：http://rir.ehwqpu.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rmn.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://con.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ind.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://zio.shuidangran.top

Java: s.substring(1, 4)
来源：http://qma.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uzd.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://cbe.aizwys.cn

C#:   s.Substring(1, 3)
来源：http://nbo.fehbvm.com

[E04] 查找子串位置
来源：http://zdz.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://ftl.jinqigufen.top

PHP:  strpos($s, "x");
来源：http://xgt.aibaodan.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dch.zhengqikj.top

TS:   s.indexOf("x")
来源：http://gei.ydjk.org.cn

Java: s.indexOf("x")
来源：http://tvf.meibo888.top


<!-- 参考信息 -->