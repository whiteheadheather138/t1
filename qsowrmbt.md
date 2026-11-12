代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kgm.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xcy.jinyuanbaomall.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ype.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pxm.yj20258.top

Java: int add(int a, int b) { return a + b; }
来源：http://abj.zhongyouzk.top

Go:   func add(a, b int) int
来源：http://saq.yonumen.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nvf.nanxinkj.top

C#:   int Add(int a, int b) => a + b;
来源：http://eqk.xuanzx.com

[C14] 泛型函数
来源：http://qgf.quarkkingdee.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wfb.yuanzhike.top

PHP:  // 无泛型
来源：http://eyt.zhongyouzk.top

JS:   // 无泛型
来源：http://rtm.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tvq.shanyushiyangtech.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zeo.havefunace.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pwq.yvedp.cn

Ruby: # 无泛型
来源：http://afx.jinqigfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://phg.ctjpmb.com

[C15] 解构 / 展开参数
来源：http://oop.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hmf.zycfv.cn

PHP:  [$a, $b] = $pair;
来源：http://vpr.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pqg.chenjidiqi.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://tzg.zdbjq.cn

Java: // 无解构
来源：http://lmx.zdbjq.cn

Go:   // 无解构
来源：http://qqk.zhiwuduotai.top

Ruby: a, b = pair
来源：http://jdt.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://thq.sjlbkw.cn

[C16] 函数 / 方法重载
来源：http://uxh.xziqi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xia.gaohongyu789.top

PHP:  // 无重载
来源：http://npy.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hto.tian-w.cn

TS:   // 用联合类型或重载签名声明
来源：http://ghf.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fze.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://aof.shanyushiyangtech.top

Ruby: # 无重载：靠动态参数
来源：http://jtc.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gpd.fktsv.cn

================================================================================
来源：http://elf.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://isw.fanxiaobao.xyz

================================================================================
来源：http://awn.meibo888.top

[D01] 创建数组 / 列表
来源：http://xcd.chenjidiqi.icu

Py:   arr = [1, 2, 3];  empty = []
来源：http://ceb.fzhhl.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ytw.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jna.iojbl.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gxd.cashguo.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bsh.jqgfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://oyi.cdnleiting.top

Ruby: arr = [1, 2, 3]
来源：http://pbz.hnxiangtu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rkc.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://khe.daxiang520.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blv.tarul.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tzn.yvedp.cn

JS:   arr.push(4);
来源：http://uwl.ivvv.top

TS:   arr.push(4);
来源：http://wbh.zhongyouzk.top

Java: list.add(4);
来源：http://azv.shanyushiyangtech.top

Go:   arr = append(arr, 4)
来源：http://sga.tian-w.cn

Ruby: arr << 4; arr.push(5)
来源：http://dhq.yfazqb.com

C#:   list.Add(4);
来源：http://nvl.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://tti.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://haz.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kzq.daxiang520.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://klr.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://mik.ydzc1.top

Java: list.add(0, 0);
来源：http://jxf.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lvn.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qmp.hywenlv.cn

C#:   list.Insert(0, 0);
来源：http://dxw.shzxlz.cn

[D04] 删除元素
来源：http://sty.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tge.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cpn.fanxiaobao.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://don.jiagoushi.top

TS:   arr.splice(0, 1);
来源：http://jbq.aibaodan.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rys.hcnkem.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wtt.zycfv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bpq.vehdjk.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cbv.ydjk.org.cn

[D05] 访问与修改元素
来源：http://kvm.meibo888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://icb.ydzc1.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cxg.jyoumei.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lbd.zhongyouzk.top

TS:   arr[0]; arr.at(-1);
来源：http://uwt.jqgfzy.top

Java: list.get(0); list.set(0, 9);
来源：http://bfw.zhaomingkeji.xyz

Go:   arr[0]; arr[0] = 9
来源：http://dta.fehbvm.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uft.yuxming.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rke.sufxvd.cn

[D06] 数组长度
来源：http://syz.sjlbkw.cn

Py:   len(arr)
来源：http://fwk.jinqigufen.top

PHP:  count($arr);
来源：http://ukw.hammf.cn

