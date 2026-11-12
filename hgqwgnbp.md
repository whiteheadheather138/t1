代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vyd.xingfuxueyuan.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kvp.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://afx.gzhubu.top

Ruby: # 无泛型
来源：http://vaa.zhoulong.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xnp.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://vej.dashuyun.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fhy.zdbjq.cn

PHP:  [$a, $b] = $pair;
来源：http://esn.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hiy.cheryme.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hha.cashguo.top

Java: // 无解构
来源：http://cqw.jlsjyb.cn

Go:   // 无解构
来源：http://gxp.fanxiaobao.xyz

Ruby: a, b = pair
来源：http://vqh.xinyue.icu

C#:   var (a, b) = pair;
来源：http://byq.zycfv.cn

[C16] 函数 / 方法重载
来源：http://duj.aibaodan.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qoh.quarkkingdee.top

PHP:  // 无重载
来源：http://plx.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yrv.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://ciw.zhixingplan.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qhr.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://ruf.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://qyc.pengpengdd.cyou

C#:   void F(int a) {}  void F(string a) {}
来源：http://zhf.sufxvd.cn

================================================================================
来源：http://wmr.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://ilo.guannengcc.top

================================================================================
来源：http://gqo.jianghu66.top

[D01] 创建数组 / 列表
来源：http://iro.yueranfly.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://rsn.xziqi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sjm.jqgfzy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bvb.hfpthk.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dzz.tian-w.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vcb.dianchejie.cn

Go:   arr := []int{1, 2, 3}
来源：http://bbn.hfpthk.cn

Ruby: arr = [1, 2, 3]
来源：http://mmi.hongshengwenyu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://scc.uphjek.com

[D02] 追加元素到末尾
来源：http://khp.shuidangran.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zqj.vehdjk.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nnq.pycfn.com

JS:   arr.push(4);
来源：http://wyj.andypj.xyz

TS:   arr.push(4);
来源：http://kfo.svipenyu.cn

Java: list.add(4);
来源：http://qjc.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://eie.smart0.xyz

Ruby: arr << 4; arr.push(5)
来源：http://qga.xinyue.icu

C#:   list.Add(4);
来源：http://bhn.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://nfu.52xcode.cn

Py:   arr.insert(0, 0)
来源：http://boc.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://piq.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iok.hnqzz.top

TS:   arr.splice(0, 0, 0);
来源：http://wmb.uphjek.com

Java: list.add(0, 0);
来源：http://saf.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://lda.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://tfx.jqgfzy.top

C#:   list.Insert(0, 0);
来源：http://out.xuanzx.com

[D04] 删除元素
来源：http://zth.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yki.hongshengwenyu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zqy.yuxming.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://los.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://ckj.yuxming.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zxo.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://evq.cheryme.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tew.hcnkem.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qlq.cheryme.top

[D05] 访问与修改元素
来源：http://otf.chenlongwang.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eox.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lka.gaohongyu789.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dut.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://tgp.zhengqikj.top

Java: list.get(0); list.set(0, 9);
来源：http://qod.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://mtq.chenjidiqi.icu

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://neu.wangdashe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://buq.gogol.net.cn

[D06] 数组长度
来源：http://zia.daria6918.cn

Py:   len(arr)
来源：http://kfx.xylfe.cn

PHP:  count($arr);
来源：http://mka.kuanghao11.cn

JS:   arr.length
来源：http://xqf.feifeiyinyue.top

TS:   arr.length
来源：http://jin.zhiwuduotai.top

Java: list.size();
来源：http://hjl.0kj1m.cn

Go:   len(arr)
来源：http://epv.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://vyv.ydjk.org.cn

C#:   list.Count;
来源：http://cud.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://dxu.jianghu66.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qrm.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iox.fktsv.cn

JS:   arr.slice(1, 4);
来源：http://biv.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://gga.yueranfly.top

Java: list.subList(1, 4);
来源：http://rcc.guowangkeji.top

