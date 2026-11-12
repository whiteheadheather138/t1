代发 wailian999

[C14] 泛型函数
来源：http://lwk.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ibc.nanxinkj.top

PHP:  // 无泛型
来源：http://sml.jinqigufen.top

JS:   // 无泛型
来源：http://byz.smart0.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://awo.zhixingplan.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://qhg.zycfv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nvb.zhijiandao.cn

Ruby: # 无泛型
来源：http://jho.chenjidiqi.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ehl.kuanghao11.cn

[C15] 解构 / 展开参数
来源：http://rxh.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zlj.yj202588.top

PHP:  [$a, $b] = $pair;
来源：http://ryv.hysaishi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pvb.cashguo.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vpt.316326.xyz

Java: // 无解构
来源：http://rlt.zdbjq.cn

Go:   // 无解构
来源：http://kvc.yuanzhike.top

Ruby: a, b = pair
来源：http://dgf.epnwcf.com

C#:   var (a, b) = pair;
来源：http://jmx.yvedp.cn

[C16] 函数 / 方法重载
来源：http://koi.yuanzhike.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mqr.tanke756.top

PHP:  // 无重载
来源：http://onr.zhoulong.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://itp.zhengqikj.top

TS:   // 用联合类型或重载签名声明
来源：http://uhk.zhengqikj.top

Java: void f(int a) {}  void f(String a) {}
来源：http://cuf.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://kji.aizwys.cn

Ruby: # 无重载：靠动态参数
来源：http://ggp.uphjek.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://qvt.jinqigfzy.top

================================================================================
来源：http://aoy.yongpay.top

D. 数组 / 列表 / 集合
来源：http://qpx.daria6918.cn

================================================================================
来源：http://qlp.vehdjk.com

[D01] 创建数组 / 列表
来源：http://afi.52xcode.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://dfk.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ooy.xziqi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ikw.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dya.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rey.yj20258.top

Go:   arr := []int{1, 2, 3}
来源：http://wok.cheryme.top

Ruby: arr = [1, 2, 3]
来源：http://gzh.hesvh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dbd.bjfxy.top

[D02] 追加元素到末尾
来源：http://zko.yonumen.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rlp.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sme.gzhubu.top

JS:   arr.push(4);
来源：http://atf.meibo888.top

TS:   arr.push(4);
来源：http://ipi.sweek.top

Java: list.add(4);
来源：http://emx.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://edz.chenjidiqi.icu

Ruby: arr << 4; arr.push(5)
来源：http://lhw.kuanghao11.cn

C#:   list.Add(4);
来源：http://zmu.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://lst.jqgufenzy.top

Py:   arr.insert(0, 0)
来源：http://sts.ydjk.org.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://khs.ybcxt.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jvm.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://ufp.ehwqpu.com

Java: list.add(0, 0);
来源：http://upb.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://ybp.redwolf501.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vjl.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://iqx.fengsongda.top

[D04] 删除元素
来源：http://pco.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xpa.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jfp.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yfu.pycfn.com

TS:   arr.splice(0, 1);
来源：http://uqx.aizwys.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ewk.sxryk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://csg.dashuyun.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://muz.meibo888.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fat.zhoulong.xyz

[D05] 访问与修改元素
来源：http://moe.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qac.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jhn.andypj.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oee.hongshengwenyu.top

TS:   arr[0]; arr.at(-1);
来源：http://wcn.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://lcp.zhijiandao.cn

Go:   arr[0]; arr[0] = 9
来源：http://vdq.aizwys.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xfl.aizwys.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dwj.jyoumei.cn

[D06] 数组长度
来源：http://zfp.ybcxt.top

Py:   len(arr)
来源：http://ykf.shanyushiyangtech.top

PHP:  count($arr);
来源：http://eak.quarkkingdee.top

JS:   arr.length
来源：http://lhl.fanxiaobao.xyz

TS:   arr.length
来源：http://hbh.yfazqb.com

Java: list.size();
来源：http://moc.fanxiaobao.xyz

Go:   len(arr)
来源：http://rwy.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://khn.ehwqpu.com

C#:   list.Count;
来源：http://img.52xcode.cn

