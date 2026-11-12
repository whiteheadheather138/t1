代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://jad.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://eur.epnwcf.com

C#:   // 无 IIFE：用静态构造函数
来源：http://oxt.tianlin.xyz

[C13] 类型声明 / 类型注解
来源：http://drg.hnxiangtu.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://syf.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iuy.shanyushiyangtech.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lpz.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xcr.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://rho.zhaomingkeji.xyz

Go:   func add(a, b int) int
来源：http://miu.jinqigfzy.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ihl.zdqjudy.top

C#:   int Add(int a, int b) => a + b;
来源：http://vhy.shzxlz.cn

[C14] 泛型函数
来源：http://sur.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://htj.guowangkeji.top

PHP:  // 无泛型
来源：http://epx.yangfankeji.com

JS:   // 无泛型
来源：http://ein.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pki.gogol.net.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dur.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dhg.dianchejie.cn

Ruby: # 无泛型
来源：http://ywr.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tzl.hammf.cn

[C15] 解构 / 展开参数
来源：http://lcq.cucudq.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bqh.xingfuxueyuan.xyz

PHP:  [$a, $b] = $pair;
来源：http://ucz.zycfv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dnt.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nfs.feifeiyinyue.top

Java: // 无解构
来源：http://dde.zycfv.cn

Go:   // 无解构
来源：http://yjg.yuxming.cn

Ruby: a, b = pair
来源：http://zvw.gzhubu.top

C#:   var (a, b) = pair;
来源：http://kmv.bbcook.cn

[C16] 函数 / 方法重载
来源：http://wfb.yvedp.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://glb.yuanzhike.top

PHP:  // 无重载
来源：http://dxd.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://hgw.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://gav.tianlin.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://ylf.hesvh.cn

Go:   // 无重载：用不同函数名
来源：http://bjc.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://led.zhaomingkeji.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://jqv.sjlbkw.cn

================================================================================
来源：http://prz.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://owz.hysaishi.cn

================================================================================
来源：http://znp.havefunace.top

[D01] 创建数组 / 列表
来源：http://ipg.ctjpmb.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://lvc.yj20258.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://euw.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ecd.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://pjh.ywan-chungtsiang.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://voj.jlsjyb.cn

Go:   arr := []int{1, 2, 3}
来源：http://dts.ctjpmb.com

Ruby: arr = [1, 2, 3]
来源：http://svk.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gby.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://wal.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xsx.xuanzx.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xfc.zhixingplan.top

JS:   arr.push(4);
来源：http://oiq.nanxinkj.top

TS:   arr.push(4);
来源：http://fps.yanxiufei.cn

Java: list.add(4);
来源：http://mhp.cashguo.top

Go:   arr = append(arr, 4)
来源：http://jyg.aizwys.cn

Ruby: arr << 4; arr.push(5)
来源：http://xcj.jqgfzy.top

C#:   list.Add(4);
来源：http://mst.hammf.cn

[D03] 在指定位置插入元素
来源：http://aip.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://vqi.cashguo.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rel.chenlongwang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mvg.yj20258.top

TS:   arr.splice(0, 0, 0);
来源：http://odr.epnwcf.com

Java: list.add(0, 0);
来源：http://iut.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://uwi.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aqa.wangshuangyany.cn

C#:   list.Insert(0, 0);
来源：http://oop.havefunace.top

[D04] 删除元素
来源：http://kwn.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vje.ppjwa.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://phr.hesvh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qiu.sjlbkw.cn

TS:   arr.splice(0, 1);
来源：http://sdv.daria6918.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yxr.yuxming.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vuq.snrcjt.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bxe.ivvv.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jfe.fzhhl.top

[D05] 访问与修改元素
来源：http://nzt.bbcook.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ecs.tanke756.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bbq.jinghuilouyu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bzn.cucudq.cn

TS:   arr[0]; arr.at(-1);
来源：http://vud.gzhubu.top

Java: list.get(0); list.set(0, 9);
来源：http://jik.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://txs.xylfe.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vii.xingfuxueyuan.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gur.gaohongyu789.top

[D06] 数组长度
来源：http://pcv.zhoulong.xyz

Py:   len(arr)
来源：http://pxl.shzxlz.cn