Go:   arr[1:4]
来源：http://pan.yj202588.top

Ruby: arr[1, 3]
来源：http://fol.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://sou.quarkkingdee.top

[D08] 合并两个数组
来源：http://jsx.hongshengwenyu.top

Py:   a + b;  a.extend(b)
来源：http://qzt.yj202588.top

PHP:  array_merge($a, $b);
来源：http://egt.gotoacloud.top

JS:   [...a, ...b];  a.concat(b);
来源：http://odf.ywan-chungtsiang.top

TS:   [...a, ...b];
来源：http://qec.nanxinkj.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zrh.uphjek.com

Go:   append(a, b...)
来源：http://xef.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://olr.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://mjz.yangfankeji.com

[D09] 排序（升序）
来源：http://iio.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://hoe.tian-w.cn

PHP:  sort($arr);
来源：http://dvv.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kvd.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zrl.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dey.ybcxt.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ett.zhongyouzk.top

Ruby: arr.sort
来源：http://swq.zdqjudy.top

C#:   list.Sort();
来源：http://owt.cqqwz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qhk.hnqzz.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qll.hysaishi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vtd.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://khg.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rpr.yfazqb.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://iap.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iej.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kyn.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rss.yuanzhike.top

[D11] 反转数组
来源：http://wwv.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://nib.jqgfzy.top

PHP:  array_reverse($arr);
来源：http://dsc.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cra.yonumen.top

TS:   [...arr].reverse();
来源：http://fyg.c1oappe.top

Java: Collections.reverse(list);
来源：http://xpb.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://wof.yongpay.top

Ruby: arr.reverse
来源：http://khg.shanyushiyangkeji.top

C#:   list.Reverse();
来源：http://xsn.mhx1999.top

[D12] 查找元素下标
来源：http://ckj.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://pvc.ivvv.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://krb.redwolf501.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzn.sysykeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xof.shangyingyoupin.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hrr.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://ujn.tarul.cn

Ruby: arr.index(x)
来源：http://wcf.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://wwl.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://jfo.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://otp.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qdo.zhijiandao.cn

JS:   arr.filter(x => x > 3)
来源：http://fvs.zhaomingkeji.xyz

TS:   arr.filter(x => x > 3)
来源：http://lgw.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bfh.vqdsnc.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oym.jinyuanbaomall.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bxl.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://evo.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://iad.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gsf.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jzq.cucudq.cn

JS:   arr.map(x => x * 2)
来源：http://vln.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://ypk.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://adi.fengsongda.top

Go:   // 手写循环
来源：http://zlr.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://nyt.yanxiufei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ksa.bbcook.cn

[D15] 去重
来源：http://iwl.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dkk.birdmap.top

PHP:  array_unique($arr);
来源：http://ltp.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://hkm.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://ryv.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tor.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://wfi.aizwys.cn

Ruby: arr.uniq
来源：http://lng.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://eht.yj20258888.top

[D16] 求和与平均值
来源：http://pub.yj20258.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ahd.nanxuanxn.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://deg.fanxiaobao.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ccr.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pmr.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aoj.ppjwa.cn

Go:   // 手写循环累加
来源：http://sqv.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vfc.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://fug.bjfxy.top

[D17] 最大值与最小值
来源：http://qig.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://qrt.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://ijo.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vck.yfazqb.com

TS:   Math.max(...arr);
来源：http://zfo.hongshengwenyu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dyp.shanyushiyangkeji.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oua.uphjek.com

Ruby: arr.max;  arr.min
来源：http://afr.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://xzz.hammf.cn

[D18] 扁平化嵌套数组
来源：http://ymo.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fzx.yj202588.top

PHP:  array_merge(...$nested);
来源：http://vxa.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mwz.ybcxt.top

TS:   nested.flat();
来源：http://rwo.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxi.daria6918.cn

Go:   // 手写双层循环
来源：http://bus.tian-w.cn

