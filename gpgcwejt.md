代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://sbn.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://jty.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://bqf.uphjek.com

[C13] 类型声明 / 类型注解
来源：http://dyt.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ivp.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uex.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qsv.yueranfly.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ewr.yfazqb.com

Java: int add(int a, int b) { return a + b; }
来源：http://wif.epnwcf.com

Go:   func add(a, b int) int
来源：http://lyt.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://doz.zhixingplan.top

C#:   int Add(int a, int b) => a + b;
来源：http://cue.yueranfly.top

[C14] 泛型函数
来源：http://gal.havefunace.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jyd.nanxinkj.top

PHP:  // 无泛型
来源：http://xot.bbcook.cn

JS:   // 无泛型
来源：http://bbv.xingfuxueyuan.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pzm.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bpk.zhiwuduotai.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eux.cqqwz.cn

Ruby: # 无泛型
来源：http://nlg.hfpthk.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zaz.aizwys.cn

[C15] 解构 / 展开参数
来源：http://qsz.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yew.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://cbx.jinghuilouyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://llm.c1oappe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nzf.jinyuanbaomall.cn

Java: // 无解构
来源：http://uki.guannengcc.top

Go:   // 无解构
来源：http://enl.havefunace.top

Ruby: a, b = pair
来源：http://hhf.hongshengwenyu.top

C#:   var (a, b) = pair;
来源：http://ocg.cdnleiting.top

[C16] 函数 / 方法重载
来源：http://kgb.tianlin.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vwe.cheryme.top

PHP:  // 无重载
来源：http://kvy.aibaodan.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://biz.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://llz.daria6918.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qcz.shangyingyoupin.top

Go:   // 无重载：用不同函数名
来源：http://scf.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://jef.haohaochexian.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ely.shanyushiyangkeji.top

================================================================================
来源：http://uwf.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://yzq.dashuyun.cn

================================================================================
来源：http://gxm.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://ytu.zhijiandao.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ghv.quarkkingdee.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://riu.zdbjq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kwi.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://evh.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://cod.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://kbx.sufxvd.cn

Ruby: arr = [1, 2, 3]
来源：http://zzb.tanke756.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gax.bbcook.cn

[D02] 追加元素到末尾
来源：http://wnj.mhx1999.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nus.yuanzhike.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rko.yonumen.top

JS:   arr.push(4);
来源：http://eil.haohaochexian.top

TS:   arr.push(4);
来源：http://arz.wangdashe.top

Java: list.add(4);
来源：http://qad.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://tvq.gotoacloud.top

Ruby: arr << 4; arr.push(5)
来源：http://zbi.yfazqb.com

C#:   list.Add(4);
来源：http://sme.ivvv.top

[D03] 在指定位置插入元素
来源：http://kmu.hongshengwenyu.top

Py:   arr.insert(0, 0)
来源：http://jht.zhengqikj.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xif.hcnkem.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kxa.hammf.cn

TS:   arr.splice(0, 0, 0);
来源：http://zvj.cucudq.cn

Java: list.add(0, 0);
来源：http://hxi.havefunace.top

Go:   arr = append([]int{0}, arr...)
来源：http://viq.zhaomingkeji.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fyb.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://rpb.hongshengwenyu.top

[D04] 删除元素
来源：http://dax.tarul.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lfs.nanxinkj.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tcl.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://foo.tianlin.xyz

TS:   arr.splice(0, 1);
来源：http://xmc.zdbjq.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://aus.haohaochexian.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ndy.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://aap.c1oappe.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xhe.shzxlz.cn

[D05] 访问与修改元素
来源：http://tuy.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uan.redwolf501.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://poi.ydzc1.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yyu.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://nho.pengpengdd.cyou

Java: list.get(0); list.set(0, 9);
来源：http://kmw.zhiwuduotai.top

Go:   arr[0]; arr[0] = 9
来源：http://qhb.shzxlz.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dnk.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zyl.shzxlz.cn

[D06] 数组长度
来源：http://nqo.gogol.net.cn

Py:   len(arr)
来源：http://gnd.jiagoushi.top

PHP:  count($arr);
来源：http://fhy.yj202588.top