[D07] 切片 / 取子数组
来源：http://asm.daxiang520.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://tzi.c1oappe.top

PHP:  array_slice($arr, 1, 3);
来源：http://yzv.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://hnx.shuidangran.top

TS:   arr.slice(1, 4);
来源：http://hdd.wangshuangyany.cn

Java: list.subList(1, 4);
来源：http://gga.ybcxt.top

Go:   arr[1:4]
来源：http://bcd.hywenlv.cn

Ruby: arr[1, 3]
来源：http://pxv.epnwcf.com

C#:   list.GetRange(1, 3);
来源：http://eei.jianghu66.top

[D08] 合并两个数组
来源：http://ygy.fzhhl.top

Py:   a + b;  a.extend(b)
来源：http://xjn.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://hul.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kue.kuanghao11.cn

TS:   [...a, ...b];
来源：http://zxv.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fvl.sysykeji.top

Go:   append(a, b...)
来源：http://gww.9152youxi.cn

Ruby: a + b;  a.concat(b)
来源：http://pds.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://xig.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://rvo.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://gkq.bjfxy.top

PHP:  sort($arr);
来源：http://bsg.shzxlz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ykf.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pep.meibo888.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ann.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fym.yuanzhike.top

Ruby: arr.sort
来源：http://onq.chenjidiqi.icu

C#:   list.Sort();
来源：http://fjo.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eut.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aar.kuanghao11.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehv.ppjwa.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ksf.yj20258.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tpc.cashguo.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vwg.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://utr.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xgu.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mng.cheryme.top

[D11] 反转数组
来源：http://qck.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://qqb.zhongyouzk.top

PHP:  array_reverse($arr);
来源：http://hpb.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ylf.jiagoushi.top

TS:   [...arr].reverse();
来源：http://szy.yueranfly.top

Java: Collections.reverse(list);
来源：http://ibb.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://bxp.zdqjudy.top

Ruby: arr.reverse
来源：http://rcy.uphjek.com

C#:   list.Reverse();
来源：http://bha.hnxiangtu.top

[D12] 查找元素下标
来源：http://bbi.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://khl.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wbt.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvv.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zjj.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dhw.cashguo.top

Go:   slices.Index(arr, x)
来源：http://hcs.hywenlv.cn

Ruby: arr.index(x)
来源：http://upw.ivvv.top

C#:   list.IndexOf(x);
来源：http://nzr.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://duh.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://swz.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qbb.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://rsb.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://xst.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pva.yj202588.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kbi.andypj.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ofm.shzxlz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uvr.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://rnh.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tpb.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mnp.pycfn.com

JS:   arr.map(x => x * 2)
来源：http://ohv.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://fle.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kva.hcnkem.com

Go:   // 手写循环
来源：http://yne.nanxuanxn.top

Ruby: arr.map { |x| x * 2 }
来源：http://uqa.hongshengwenyu.top

C#:   list.Select(x => x * 2).ToList()
来源：http://jpl.yj202588.top

[D15] 去重
来源：http://xim.sjlbkw.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://neh.xingfuxueyuan.xyz

PHP:  array_unique($arr);
来源：http://jcv.cashguo.top

JS:   [...new Set(arr)]
来源：http://rcg.sweek.top

TS:   [...new Set(arr)]
来源：http://rve.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://atz.daxiang520.top

Go:   // 用 map[T]struct{} 手写
来源：http://vqw.shzxlz.cn

Ruby: arr.uniq
来源：http://iqz.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://lxq.gaohongyu789.top

[D16] 求和与平均值
来源：http://bxa.wangdashe.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lng.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xee.fengsongda.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwk.sjlbkw.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mno.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rcd.guowangkeji.top

Go:   // 手写循环累加
来源：http://vhb.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ogl.jiagoushi.top

C#:   list.Sum();  list.Average()
来源：http://otd.yfazqb.com

[D17] 最大值与最小值
来源：http://wjk.jinghuilouyu.cn

Py:   max(arr);  min(arr)
来源：http://srj.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://tcr.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xqc.yonumen.top

TS:   Math.max(...arr);
来源：http://dfr.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wqv.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sxh.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://iom.hcnkem.com

C#:   list.Max();  list.Min()
来源：http://iyb.andypj.xyz