Ruby: nested.flatten
来源：http://ucg.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://oyy.cdnleiting.top

[D19] 按字段分组
来源：http://yqm.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://elg.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lwz.hysaishi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jfl.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jpr.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qyp.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://ldn.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pxq.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mib.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://pjq.haohaochexian.top

Py:   Counter(arr)
来源：http://zgt.tarul.cn

PHP:  array_count_values($arr);
来源：http://rep.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qsn.guowangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fvr.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gev.zhijiandao.cn

Go:   // 手写 map[T]int
来源：http://qrh.jqgfzy.top

Ruby: arr.tally
来源：http://pws.tanke756.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rbk.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://vtm.tarul.cn

Py:   x in arr
来源：http://sxl.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://nal.fehbvm.com

JS:   arr.includes(x)
来源：http://afk.haohaochexian.top

TS:   arr.includes(x)
来源：http://thb.ctjpmb.com

Java: list.contains(x)
来源：http://bke.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://uht.yj20258888.top

Ruby: arr.include?(x)
来源：http://dvr.redwolf501.top

C#:   list.Contains(x)
来源：http://dnd.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://gea.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sng.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vaf.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rja.yuxming.cn

TS:   [...arr];
来源：http://ovd.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://cri.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tbm.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://xsm.bjfxy.top

C#:   new List<int>(list);
来源：http://qpa.snrcjt.cn

[D23] reduce 累积计算
来源：http://afb.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://amk.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vaf.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://szh.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpj.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://smt.aizwys.cn

Go:   // 手写循环
来源：http://vcf.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wre.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iee.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://wcl.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ypu.tianlin.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tmv.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lsg.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xza.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hlk.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ode.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kym.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wvt.nanxuanxn.top

[D25] Set 集合去重与交并差
来源：http://cjn.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qqu.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://meu.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jla.fzhhl.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wjh.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oux.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pst.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qjv.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pvs.shuidangran.top

[D26] 数组转字符串
来源：http://mgy.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://rhk.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://moh.cucudq.cn

JS:   arr.join(", ")
来源：http://yxl.chenlongwang.top

TS:   arr.join(", ")
来源：http://sto.yj202588.top

Java: String.join(", ", list)
来源：http://esa.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://dju.ydzc1.top

Ruby: arr.join(", ")
来源：http://cvd.c1oappe.top

C#:   string.Join(", ", list)
来源：http://ofv.zdqjudy.top

================================================================================
来源：http://rrp.hywenlv.cn

E. 字符串处理
来源：http://afo.daria6918.cn

================================================================================
来源：http://uor.yj20258.top

[E01] 拼接字符串
来源：http://grd.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ucw.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://arb.hywenlv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sua.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dlw.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wos.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gtv.yfazqb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ilx.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ajs.hesvh.cn

[E02] 重复字符串
来源：http://iwc.hnqzz.top

Py:   "ab" * 3
来源：http://bab.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://sjk.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://dqj.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://krf.uphjek.com

Java: "ab".repeat(3)
来源：http://inf.zhongyouzk.top

Go:   strings.Repeat("ab", 3)
来源：http://adf.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://xdh.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uwy.ydjk.org.cn

[E03] 截取子串
来源：http://xly.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://khx.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bjg.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gyq.hysaishi.cn

TS:   s.slice(1, 4)
来源：http://lqt.jinyuanbaomall.cn

Java: s.substring(1, 4)
来源：http://taq.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://omu.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hoh.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://rfg.jianghu66.top

[E04] 查找子串位置
来源：http://nrs.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://ctf.yj202588.top

PHP:  strpos($s, "x");
来源：http://wpn.0kj1m.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://voq.redwolf501.top

TS:   s.indexOf("x")
来源：http://xxh.jlsjyb.cn

Java: s.indexOf("x")
来源：http://qmo.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://fnw.hnqzz.top

Ruby: s.index("x")
来源：http://akh.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://epc.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zzq.gogol.net.cn


<!-- 参考信息 -->