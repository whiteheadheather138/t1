代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://pbk.ivvv.top

Ruby: -> { puts "run" }.call
来源：http://snb.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ppb.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://glp.mhx1999.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dkn.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvu.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kiu.hysaishi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oae.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://hpm.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://jcj.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wfc.fengsongda.top

C#:   int Add(int a, int b) => a + b;
来源：http://pkp.zdbjq.cn

[C14] 泛型函数
来源：http://dar.smart0.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://erb.yj202588.top

PHP:  // 无泛型
来源：http://vmd.ydjk.org.cn

JS:   // 无泛型
来源：http://egi.pycfn.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gxu.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ovv.jqgufenzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rdd.yuxming.cn

Ruby: # 无泛型
来源：http://apz.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xsa.zhongyouzk.top

[C15] 解构 / 展开参数
来源：http://hoh.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://klr.zdqjudy.top

PHP:  [$a, $b] = $pair;
来源：http://mgj.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://svk.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ejk.52xcode.cn

Java: // 无解构
来源：http://uww.jinghuilouyu.cn

Go:   // 无解构
来源：http://dtn.aibaodan.cn

Ruby: a, b = pair
来源：http://poz.iojbl.cn

C#:   var (a, b) = pair;
来源：http://esc.zhaomingkeji.xyz

[C16] 函数 / 方法重载
来源：http://ybk.kuanghao11.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kdy.jianghu66.top

PHP:  // 无重载
来源：http://vto.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uhm.svipenyu.cn

TS:   // 用联合类型或重载签名声明
来源：http://jmd.yuanzhike.top

Java: void f(int a) {}  void f(String a) {}
来源：http://uyj.yonumen.top

Go:   // 无重载：用不同函数名
来源：http://fiu.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://ygu.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://eas.shanyushiyangtech.top

================================================================================
来源：http://abq.pengpengdd.cyou

D. 数组 / 列表 / 集合
来源：http://vdg.gzhubu.top

================================================================================
来源：http://aak.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://pfw.xuetiantiany.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://oqf.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fyw.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zwb.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://nox.sufxvd.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bux.snrcjt.cn

Go:   arr := []int{1, 2, 3}
来源：http://ujc.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://dkc.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mxk.gotoacloud.top

[D02] 追加元素到末尾
来源：http://rrh.xylfe.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jth.uphjek.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://crr.yfazqb.com

JS:   arr.push(4);
来源：http://fjk.tianlin.xyz

TS:   arr.push(4);
来源：http://suq.fzhhl.top

Java: list.add(4);
来源：http://byu.daria6918.cn

Go:   arr = append(arr, 4)
来源：http://tpj.aibaodan.cn

Ruby: arr << 4; arr.push(5)
来源：http://qof.zhaomingkeji.xyz

C#:   list.Add(4);
来源：http://gmf.xuanzx.com

[D03] 在指定位置插入元素
来源：http://bnf.feifeiyinyue.top

Py:   arr.insert(0, 0)
来源：http://gwt.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cum.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wdd.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://vjh.ybcxt.top

Java: list.add(0, 0);
来源：http://vka.guannengcc.top

Go:   arr = append([]int{0}, arr...)
来源：http://etb.kuanghao11.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lfq.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://fxb.vehdjk.com

[D04] 删除元素
来源：http://ltd.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cny.gotoacloud.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xst.epnwcf.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lur.dianchejie.cn

TS:   arr.splice(0, 1);
来源：http://znw.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xuj.zdbjq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://peu.zhongyouzk.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dmq.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lsg.yj20258.top

[D05] 访问与修改元素
来源：http://led.jyoumei.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://iyl.nanxuanxn.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://lld.vqdsnc.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://okw.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://idn.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://pec.yj20258888.top

Go:   arr[0]; arr[0] = 9
来源：http://nev.jiagoushi.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rhm.316326.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bly.zhongyouzk.top

[D06] 数组长度
来源：http://owh.jianghu66.top

Py:   len(arr)
来源：http://meo.wangdashe.top