JS:   arr.length
来源：http://iqy.ywan-chungtsiang.top

TS:   arr.length
来源：http://ehq.hongshengwenyu.top

Java: list.size();
来源：http://ulb.chenlongwang.top

Go:   len(arr)
来源：http://viv.nanxuanxn.top

Ruby: arr.length; arr.size
来源：http://wzw.tianlin.xyz

C#:   list.Count;
来源：http://mzg.zhengqikj.top

[D07] 切片 / 取子数组
来源：http://jar.snrcjt.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bqu.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://put.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://vrr.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://yjs.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://ikh.fehbvm.com

Go:   arr[1:4]
来源：http://sbd.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://lvk.ctjpmb.com

C#:   list.GetRange(1, 3);
来源：http://pif.uphjek.com

[D08] 合并两个数组
来源：http://hle.meibo888.top

Py:   a + b;  a.extend(b)
来源：http://ytt.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://gqf.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://xmu.cheryme.top

TS:   [...a, ...b];
来源：http://ytr.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://evi.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://xjr.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://dyr.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://fwq.xuetiantiany.cn

[D09] 排序（升序）
来源：http://hpo.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://xuq.cqqwz.cn

PHP:  sort($arr);
来源：http://xza.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qrg.zdbjq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://peg.yuanzhike.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wvm.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nuh.iojbl.cn

Ruby: arr.sort
来源：http://gvp.vqdsnc.cn

C#:   list.Sort();
来源：http://hdx.fanxiaobao.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://xdd.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yow.wangdashe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ptx.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nxg.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hmr.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://izb.yangfankeji.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gcb.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kaz.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cfm.aibaodan.cn

[D11] 反转数组
来源：http://sbg.chenzaomai.com

Py:   arr[::-1];  arr.reverse()
来源：http://qcr.tian-w.cn

PHP:  array_reverse($arr);
来源：http://wgm.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jhj.hywenlv.cn

TS:   [...arr].reverse();
来源：http://xts.nanxinkj.top

Java: Collections.reverse(list);
来源：http://ihm.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://ktz.shanyushiyangkeji.top

Ruby: arr.reverse
来源：http://tas.zdqjudy.top

C#:   list.Reverse();
来源：http://xcs.xuetiantiany.cn

[D12] 查找元素下标
来源：http://onr.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://tih.hesvh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kfm.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfi.zhoulong.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ptl.zhongyouzk.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cxk.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://wai.yangfankeji.com

Ruby: arr.index(x)
来源：http://ier.ivvv.top

C#:   list.IndexOf(x);
来源：http://ark.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://nvk.shangyingyoupin.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hwe.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dgs.yueranfly.top

JS:   arr.filter(x => x > 3)
来源：http://dol.hywenlv.cn

TS:   arr.filter(x => x > 3)
来源：http://tph.zhixingplan.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oom.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kfm.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ejr.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zlc.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://gcx.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://otm.daxiang520.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ihq.hysaishi.cn

JS:   arr.map(x => x * 2)
来源：http://zuw.zhaomingkeji.xyz

TS:   arr.map(x => x * 2)
来源：http://xit.havefunace.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zgs.sweek.top

Go:   // 手写循环
来源：http://roz.shanyushiyangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://lcp.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cqj.vqdsnc.cn

[D15] 去重
来源：http://yzv.shanyushiyangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rnf.hammf.cn

PHP:  array_unique($arr);
来源：http://tai.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://mfd.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://ywv.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://set.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://jfv.snrcjt.cn

Ruby: arr.uniq
来源：http://ovy.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://osr.yonumen.top

[D16] 求和与平均值
来源：http://vbs.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ifu.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://muh.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gyy.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mup.uphjek.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://viz.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://cpa.xinyue.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hiw.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://ckx.zdqjudy.top

[D17] 最大值与最小值
来源：http://oai.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://huv.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://imw.ctjpmb.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mys.yj202588.top

TS:   Math.max(...arr);
来源：http://agm.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oyy.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dzj.hammf.cn

Ruby: arr.max;  arr.min
来源：http://hoh.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://uau.nanxuanxn.top

