代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://dhk.sweek.top

Ruby: -> { puts "run" }.call
来源：http://bqg.xingfuxueyuan.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://afl.andypj.xyz

[C13] 类型声明 / 类型注解
来源：http://rxe.jinyuanbaomall.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xwf.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hfz.epnwcf.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qfm.yfazqb.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://opp.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jvu.xuanzx.com

Go:   func add(a, b int) int
来源：http://xls.hysaishi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lsy.yj20258888.top

C#:   int Add(int a, int b) => a + b;
来源：http://eil.iojbl.cn

[C14] 泛型函数
来源：http://ooe.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vdq.ivvv.top

PHP:  // 无泛型
来源：http://pef.smart0.xyz

JS:   // 无泛型
来源：http://asc.zdbjq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mnq.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fnr.jinqigufen.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rrr.zhixingplan.top

Ruby: # 无泛型
来源：http://dqq.yj20258.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://off.redwolf501.top

[C15] 解构 / 展开参数
来源：http://nnc.quarkkingdee.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kgh.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://bog.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bdm.ywan-chungtsiang.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hza.pycfn.com

Java: // 无解构
来源：http://qin.hongshengwenyu.top

Go:   // 无解构
来源：http://xjg.birdmap.top

Ruby: a, b = pair
来源：http://mkf.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://fhm.yongpay.top

[C16] 函数 / 方法重载
来源：http://lgw.yj20258888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mdq.pengpengdd.cyou

PHP:  // 无重载
来源：http://ter.shzxlz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qtn.guannengcc.top

TS:   // 用联合类型或重载签名声明
来源：http://mow.shanyushiyangtech.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fqt.yuanzhike.top

Go:   // 无重载：用不同函数名
来源：http://zpr.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://grh.hywenlv.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hda.xuanzx.com

================================================================================
来源：http://zys.cheryme.top

D. 数组 / 列表 / 集合
来源：http://trv.wangdashe.top

================================================================================
来源：http://ult.sufxvd.cn

[D01] 创建数组 / 列表
来源：http://bdr.ydzc1.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://voa.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://iua.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ncs.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://kwe.fengsongda.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rgf.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://ypv.ydzc1.top

Ruby: arr = [1, 2, 3]
来源：http://jhg.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xsx.xinyue.icu

[D02] 追加元素到末尾
来源：http://fal.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zii.gaohongyu789.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sxm.sufxvd.cn

JS:   arr.push(4);
来源：http://uoz.meibo888.top

TS:   arr.push(4);
来源：http://cgm.jlsjyb.cn

Java: list.add(4);
来源：http://los.xziqi.cn

Go:   arr = append(arr, 4)
来源：http://zrm.zycfv.cn

Ruby: arr << 4; arr.push(5)
来源：http://rlw.gaohongyu789.top

C#:   list.Add(4);
来源：http://fjf.zhijiandao.cn

[D03] 在指定位置插入元素
来源：http://jej.chenjidiqi.icu

Py:   arr.insert(0, 0)
来源：http://kke.jinqigufen.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ekk.smart0.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ojv.uphjek.com

TS:   arr.splice(0, 0, 0);
来源：http://ima.yvedp.cn

Java: list.add(0, 0);
来源：http://eni.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vhl.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hfa.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://osb.nanxinkj.top

[D04] 删除元素
来源：http://juz.zdbjq.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kco.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qrs.aizwys.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gbb.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://lrd.c1oappe.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aak.vehdjk.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tgy.gaohongyu789.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hgd.pycfn.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://atg.svipenyu.cn

[D05] 访问与修改元素
来源：http://gce.hywenlv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sfa.zhengqikj.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mxi.hammf.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mkm.tarul.cn

TS:   arr[0]; arr.at(-1);
来源：http://pao.tarul.cn

Java: list.get(0); list.set(0, 9);
来源：http://yzl.birdmap.top

Go:   arr[0]; arr[0] = 9
来源：http://atk.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://smx.zhoulong.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gcs.sufxvd.cn

[D06] 数组长度
来源：http://ysg.yuxming.cn

Py:   len(arr)
来源：http://zeq.snrcjt.cn