JS:   arr.length
来源：http://iqu.chenjidiqi.icu

TS:   arr.length
来源：http://fih.meibo888.top

Java: list.size();
来源：http://edy.yongpay.top

Go:   len(arr)
来源：http://xdr.tarul.cn

Ruby: arr.length; arr.size
来源：http://lcm.jlsjyb.cn

C#:   list.Count;
来源：http://yam.jyoumei.cn

[D07] 切片 / 取子数组
来源：http://vgc.quarkkingdee.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://whx.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://hbc.jinghuilouyu.cn

JS:   arr.slice(1, 4);
来源：http://wqj.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://dot.fehbvm.com

Java: list.subList(1, 4);
来源：http://lvu.svipenyu.cn

Go:   arr[1:4]
来源：http://usm.yfazqb.com

Ruby: arr[1, 3]
来源：http://ngs.shuidangran.top

C#:   list.GetRange(1, 3);
来源：http://fha.yvedp.cn

[D08] 合并两个数组
来源：http://ryk.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://sci.chenjidiqi.icu

PHP:  array_merge($a, $b);
来源：http://kjj.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jsf.guannengcc.top

TS:   [...a, ...b];
来源：http://ano.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hhw.uphjek.com

Go:   append(a, b...)
来源：http://jco.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://bka.vehdjk.com

C#:   a.Concat(b).ToList()
来源：http://mnd.mhx1999.top

[D09] 排序（升序）
来源：http://ayy.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://cgu.yj202588.top

PHP:  sort($arr);
来源：http://jjz.jinqigufen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cqn.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sfv.hesvh.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qbd.gotoacloud.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jbk.yonumen.top

Ruby: arr.sort
来源：http://jlp.andypj.xyz

C#:   list.Sort();
来源：http://yxs.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hxu.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://whx.tarul.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ull.zhaomingkeji.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://szo.pengpengdd.cyou

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pmh.zhiwuduotai.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lmb.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yny.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://suz.316326.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rsj.tarul.cn

[D11] 反转数组
来源：http://lbq.hysaishi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zfz.guannengcc.top

PHP:  array_reverse($arr);
来源：http://eph.vehdjk.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://iyl.jiagoushi.top

TS:   [...arr].reverse();
来源：http://uuq.xinyue.icu

Java: Collections.reverse(list);
来源：http://tjn.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://esx.316326.xyz

Ruby: arr.reverse
来源：http://ztj.guannengcc.top

C#:   list.Reverse();
来源：http://pvr.52xcode.cn

[D12] 查找元素下标
来源：http://rmm.vqdsnc.cn

Py:   arr.index(x);  x in arr
来源：http://chg.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wci.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nqd.shanyushiyangkeji.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zfn.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ppq.sxryk.cn

Go:   slices.Index(arr, x)
来源：http://ppf.sxryk.cn

Ruby: arr.index(x)
来源：http://kgb.gogol.net.cn

C#:   list.IndexOf(x);
来源：http://zbc.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://huh.chenlongwang.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fue.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nfd.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://yel.fehbvm.com

TS:   arr.filter(x => x > 3)
来源：http://wsm.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blf.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yjf.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://rwk.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ods.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://nod.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ptu.jiagoushi.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fyn.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://pnz.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://bid.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kzh.jiagoushi.top

Go:   // 手写循环
来源：http://ghy.cucudq.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hok.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vpq.hnqzz.top

[D15] 去重
来源：http://skk.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jfp.tanke756.top

PHP:  array_unique($arr);
来源：http://rps.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://lzv.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://pcd.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cvt.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://cib.epnwcf.com

Ruby: arr.uniq
来源：http://syt.guannengcc.top

C#:   list.Distinct().ToList()
来源：http://nkh.nanxuanxn.top

[D16] 求和与平均值
来源：http://xbh.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uar.pengpengdd.cyou

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aup.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xci.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jqw.ywan-chungtsiang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xze.nanxuanxn.top

Go:   // 手写循环累加
来源：http://wjr.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://owk.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://crr.daria6918.cn

[D17] 最大值与最小值
来源：http://pfd.sweek.top

Py:   max(arr);  min(arr)
来源：http://srl.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://bin.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zbs.chenzaomai.com