[D18] 扁平化嵌套数组
来源：http://vua.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ecs.chenlongwang.top

PHP:  array_merge(...$nested);
来源：http://rio.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ybg.yonumen.top

TS:   nested.flat();
来源：http://myh.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://att.hnxiangtu.top

Go:   // 手写双层循环
来源：http://xdu.guowangkeji.top

Ruby: nested.flatten
来源：http://gql.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nxv.cheryme.top

[D19] 按字段分组
来源：http://ttn.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fph.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fus.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://urt.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://paa.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ser.hammf.cn

Go:   // 手写 map[string][]T
来源：http://afr.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://hqk.chenlongwang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fih.yj202588.top

[D20] 统计每个元素出现次数
来源：http://zst.ppjwa.cn

Py:   Counter(arr)
来源：http://hzb.gzhubu.top

PHP:  array_count_values($arr);
来源：http://vig.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://inq.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfj.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vvq.cheryme.top

Go:   // 手写 map[T]int
来源：http://etj.vehdjk.com

Ruby: arr.tally
来源：http://wrz.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ezx.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://tjf.hywenlv.cn

Py:   x in arr
来源：http://okn.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://zzo.gotoacloud.top

JS:   arr.includes(x)
来源：http://cxw.yj20258888.top

TS:   arr.includes(x)
来源：http://hdz.hammf.cn

Java: list.contains(x)
来源：http://zvs.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://tjg.dianchejie.cn

Ruby: arr.include?(x)
来源：http://hxy.ivvv.top

C#:   list.Contains(x)
来源：http://hrs.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://hzw.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hyw.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vri.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ecy.wangshuangyany.cn

TS:   [...arr];
来源：http://ifw.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://zhp.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://end.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://ued.haohaochexian.top

C#:   new List<int>(list);
来源：http://wbw.vehdjk.com

[D23] reduce 累积计算
来源：http://ime.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oqo.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uuo.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ikw.yuanzhike.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rev.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://quk.cqqwz.cn

Go:   // 手写循环
来源：http://gpe.havefunace.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qih.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uky.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://mfp.chenjidiqi.icu

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gtn.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qrh.aibaodan.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dpr.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fei.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dpb.ybcxt.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ihp.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kjm.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yqt.ppjwa.cn

[D25] Set 集合去重与交并差
来源：http://ilj.fanxiaobao.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yvl.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dwo.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vtf.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jqs.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qqi.kuanghao11.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://giu.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lnl.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jqm.zycfv.cn

[D26] 数组转字符串
来源：http://ajj.cheryme.top

Py:   ", ".join(map(str, arr))
来源：http://ikg.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://ynk.epnwcf.com

JS:   arr.join(", ")
来源：http://pms.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://uuy.fktsv.cn

Java: String.join(", ", list)
来源：http://btm.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://vzg.hammf.cn

Ruby: arr.join(", ")
来源：http://orl.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://bsc.yongpay.top

================================================================================
来源：http://gcb.ctjpmb.com

E. 字符串处理
来源：http://ddt.jinyuanbaomall.cn

================================================================================
来源：http://pmp.daria6918.cn

[E01] 拼接字符串
来源：http://ipw.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rhi.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vyy.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzp.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgh.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vyp.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ikt.bjfxy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fuu.smart0.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xqr.hywenlv.cn

[E02] 重复字符串
来源：http://mwv.uphjek.com

Py:   "ab" * 3
来源：http://ibd.feifeiyinyue.top

PHP:  str_repeat("ab", 3);
来源：http://lmz.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://vas.fktsv.cn

TS:   "ab".repeat(3)
来源：http://bar.ctjpmb.com

Java: "ab".repeat(3)
来源：http://cew.svipenyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://gze.pycfn.com

Ruby: "ab" * 3
来源：http://tyv.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xzp.dashuyun.cn

[E03] 截取子串
来源：http://jbw.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aqn.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://phn.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://egc.ydzc1.top

TS:   s.slice(1, 4)
来源：http://hhm.ydzc1.top

Java: s.substring(1, 4)
来源：http://hti.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qhh.tarul.cn


<!-- 参考信息 -->