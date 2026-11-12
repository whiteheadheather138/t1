代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://nnq.guowangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xlq.yueranfly.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://css.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ula.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pbb.yj20258.top

Go:   func add(a, b int) int
来源：http://sby.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://grg.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://pka.bbcook.cn

[C14] 泛型函数
来源：http://vgl.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rzd.aizwys.cn

PHP:  // 无泛型
来源：http://fui.epnwcf.com

JS:   // 无泛型
来源：http://ebu.yuanzhike.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://iki.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kcd.xuanzx.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vta.shangyingyoupin.top

Ruby: # 无泛型
来源：http://ofk.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kxa.ehwqpu.com

[C15] 解构 / 展开参数
来源：http://lcn.hesvh.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dno.jinqigfzy.top

PHP:  [$a, $b] = $pair;
来源：http://flh.bbcook.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dax.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zok.tianlin.xyz

Java: // 无解构
来源：http://jwn.sufxvd.cn

Go:   // 无解构
来源：http://gdv.xziqi.cn

Ruby: a, b = pair
来源：http://mcr.jinghuilouyu.cn

C#:   var (a, b) = pair;
来源：http://jlg.gzhubu.top

[C16] 函数 / 方法重载
来源：http://axt.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wog.jyoumei.cn

PHP:  // 无重载
来源：http://uky.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rjv.ivvv.top

TS:   // 用联合类型或重载签名声明
来源：http://zmd.cucudq.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hlt.gogol.net.cn

Go:   // 无重载：用不同函数名
来源：http://azf.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://mwr.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nzx.hcnkem.com

================================================================================
来源：http://tba.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://ypd.birdmap.top

================================================================================
来源：http://ikj.pycfn.com

[D01] 创建数组 / 列表
来源：http://ejx.316326.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://vzh.zhijiandao.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://unr.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jxk.jinghuilouyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ljx.yj20258888.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mmj.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://ezf.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://jab.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yuy.havefunace.top

[D02] 追加元素到末尾
来源：http://ryc.xuetiantiany.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://eso.cucudq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xiu.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://agr.jqgufenzy.top

TS:   arr.push(4);
来源：http://kmq.tarul.cn

Java: list.add(4);
来源：http://qga.ivvv.top

Go:   arr = append(arr, 4)
来源：http://yuw.316326.xyz

Ruby: arr << 4; arr.push(5)
来源：http://zke.ydjk.org.cn

C#:   list.Add(4);
来源：http://dbr.fanxiaobao.xyz

[D03] 在指定位置插入元素
来源：http://thw.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://qyj.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hcb.316326.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ige.shuidangran.top

TS:   arr.splice(0, 0, 0);
来源：http://rex.chenlongwang.top

Java: list.add(0, 0);
来源：http://vxf.tarul.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hay.vqdsnc.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mgo.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://cva.shanyushiyangtech.top

[D04] 删除元素
来源：http://hsf.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gfr.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nup.nwbrower.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qyd.hesvh.cn

TS:   arr.splice(0, 1);
来源：http://mhp.vqdsnc.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zzy.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rhf.shanyushiyangtech.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tap.shzxlz.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://clh.hywenlv.cn

[D05] 访问与修改元素
来源：http://qyg.aibaodan.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://dck.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zyw.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wsf.zhijiandao.cn

TS:   arr[0]; arr.at(-1);
来源：http://wyp.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://uhb.cheryme.top

Go:   arr[0]; arr[0] = 9
来源：http://kzy.xuanzx.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ehb.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qmd.zhiwuduotai.top

[D06] 数组长度
来源：http://wmj.zhoulong.xyz

Py:   len(arr)
来源：http://qzz.bjfxy.top

PHP:  count($arr);
来源：http://svp.aibaodan.cn

JS:   arr.length
来源：http://pfn.yongpay.top

TS:   arr.length
来源：http://geb.birdmap.top

Java: list.size();
来源：http://ypd.jinqigufen.top

Go:   len(arr)
来源：http://khk.aizwys.cn