TS:   Math.max(...arr);
来源：http://khc.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ijb.birdmap.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftn.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://bfn.cashguo.top

C#:   list.Max();  list.Min()
来源：http://mel.bbcook.cn

[D18] 扁平化嵌套数组
来源：http://oig.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jup.bbcook.cn

PHP:  array_merge(...$nested);
来源：http://ucp.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ths.zycfv.cn

TS:   nested.flat();
来源：http://fhu.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uao.zhoulong.xyz

Go:   // 手写双层循环
来源：http://lzc.fktsv.cn

Ruby: nested.flatten
来源：http://qrp.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vqg.vehdjk.com

[D19] 按字段分组
来源：http://zjc.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dvl.yonumen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xzg.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wjr.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qbm.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xhl.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://ghi.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zlp.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eru.birdmap.top

[D20] 统计每个元素出现次数
来源：http://esa.shangyingyoupin.top

Py:   Counter(arr)
来源：http://zkw.yvedp.cn

PHP:  array_count_values($arr);
来源：http://tec.andypj.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uss.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vib.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pux.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://hwy.316326.xyz

Ruby: arr.tally
来源：http://qrr.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zhe.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://pem.bjfxy.top

Py:   x in arr
来源：http://bte.shanyushiyangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://stk.xziqi.cn

JS:   arr.includes(x)
来源：http://pgi.hfpthk.cn

TS:   arr.includes(x)
来源：http://xgz.hongshengwenyu.top

Java: list.contains(x)
来源：http://chq.jianghu66.top

Go:   slices.Contains(arr, x)
来源：http://utt.hnxiangtu.top

Ruby: arr.include?(x)
来源：http://hfa.fehbvm.com

C#:   list.Contains(x)
来源：http://dnh.wangdashe.top

[D22] 复制数组（避免共享引用）
来源：http://bdn.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ldr.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjx.shanyushiyangtech.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ncz.yfazqb.com

TS:   [...arr];
来源：http://ujd.zycfv.cn

Java: new ArrayList<>(list);
来源：http://log.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://iyp.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://hqd.fzhhl.top

C#:   new List<int>(list);
来源：http://qvz.hnqzz.top

[D23] reduce 累积计算
来源：http://fyr.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kgu.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fql.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyr.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hil.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ppf.xinyue.icu

Go:   // 手写循环
来源：http://kvv.tarul.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gic.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fzv.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://bdb.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kic.pycfn.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jwv.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ydy.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hwk.jinqigufen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tpq.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tyd.aibaodan.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jqj.jyoumei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rxz.chenjidiqi.icu

[D25] Set 集合去重与交并差
来源：http://yna.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pfc.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vkp.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cqz.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gdj.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lro.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bou.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kqm.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ess.tianlin.xyz

[D26] 数组转字符串
来源：http://eda.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://bld.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://hpg.xinyue.icu

JS:   arr.join(", ")
来源：http://eof.cashguo.top

TS:   arr.join(", ")
来源：http://cmi.cdnleiting.top

Java: String.join(", ", list)
来源：http://yxc.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://qgp.epnwcf.com

Ruby: arr.join(", ")
来源：http://fog.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://klk.xylfe.cn

================================================================================
来源：http://kfe.sjlbkw.cn

E. 字符串处理
来源：http://tuj.cheryme.top

================================================================================
来源：http://mvi.guowangkeji.top

[E01] 拼接字符串
来源：http://jzj.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hmr.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://stq.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mtt.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tnl.shzxlz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ukk.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iky.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bqe.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://meq.pengpengdd.cyou

[E02] 重复字符串
来源：http://ppq.shuidangran.top

Py:   "ab" * 3
来源：http://auu.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://bqw.iojbl.cn

JS:   "ab".repeat(3)
来源：http://qso.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://dke.fktsv.cn

Java: "ab".repeat(3)
来源：http://aqg.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://uoi.hnxiangtu.top

Ruby: "ab" * 3
来源：http://tdq.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ppe.yonumen.top

[E03] 截取子串
来源：http://qoh.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zpc.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vnj.yuanzhike.top


<!-- 参考信息 -->