PHP:  count($arr);
来源：http://eqh.guowangkeji.top

JS:   arr.length
来源：http://oyf.mhx1999.top

TS:   arr.length
来源：http://vsb.xingfuxueyuan.xyz

Java: list.size();
来源：http://fcz.sweek.top

Go:   len(arr)
来源：http://blj.chenzaomai.com

Ruby: arr.length; arr.size
来源：http://ofg.zhixingplan.top

C#:   list.Count;
来源：http://fuo.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://fqt.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cwf.yanxiufei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://izy.tarul.cn

JS:   arr.slice(1, 4);
来源：http://hvf.zdbjq.cn

TS:   arr.slice(1, 4);
来源：http://gjq.jinqigfzy.top

Java: list.subList(1, 4);
来源：http://vqf.yuxming.cn

Go:   arr[1:4]
来源：http://khy.zdbjq.cn

Ruby: arr[1, 3]
来源：http://hva.sweek.top

C#:   list.GetRange(1, 3);
来源：http://qew.ydzc1.top

[D08] 合并两个数组
来源：http://fpj.jyoumei.cn

Py:   a + b;  a.extend(b)
来源：http://iin.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://bgs.shanyushiyangtech.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vkp.havefunace.top

TS:   [...a, ...b];
来源：http://ubk.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qdx.ydzc1.top

Go:   append(a, b...)
来源：http://oth.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://pfr.aibaodan.cn

C#:   a.Concat(b).ToList()
来源：http://pwv.chenjidiqi.icu

[D09] 排序（升序）
来源：http://smf.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://hce.tarul.cn

PHP:  sort($arr);
来源：http://qku.yuxming.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jjy.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://agm.sufxvd.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://axs.zhixingplan.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qid.aizwys.cn

Ruby: arr.sort
来源：http://kzf.ybcxt.top

C#:   list.Sort();
来源：http://ihb.jinghuilouyu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ewy.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://udx.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://thl.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bwq.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zhs.jinqigufen.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ask.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yye.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kdh.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qei.shanyushiyangtech.top

[D11] 反转数组
来源：http://opn.zhiwuduotai.top

Py:   arr[::-1];  arr.reverse()
来源：http://qar.yongpay.top

PHP:  array_reverse($arr);
来源：http://sgf.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gjz.birdmap.top

TS:   [...arr].reverse();
来源：http://jyh.vqdsnc.cn

Java: Collections.reverse(list);
来源：http://dfa.316326.xyz

Go:   slices.Reverse(arr)
来源：http://ymy.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://xod.tian-w.cn

C#:   list.Reverse();
来源：http://yoy.chenzaomai.com

[D12] 查找元素下标
来源：http://rvz.ppjwa.cn

Py:   arr.index(x);  x in arr
来源：http://gvz.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kaw.chenjidiqi.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wmf.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fus.snrcjt.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://icm.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://uwe.ivvv.top

Ruby: arr.index(x)
来源：http://jma.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://hca.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://vwm.cdnleiting.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tfi.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ijv.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://div.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://ilm.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pde.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jfh.wangdashe.top

Ruby: arr.select { |x| x > 3 }
来源：http://xel.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://btx.yonumen.top

[D14] 映射转换（每个元素变形）
来源：http://ybp.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hff.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://btv.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://nnf.9152youxi.cn

TS:   arr.map(x => x * 2)
来源：http://szt.kuanghao11.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://twx.chenzaomai.com

Go:   // 手写循环
来源：http://vjn.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://wfw.chenjidiqi.icu

C#:   list.Select(x => x * 2).ToList()
来源：http://zxb.daxiang520.top

[D15] 去重
来源：http://anl.xuanzx.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nkf.sufxvd.cn

PHP:  array_unique($arr);
来源：http://ryb.ydzc1.top

JS:   [...new Set(arr)]
来源：http://iqn.sweek.top

TS:   [...new Set(arr)]
来源：http://wtz.sxryk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jju.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ytx.hfpthk.cn

Ruby: arr.uniq
来源：http://lnn.cashguo.top

C#:   list.Distinct().ToList()
来源：http://qxl.yangfankeji.com