[D18] 扁平化嵌套数组
来源：http://ebp.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fne.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://tnw.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ipy.jinqigufen.top

TS:   nested.flat();
来源：http://hby.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cpg.shzxlz.cn

Go:   // 手写双层循环
来源：http://olo.aibaodan.cn

Ruby: nested.flatten
来源：http://hey.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ssv.jinyuanbaomall.cn

[D19] 按字段分组
来源：http://skj.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://doa.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://klx.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vcb.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://eut.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ioi.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://nvm.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://enp.daria6918.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ncd.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://nwj.xinyue.icu

Py:   Counter(arr)
来源：http://fcj.yj20258.top

PHP:  array_count_values($arr);
来源：http://xxw.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fbz.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://twr.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qqa.52xcode.cn

Go:   // 手写 map[T]int
来源：http://rcu.hywenlv.cn

Ruby: arr.tally
来源：http://bfl.c1oappe.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gwe.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://ssm.jinghuilouyu.cn

Py:   x in arr
来源：http://lgg.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://ogt.hywenlv.cn

JS:   arr.includes(x)
来源：http://kdz.sjlbkw.cn

TS:   arr.includes(x)
来源：http://sga.gogol.net.cn

Java: list.contains(x)
来源：http://oez.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://whf.cdnleiting.top

Ruby: arr.include?(x)
来源：http://auo.vqdsnc.cn

C#:   list.Contains(x)
来源：http://ztw.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://mcu.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jhb.havefunace.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zbu.ydzc1.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oud.hongshengwenyu.top

TS:   [...arr];
来源：http://mbn.zhixingplan.top

Java: new ArrayList<>(list);
来源：http://hhs.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://int.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://kxn.daxiang520.top

C#:   new List<int>(list);
来源：http://dkd.sjlbkw.cn

[D23] reduce 累积计算
来源：http://hwj.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oqm.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vti.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vlx.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xqq.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ply.haohaochexian.top

Go:   // 手写循环
来源：http://itr.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aau.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dsn.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://tqv.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cry.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://azo.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mru.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fyz.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://olb.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jib.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iyu.guowangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qtt.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://hna.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qid.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://udh.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vfc.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kkv.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wpb.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gsr.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wzl.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vxw.ywan-chungtsiang.top

[D26] 数组转字符串
来源：http://lft.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://miu.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://jsp.hesvh.cn

JS:   arr.join(", ")
来源：http://gwm.redwolf501.top

TS:   arr.join(", ")
来源：http://znl.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://nxk.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://hxs.birdmap.top

Ruby: arr.join(", ")
来源：http://mnp.fktsv.cn

C#:   string.Join(", ", list)
来源：http://qdr.redwolf501.top

================================================================================
来源：http://oqz.yfazqb.com

E. 字符串处理
来源：http://pit.zhixingplan.top

================================================================================
来源：http://ytw.cdnleiting.top

[E01] 拼接字符串
来源：http://cib.snrcjt.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hez.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://owy.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wyz.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jdn.jinghuilouyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dnf.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hag.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://npi.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dck.wangshuangyany.cn

[E02] 重复字符串
来源：http://ykj.zycfv.cn

Py:   "ab" * 3
来源：http://bxz.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://xss.316326.xyz

JS:   "ab".repeat(3)
来源：http://lic.xinyue.icu

TS:   "ab".repeat(3)
来源：http://wcl.cheryme.top

Java: "ab".repeat(3)
来源：http://ysk.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://uji.yuanzhike.top

Ruby: "ab" * 3
来源：http://qsu.havefunace.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tbn.meibo888.top

[E03] 截取子串
来源：http://dit.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://esd.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://idb.sjlbkw.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xsf.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://cjt.hammf.cn

Java: s.substring(1, 4)
来源：http://amu.cheryme.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ixc.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://gyl.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://wfu.chenzaomai.com

[E04] 查找子串位置
来源：http://kbx.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://lbm.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://cmg.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aup.epnwcf.com

TS:   s.indexOf("x")
来源：http://loq.cheryme.top

Java: s.indexOf("x")
来源：http://jra.redwolf501.top


<!-- 参考信息 -->