PHP:  count($arr);
来源：http://pde.nanxuanxn.top

JS:   arr.length
来源：http://gdg.yj20258888.top

TS:   arr.length
来源：http://laj.guannengcc.top

Java: list.size();
来源：http://vea.yonumen.top

Go:   len(arr)
来源：http://gmw.yfazqb.com

Ruby: arr.length; arr.size
来源：http://zwb.tanke756.top

C#:   list.Count;
来源：http://eay.aibaodan.cn

[D07] 切片 / 取子数组
来源：http://dfc.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gaj.zdbjq.cn

PHP:  array_slice($arr, 1, 3);
来源：http://nli.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://bkv.aizwys.cn

TS:   arr.slice(1, 4);
来源：http://ofv.yj202588.top

Java: list.subList(1, 4);
来源：http://lqn.jlsjyb.cn

Go:   arr[1:4]
来源：http://zwj.redwolf501.top

Ruby: arr[1, 3]
来源：http://yvd.c1oappe.top

C#:   list.GetRange(1, 3);
来源：http://dhj.xziqi.cn

[D08] 合并两个数组
来源：http://zoy.sxryk.cn

Py:   a + b;  a.extend(b)
来源：http://osu.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://lhw.smart0.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://qga.zycfv.cn

TS:   [...a, ...b];
来源：http://goc.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vdv.pycfn.com

Go:   append(a, b...)
来源：http://jjx.zdqjudy.top

Ruby: a + b;  a.concat(b)
来源：http://zqy.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://xua.zhixingplan.top

[D09] 排序（升序）
来源：http://csg.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://uat.pycfn.com

PHP:  sort($arr);
来源：http://ekx.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gky.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dlv.fktsv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gaj.dashuyun.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ver.gotoacloud.top

Ruby: arr.sort
来源：http://vyn.hfpthk.cn

C#:   list.Sort();
来源：http://fji.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://uum.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pml.yuxming.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wwr.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xoi.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ytd.svipenyu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cmk.xuetiantiany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://okj.xziqi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ahr.dashuyun.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rnp.ydzc1.top

[D11] 反转数组
来源：http://gqx.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://wcp.c1oappe.top

PHP:  array_reverse($arr);
来源：http://kdi.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://klp.hnqzz.top

TS:   [...arr].reverse();
来源：http://wmj.wangshuangyany.cn

Java: Collections.reverse(list);
来源：http://kfb.epnwcf.com

Go:   slices.Reverse(arr)
来源：http://llv.iojbl.cn

Ruby: arr.reverse
来源：http://kso.jinqigufen.top

C#:   list.Reverse();
来源：http://fnb.shangyingyoupin.top

[D12] 查找元素下标
来源：http://epo.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://edu.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zkq.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tti.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bdb.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://luf.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://cee.andypj.xyz

Ruby: arr.index(x)
来源：http://ukq.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://ldv.ywan-chungtsiang.top

[D13] 过滤（保留满足条件的）
来源：http://ttw.zhongyouzk.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dka.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dfj.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://use.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://ozq.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zxg.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gwk.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://jov.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pbw.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://aux.jinqigufen.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dui.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vlg.nanxuanxn.top

JS:   arr.map(x => x * 2)
来源：http://rdu.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://gmv.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dkx.yvedp.cn

Go:   // 手写循环
来源：http://bau.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vdb.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wlw.uphjek.com

[D15] 去重
来源：http://sza.feifeiyinyue.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xfk.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://ymu.quarkkingdee.top

JS:   [...new Set(arr)]
来源：http://tki.yvedp.cn

TS:   [...new Set(arr)]
来源：http://zow.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cnd.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://adg.yanxiufei.cn

Ruby: arr.uniq
来源：http://nla.jianghu66.top

C#:   list.Distinct().ToList()
来源：http://pij.epnwcf.com

[D16] 求和与平均值
来源：http://cpa.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cyw.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dlc.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vqd.cqqwz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ymh.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zpg.9152youxi.cn