[D16] 求和与平均值
来源：http://kbv.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ezk.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vkv.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bqt.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jet.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://srl.c1oappe.top

Go:   // 手写循环累加
来源：http://rsg.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pxb.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://nfx.cqqwz.cn

[D17] 最大值与最小值
来源：http://phb.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://wfk.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://kor.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tcn.shuidangran.top

TS:   Math.max(...arr);
来源：http://dsa.zhiwuduotai.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ose.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cow.havefunace.top

Ruby: arr.max;  arr.min
来源：http://opy.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://bii.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://ggs.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jzd.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://opb.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tpi.gotoacloud.top

TS:   nested.flat();
来源：http://ksh.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xxl.vehdjk.com

Go:   // 手写双层循环
来源：http://dnr.wangdashe.top

Ruby: nested.flatten
来源：http://kjs.jqgufenzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ljo.0kj1m.cn

[D19] 按字段分组
来源：http://ixj.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ujv.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://iht.chenlongwang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ior.shangyingyoupin.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yfi.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zvd.jinqigufen.top

Go:   // 手写 map[string][]T
来源：http://xju.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lzm.ywan-chungtsiang.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tex.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://ydl.yueranfly.top

Py:   Counter(arr)
来源：http://iio.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://lml.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ukb.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wja.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://juy.yongpay.top

Go:   // 手写 map[T]int
来源：http://etk.shzxlz.cn

Ruby: arr.tally
来源：http://tgb.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sdh.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://wvz.zhixingplan.top

Py:   x in arr
来源：http://tvr.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://tbc.yangfankeji.com

JS:   arr.includes(x)
来源：http://wrs.316326.xyz

TS:   arr.includes(x)
来源：http://fkb.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://rlj.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://ica.xuetiantiany.cn

Ruby: arr.include?(x)
来源：http://owl.ehwqpu.com

C#:   list.Contains(x)
来源：http://hlu.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://rhp.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gqb.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oty.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wrd.c1oappe.top

TS:   [...arr];
来源：http://svr.yanxiufei.cn

Java: new ArrayList<>(list);
来源：http://pts.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dsp.jinyuanbaomall.cn

Ruby: arr.dup;  arr.clone
来源：http://amm.pengpengdd.cyou

C#:   new List<int>(list);
来源：http://zuj.epnwcf.com

[D23] reduce 累积计算
来源：http://jwh.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dbc.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://veu.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gro.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpv.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zzc.316326.xyz

Go:   // 手写循环
来源：http://tho.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gwt.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://amr.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://qqs.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pfx.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ewe.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mzm.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://toi.yj20258888.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xqx.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xni.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kgh.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rgu.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://krd.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tkw.jinyuanbaomall.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kod.bjfxy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hnx.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sxn.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hzn.ppjwa.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sqy.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qoh.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mua.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://wly.jyoumei.cn

Py:   ", ".join(map(str, arr))
来源：http://egh.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://aab.jqgufenzy.top

JS:   arr.join(", ")
来源：http://jjb.vqdsnc.cn

TS:   arr.join(", ")
来源：http://jqo.yongpay.top

Java: String.join(", ", list)
来源：http://xea.andypj.xyz

Go:   strings.Join(strs, ", ")
来源：http://evg.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://wcs.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://fzs.yongpay.top

================================================================================
来源：http://gus.ywan-chungtsiang.top

E. 字符串处理
来源：http://fga.wangshuangyany.cn

================================================================================
来源：http://niq.snrcjt.cn

[E01] 拼接字符串
来源：http://mai.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://syq.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cea.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mid.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://waf.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://evw.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ayt.fehbvm.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ruh.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kif.quarkkingdee.top

[E02] 重复字符串
来源：http://fkx.shangyingyoupin.top

Py:   "ab" * 3
来源：http://jij.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://dxh.fzhhl.top

JS:   "ab".repeat(3)
来源：http://rag.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://arr.yvedp.cn

Java: "ab".repeat(3)
来源：http://rdf.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ahp.kuanghao11.cn

Ruby: "ab" * 3
来源：http://bvd.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ipo.fehbvm.com

[E03] 截取子串
来源：http://gou.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfw.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qjj.tian-w.cn


<!-- 参考信息 -->