Ruby: arr.length; arr.size
来源：http://cxi.ivvv.top

C#:   list.Count;
来源：http://bjs.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://mih.ehwqpu.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uxn.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ggx.meibo888.top

JS:   arr.slice(1, 4);
来源：http://mbh.ydjk.org.cn

TS:   arr.slice(1, 4);
来源：http://qqm.aibaodan.cn

Java: list.subList(1, 4);
来源：http://rcu.jiagoushi.top

Go:   arr[1:4]
来源：http://kyl.nanxinkj.top

Ruby: arr[1, 3]
来源：http://kaa.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://cug.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://nnz.andypj.xyz

Py:   a + b;  a.extend(b)
来源：http://cfp.zdqjudy.top

PHP:  array_merge($a, $b);
来源：http://spq.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ewb.iojbl.cn

TS:   [...a, ...b];
来源：http://qqg.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tgk.zhijiandao.cn

Go:   append(a, b...)
来源：http://cjg.hysaishi.cn

Ruby: a + b;  a.concat(b)
来源：http://vsr.ydjk.org.cn

C#:   a.Concat(b).ToList()
来源：http://vno.hfpthk.cn

[D09] 排序（升序）
来源：http://ohu.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://rfr.havefunace.top

PHP:  sort($arr);
来源：http://dxp.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uzj.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dng.ybcxt.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tmq.yueranfly.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://msz.xylfe.cn

Ruby: arr.sort
来源：http://myi.birdmap.top

C#:   list.Sort();
来源：http://ejz.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://bpe.xingfuxueyuan.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mxk.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lbz.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://koh.chenzaomai.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxo.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uwe.fehbvm.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://exg.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ybb.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jlg.xinyue.icu

[D11] 反转数组
来源：http://hrm.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://bwc.birdmap.top

PHP:  array_reverse($arr);
来源：http://yrh.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hwh.guowangkeji.top

TS:   [...arr].reverse();
来源：http://zhm.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://clk.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://wkf.nwbrower.top

Ruby: arr.reverse
来源：http://xqq.daxiang520.top

C#:   list.Reverse();
来源：http://cpq.pycfn.com

[D12] 查找元素下标
来源：http://zil.mhx1999.top

Py:   arr.index(x);  x in arr
来源：http://qis.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://npp.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kva.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lqd.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nlr.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://vsy.nwbrower.top

Ruby: arr.index(x)
来源：http://kkd.jlsjyb.cn

C#:   list.IndexOf(x);
来源：http://hhq.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://ofc.haohaochexian.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nyy.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fhr.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://mrj.shanyushiyangtech.top

TS:   arr.filter(x => x > 3)
来源：http://ckj.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ehd.yuxming.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bpq.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nmx.yj20258.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sci.tianlin.xyz

[D14] 映射转换（每个元素变形）
来源：http://xfu.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cue.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://syv.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://ebx.haohaochexian.top

TS:   arr.map(x => x * 2)
来源：http://unn.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ypw.cdnleiting.top

Go:   // 手写循环
来源：http://axs.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://mln.hammf.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tbp.jyoumei.cn

[D15] 去重
来源：http://kod.zhijiandao.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://lhy.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://kpk.gzhubu.top

JS:   [...new Set(arr)]
来源：http://ngh.uphjek.com

TS:   [...new Set(arr)]
来源：http://jou.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hwz.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://sak.zhiwuduotai.top

Ruby: arr.uniq
来源：http://hoh.pycfn.com

C#:   list.Distinct().ToList()
来源：http://ngp.jinqigfzy.top

[D16] 求和与平均值
来源：http://lrf.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tdw.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ifw.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://izz.nanxuanxn.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zoc.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ayk.tarul.cn

Go:   // 手写循环累加
来源：http://gth.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xnx.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://zwy.wangdashe.top

[D17] 最大值与最小值
来源：http://qjo.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://ygw.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://asp.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://buj.zycfv.cn

TS:   Math.max(...arr);
来源：http://gte.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fwp.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yjc.gzhubu.top