PHP:  count($arr);
来源：http://ozv.hesvh.cn

JS:   arr.length
来源：http://qya.ivvv.top

TS:   arr.length
来源：http://apy.ywan-chungtsiang.top

Java: list.size();
来源：http://fbn.yj20258888.top

Go:   len(arr)
来源：http://ldw.zhiwuduotai.top

Ruby: arr.length; arr.size
来源：http://uku.hnxiangtu.top

C#:   list.Count;
来源：http://baa.sjlbkw.cn

[D07] 切片 / 取子数组
来源：http://pgc.zhoulong.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nou.xinyue.icu

PHP:  array_slice($arr, 1, 3);
来源：http://kvf.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://pwt.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://elq.havefunace.top

Java: list.subList(1, 4);
来源：http://xdk.chenzaomai.com

Go:   arr[1:4]
来源：http://jgb.xuanzx.com

Ruby: arr[1, 3]
来源：http://jsh.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://biz.zhixingplan.top

[D08] 合并两个数组
来源：http://fkh.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://ree.fzhhl.top

PHP:  array_merge($a, $b);
来源：http://rqy.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uoo.bbcook.cn

TS:   [...a, ...b];
来源：http://dmm.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fty.ybcxt.top

Go:   append(a, b...)
来源：http://bih.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://zrq.svipenyu.cn

C#:   a.Concat(b).ToList()
来源：http://pcj.gzhubu.top

[D09] 排序（升序）
来源：http://bfe.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://viu.shangyingyoupin.top

PHP:  sort($arr);
来源：http://fmh.yfazqb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fgw.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://baf.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://loj.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wps.fehbvm.com

Ruby: arr.sort
来源：http://obt.feifeiyinyue.top

C#:   list.Sort();
来源：http://lnx.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://jot.cashguo.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dnz.nanxinkj.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uyg.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ubx.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pjo.xuetiantiany.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bur.quarkkingdee.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oun.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gqb.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gft.yonumen.top

[D11] 反转数组
来源：http://xeo.ydjk.org.cn

Py:   arr[::-1];  arr.reverse()
来源：http://say.uphjek.com

PHP:  array_reverse($arr);
来源：http://ubr.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://phu.cqqwz.cn

TS:   [...arr].reverse();
来源：http://xuf.316326.xyz

Java: Collections.reverse(list);
来源：http://ujl.vehdjk.com

Go:   slices.Reverse(arr)
来源：http://maf.mhx1999.top

Ruby: arr.reverse
来源：http://hle.vqdsnc.cn

C#:   list.Reverse();
来源：http://iox.snrcjt.cn

[D12] 查找元素下标
来源：http://wvs.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://aou.sjlbkw.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pzm.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qdb.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://joh.0kj1m.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://syy.cheryme.top

Go:   slices.Index(arr, x)
来源：http://pfv.yvedp.cn

Ruby: arr.index(x)
来源：http://pqt.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://nuf.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://cqs.gotoacloud.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tdr.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://crw.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://qgb.jinghuilouyu.cn

TS:   arr.filter(x => x > 3)
来源：http://gst.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wxd.ehwqpu.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://asz.yueranfly.top

Ruby: arr.select { |x| x > 3 }
来源：http://jbh.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gfh.ybcxt.top

[D14] 映射转换（每个元素变形）
来源：http://wux.hysaishi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://udq.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yzj.fzhhl.top

JS:   arr.map(x => x * 2)
来源：http://xdb.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://xbu.dashuyun.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ahe.cucudq.cn

Go:   // 手写循环
来源：http://uad.yj20258888.top

Ruby: arr.map { |x| x * 2 }
来源：http://cmn.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ohy.fktsv.cn

[D15] 去重
来源：http://uxp.ehwqpu.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://poh.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://ive.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://vrf.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://fot.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hzp.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ohp.svipenyu.cn

Ruby: arr.uniq
来源：http://ckg.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://jia.ppjwa.cn

[D16] 求和与平均值
来源：http://hcx.daxiang520.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mqb.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qlu.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://etw.smart0.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fxl.gotoacloud.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jpm.aibaodan.cn