Go:   // 手写循环累加
来源：http://etu.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pdm.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://tcy.yanxiufei.cn

[D17] 最大值与最小值
来源：http://crm.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://xye.ywan-chungtsiang.top

PHP:  max($arr);  min($arr);
来源：http://sfw.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lqo.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://cwt.yj20258.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ftu.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ike.sufxvd.cn

Ruby: arr.max;  arr.min
来源：http://mzi.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://sdq.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://gns.ydjk.org.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://apk.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://tju.shanyushiyangkeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bmo.smart0.xyz

TS:   nested.flat();
来源：http://gxd.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pbp.dashuyun.cn

Go:   // 手写双层循环
来源：http://pex.nanxuanxn.top

Ruby: nested.flatten
来源：http://vuo.yonumen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xqu.daxiang520.top

[D19] 按字段分组
来源：http://ruk.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sek.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vdn.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fid.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://jtg.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ial.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://jzy.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mnz.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gau.cashguo.top

[D20] 统计每个元素出现次数
来源：http://qam.sufxvd.cn

Py:   Counter(arr)
来源：http://dwd.birdmap.top

PHP:  array_count_values($arr);
来源：http://qxr.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blb.cucudq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oqt.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xru.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://cjp.yonumen.top

Ruby: arr.tally
来源：http://egp.sxryk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ivr.snrcjt.cn

[D21] 判断是否包含某元素
来源：http://oeh.yangfankeji.com

Py:   x in arr
来源：http://zkk.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://grq.andypj.xyz

JS:   arr.includes(x)
来源：http://xec.guowangkeji.top

TS:   arr.includes(x)
来源：http://opw.kuanghao11.cn

Java: list.contains(x)
来源：http://rio.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://ewq.feifeiyinyue.top

Ruby: arr.include?(x)
来源：http://jas.gaohongyu789.top

C#:   list.Contains(x)
来源：http://dqd.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://eaf.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hgn.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dux.hfpthk.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mhe.hnqzz.top

TS:   [...arr];
来源：http://pva.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://yak.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://wsf.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://ayo.meibo888.top

C#:   new List<int>(list);
来源：http://ztm.daxiang520.top

[D23] reduce 累积计算
来源：http://ptw.jinqigufen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jmv.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sgr.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxu.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lzs.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vmb.bbcook.cn

Go:   // 手写循环
来源：http://zof.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jky.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dsg.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://nms.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://udt.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ium.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tik.fengsongda.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zve.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rtx.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ten.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://unl.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://evb.wangdashe.top

[D25] Set 集合去重与交并差
来源：http://rem.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zco.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uze.fzhhl.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zvn.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hjy.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bho.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xxf.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jlg.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lde.ehwqpu.com

[D26] 数组转字符串
来源：http://zie.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://czo.jinqigfzy.top

PHP:  implode(", ", $arr);
来源：http://jdi.aizwys.cn

JS:   arr.join(", ")
来源：http://exh.shzxlz.cn

TS:   arr.join(", ")
来源：http://srk.xylfe.cn

Java: String.join(", ", list)
来源：http://umy.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://pfc.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://ory.fengsongda.top

C#:   string.Join(", ", list)
来源：http://jim.nanxinkj.top

================================================================================
来源：http://yat.guannengcc.top

E. 字符串处理
来源：http://een.kuanghao11.cn

================================================================================
来源：http://dqp.hnqzz.top

[E01] 拼接字符串
来源：http://guu.meibo888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eti.bjfxy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jbj.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rru.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://alf.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gvh.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ror.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uex.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tvb.ybcxt.top

[E02] 重复字符串
来源：http://psr.redwolf501.top

Py:   "ab" * 3
来源：http://qmq.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://ohd.zhengqikj.top

JS:   "ab".repeat(3)
来源：http://cvc.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://vik.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://cer.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://ocz.xylfe.cn

Ruby: "ab" * 3
来源：http://hjy.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bku.birdmap.top

[E03] 截取子串
来源：http://fji.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rru.zhongyouzk.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bka.sysykeji.top


<!-- 参考信息 -->