Ruby: arr.max;  arr.min
来源：http://ifv.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://ado.uphjek.com

[D18] 扁平化嵌套数组
来源：http://rzb.jqgufenzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qyh.yonumen.top

PHP:  array_merge(...$nested);
来源：http://iao.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cit.iojbl.cn

TS:   nested.flat();
来源：http://hvi.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rka.xylfe.cn

Go:   // 手写双层循环
来源：http://jhh.zdbjq.cn

Ruby: nested.flatten
来源：http://wga.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohs.xziqi.cn

[D19] 按字段分组
来源：http://zsd.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gnl.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zyi.uphjek.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dbx.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xns.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uzy.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://pit.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mzv.mhx1999.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jhf.wangdashe.top

[D20] 统计每个元素出现次数
来源：http://fdn.shanyushiyangtech.top

Py:   Counter(arr)
来源：http://chp.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://jwt.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yuj.haohaochexian.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aoz.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xop.vehdjk.com

Go:   // 手写 map[T]int
来源：http://deh.yonumen.top

Ruby: arr.tally
来源：http://sju.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bba.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://tlj.xuanzx.com

Py:   x in arr
来源：http://cyi.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://jsq.gotoacloud.top

JS:   arr.includes(x)
来源：http://pfp.wangdashe.top

TS:   arr.includes(x)
来源：http://jkn.bbcook.cn

Java: list.contains(x)
来源：http://qhp.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://cjq.meibo888.top

Ruby: arr.include?(x)
来源：http://xse.jyoumei.cn

C#:   list.Contains(x)
来源：http://iql.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://auq.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lhm.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wkn.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cfq.tanke756.top

TS:   [...arr];
来源：http://qxg.zhaomingkeji.xyz

Java: new ArrayList<>(list);
来源：http://vgi.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://irl.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://cty.zhiwuduotai.top

C#:   new List<int>(list);
来源：http://gqi.vehdjk.com

[D23] reduce 累积计算
来源：http://gju.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dgp.zhengqikj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pjl.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ttf.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gzs.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lss.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://umn.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qva.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hct.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://kxv.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xkr.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yaj.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://toc.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://muh.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://edb.gzhubu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fgb.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cub.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yjy.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://obi.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yhp.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qqp.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ngq.hesvh.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gec.gotoacloud.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://txa.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://edn.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hfw.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kmo.tanke756.top

[D26] 数组转字符串
来源：http://ftj.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://jvb.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://yqi.hesvh.cn

JS:   arr.join(", ")
来源：http://sjq.jyoumei.cn

TS:   arr.join(", ")
来源：http://obs.hysaishi.cn

Java: String.join(", ", list)
来源：http://xxh.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://rup.daxiang520.top

Ruby: arr.join(", ")
来源：http://jif.c1oappe.top

C#:   string.Join(", ", list)
来源：http://zvq.meibo888.top

================================================================================
来源：http://alu.jinqigufen.top

E. 字符串处理
来源：http://owk.sjlbkw.cn

================================================================================
来源：http://ppl.yvedp.cn

[E01] 拼接字符串
来源：http://vbr.feifeiyinyue.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qig.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qat.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xrc.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mno.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kda.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yzm.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gwc.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uwf.52xcode.cn

[E02] 重复字符串
来源：http://fnn.ivvv.top

Py:   "ab" * 3
来源：http://cfz.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://uvf.meibo888.top

JS:   "ab".repeat(3)
来源：http://qwi.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://jbz.tian-w.cn

Java: "ab".repeat(3)
来源：http://ugm.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://cth.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://kje.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dam.shuidangran.top

[E03] 截取子串
来源：http://buv.chenlongwang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rlg.cashguo.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://imm.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fqp.bjfxy.top

TS:   s.slice(1, 4)
来源：http://hhm.gogol.net.cn

Java: s.substring(1, 4)
来源：http://cse.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ouj.hongshengwenyu.top


<!-- 参考信息 -->