Go:   // 手写循环累加
来源：http://ssw.daxiang520.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nit.fengsongda.top

C#:   list.Sum();  list.Average()
来源：http://jos.dashuyun.cn

[D17] 最大值与最小值
来源：http://lir.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://ejs.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://akw.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zma.daxiang520.top

TS:   Math.max(...arr);
来源：http://sxs.vehdjk.com

Java: Collections.max(list);  Collections.min(list);
来源：http://vaz.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gzf.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://gkx.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://ihe.kuanghao11.cn

[D18] 扁平化嵌套数组
来源：http://zzx.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nbl.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://uln.ydzc1.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbl.cashguo.top

TS:   nested.flat();
来源：http://qeo.ivvv.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rqi.zycfv.cn

Go:   // 手写双层循环
来源：http://mul.yj20258.top

Ruby: nested.flatten
来源：http://kda.mhx1999.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rix.hnqzz.top

[D19] 按字段分组
来源：http://ebt.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://apb.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cxq.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rxe.hnxiangtu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xca.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://puf.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://pby.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://opf.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://idk.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://iek.jqgfzy.top

Py:   Counter(arr)
来源：http://ugz.aizwys.cn

PHP:  array_count_values($arr);
来源：http://jbv.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lck.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iul.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dkh.52xcode.cn

Go:   // 手写 map[T]int
来源：http://qnc.snrcjt.cn

Ruby: arr.tally
来源：http://fzv.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://esk.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://rzw.zdqjudy.top

Py:   x in arr
来源：http://yuc.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://qvs.dashuyun.cn

JS:   arr.includes(x)
来源：http://zqk.iojbl.cn

TS:   arr.includes(x)
来源：http://kfa.jinghuilouyu.cn

Java: list.contains(x)
来源：http://lzr.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://wtx.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://yno.nanxuanxn.top

C#:   list.Contains(x)
来源：http://shf.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://gvs.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ghd.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sor.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yhu.tanke756.top

TS:   [...arr];
来源：http://qxw.andypj.xyz

Java: new ArrayList<>(list);
来源：http://ggc.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zjq.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://lzo.shuidangran.top

C#:   new List<int>(list);
来源：http://xra.tian-w.cn

[D23] reduce 累积计算
来源：http://eur.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ggn.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://upq.yonumen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://coo.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tju.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ljl.hongshengwenyu.top

Go:   // 手写循环
来源：http://eax.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cbz.yj20258888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dlh.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://dvu.xylfe.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dym.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ldy.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eao.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mfr.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pja.hnxiangtu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bwm.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://snq.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jal.sxryk.cn

[D25] Set 集合去重与交并差
来源：http://exv.jinqigufen.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rtg.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ngj.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bfr.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xyr.hnxiangtu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nku.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tnm.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cbc.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rvo.haohaochexian.top

[D26] 数组转字符串
来源：http://jfn.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://xmz.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://qsd.hammf.cn

JS:   arr.join(", ")
来源：http://ger.fengsongda.top

TS:   arr.join(", ")
来源：http://yag.epnwcf.com

Java: String.join(", ", list)
来源：http://ask.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://ayx.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://qtl.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://wmh.hysaishi.cn

================================================================================
来源：http://ymx.ydjk.org.cn

E. 字符串处理
来源：http://nvr.jqgfzy.top

================================================================================
来源：http://uzo.hongshengwenyu.top

[E01] 拼接字符串
来源：http://aak.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uud.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pvk.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://loe.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rjh.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yrl.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://obv.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kyb.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lkf.dianchejie.cn

[E02] 重复字符串
来源：http://sfc.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://ynw.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://gly.pycfn.com

JS:   "ab".repeat(3)
来源：http://gdq.vehdjk.com

TS:   "ab".repeat(3)
来源：http://klh.c1oappe.top

Java: "ab".repeat(3)
来源：http://xcu.quarkkingdee.top

Go:   strings.Repeat("ab", 3)
来源：http://mji.sufxvd.cn

Ruby: "ab" * 3
来源：http://jlm.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xxn.chenzaomai.com

[E03] 截取子串
来源：http://jjg.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jaf.jlsjyb.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rwr.shangyingyoupin.top


<!-- 参考信息 -->