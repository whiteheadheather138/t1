代发 wailian999

[C14] 泛型函数
来源：http://jma.iojbl.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hub.aizwys.cn

PHP:  // 无泛型
来源：http://tao.yfazqb.com

JS:   // 无泛型
来源：http://sys.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://vkx.shzxlz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xht.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fng.aibaodan.cn

Ruby: # 无泛型
来源：http://luf.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vdz.c1oappe.top

[C15] 解构 / 展开参数
来源：http://zym.birdmap.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yct.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://fgm.aizwys.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bms.xuanzx.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lgf.gaohongyu789.top

Java: // 无解构
来源：http://uku.gaohongyu789.top

Go:   // 无解构
来源：http://jni.aibaodan.cn

Ruby: a, b = pair
来源：http://heh.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://rrm.vehdjk.com

[C16] 函数 / 方法重载
来源：http://ghy.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zfx.daria6918.cn

PHP:  // 无重载
来源：http://emi.52xcode.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fbk.zhongyouzk.top

TS:   // 用联合类型或重载签名声明
来源：http://kwd.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://rcb.shanyushiyangkeji.top

Go:   // 无重载：用不同函数名
来源：http://dlm.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://kqg.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wlo.tianlin.xyz

================================================================================
来源：http://csr.yvedp.cn

D. 数组 / 列表 / 集合
来源：http://hzd.tarul.cn

================================================================================
来源：http://rgz.hammf.cn

[D01] 创建数组 / 列表
来源：http://vyt.sysykeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://icj.jlsjyb.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pzf.vqdsnc.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://eqc.jyoumei.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dks.jlsjyb.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vua.sxryk.cn

Go:   arr := []int{1, 2, 3}
来源：http://uzg.zhijiandao.cn

Ruby: arr = [1, 2, 3]
来源：http://klp.jinqigufen.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ryh.sxryk.cn

[D02] 追加元素到末尾
来源：http://wwz.uphjek.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kfr.sweek.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://grb.hesvh.cn

JS:   arr.push(4);
来源：http://dzg.316326.xyz

TS:   arr.push(4);
来源：http://auc.ybcxt.top

Java: list.add(4);
来源：http://dhs.quarkkingdee.top

Go:   arr = append(arr, 4)
来源：http://tpa.cqqwz.cn

Ruby: arr << 4; arr.push(5)
来源：http://mxy.cashguo.top

C#:   list.Add(4);
来源：http://qzj.gaohongyu789.top

[D03] 在指定位置插入元素
来源：http://ifx.yueranfly.top

Py:   arr.insert(0, 0)
来源：http://tge.hfpthk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://iwf.sysykeji.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xjh.sxryk.cn

TS:   arr.splice(0, 0, 0);
来源：http://jxs.tian-w.cn

Java: list.add(0, 0);
来源：http://kew.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://uuf.cashguo.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qsk.zhijiandao.cn

C#:   list.Insert(0, 0);
来源：http://nap.zhixingplan.top

[D04] 删除元素
来源：http://ghj.sjlbkw.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dqc.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://lvo.mhx1999.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sjz.snrcjt.cn

TS:   arr.splice(0, 1);
来源：http://svm.ywan-chungtsiang.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ppx.ctjpmb.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wxz.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vet.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nqn.zhengqikj.top

[D05] 访问与修改元素
来源：http://llv.ivvv.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://csu.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sqi.feifeiyinyue.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dtf.tanke756.top

TS:   arr[0]; arr.at(-1);
来源：http://ftw.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://xhi.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://cyr.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xbd.epnwcf.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hjk.iojbl.cn

[D06] 数组长度
来源：http://toz.guowangkeji.top

Py:   len(arr)
来源：http://wfv.zhoulong.xyz

PHP:  count($arr);
来源：http://gtf.yongpay.top

JS:   arr.length
来源：http://xby.52xcode.cn

TS:   arr.length
来源：http://rrx.fengsongda.top

Java: list.size();
来源：http://vap.ppjwa.cn

Go:   len(arr)
来源：http://cun.ydjk.org.cn

Ruby: arr.length; arr.size
来源：http://ywm.xingfuxueyuan.xyz

C#:   list.Count;
来源：http://ilh.yuxming.cn

[D07] 切片 / 取子数组
来源：http://kjo.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qxq.hcnkem.com

PHP:  array_slice($arr, 1, 3);
来源：http://ppe.jinyuanbaomall.cn

JS:   arr.slice(1, 4);
来源：http://xtj.shzxlz.cn

TS:   arr.slice(1, 4);
来源：http://ebo.pycfn.com

Java: list.subList(1, 4);
来源：http://ddz.xinyue.icu

Go:   arr[1:4]
来源：http://cop.quarkkingdee.top

Ruby: arr[1, 3]
来源：http://hmi.zhongyouzk.top

C#:   list.GetRange(1, 3);
来源：http://tmf.iojbl.cn

[D08] 合并两个数组
来源：http://lwu.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://irr.bbcook.cn

PHP:  array_merge($a, $b);
来源：http://utc.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ljt.iojbl.cn

TS:   [...a, ...b];
来源：http://wmd.guannengcc.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://her.quarkkingdee.top

Go:   append(a, b...)
来源：http://klu.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://mdy.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://aze.xuetiantiany.cn

[D09] 排序（升序）
来源：http://nxk.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://moe.fengsongda.top

PHP:  sort($arr);
来源：http://ktj.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zkj.bbcook.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hvw.hnqzz.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wla.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dav.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://hsb.hcnkem.com

C#:   list.Sort();
来源：http://uzo.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sud.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zno.0kj1m.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://acg.sweek.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://taz.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zan.zdqjudy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bnz.zdbjq.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ihv.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lud.yfazqb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ahx.fengsongda.top

[D11] 反转数组
来源：http://bcr.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://rdv.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://roa.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qkd.yuxming.cn

TS:   [...arr].reverse();
来源：http://tnl.mhx1999.top

Java: Collections.reverse(list);
来源：http://kkv.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://fwj.sjlbkw.cn

Ruby: arr.reverse
来源：http://frx.gzhubu.top

C#:   list.Reverse();
来源：http://anu.nwbrower.top

[D12] 查找元素下标
来源：http://pxy.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://byq.vqdsnc.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nme.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmk.chenzaomai.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gfw.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kai.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://ltj.bbcook.cn

Ruby: arr.index(x)
来源：http://dqd.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://ren.zhengqikj.top

[D13] 过滤（保留满足条件的）
来源：http://pgv.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zhl.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eht.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://xjx.epnwcf.com

TS:   arr.filter(x => x > 3)
来源：http://rtj.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wyl.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fng.yfazqb.com

Ruby: arr.select { |x| x > 3 }
来源：http://ede.cashguo.top

C#:   list.Where(x => x > 3).ToList()
来源：http://cfz.yvedp.cn

[D14] 映射转换（每个元素变形）
来源：http://hns.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tbs.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fuq.zdqjudy.top

JS:   arr.map(x => x * 2)
来源：http://rfv.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://wcw.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zvt.hammf.cn

Go:   // 手写循环
来源：http://nil.ivvv.top

Ruby: arr.map { |x| x * 2 }
来源：http://uqk.jlsjyb.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rfl.hnqzz.top

[D15] 去重
来源：http://cyv.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wzf.fktsv.cn

PHP:  array_unique($arr);
来源：http://jae.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://jik.tianlin.xyz

TS:   [...new Set(arr)]
来源：http://kuz.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hxm.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://mxu.andypj.xyz

Ruby: arr.uniq
来源：http://pkr.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://uuu.sysykeji.top

[D16] 求和与平均值
来源：http://ozm.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://smq.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://opa.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://edt.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dhu.meibo888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jbh.xylfe.cn

Go:   // 手写循环累加
来源：http://klb.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://waz.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://qak.cdnleiting.top

[D17] 最大值与最小值
来源：http://tny.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://nhf.daria6918.cn

PHP:  max($arr);  min($arr);
来源：http://cfl.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mxq.meibo888.top

TS:   Math.max(...arr);
来源：http://znf.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dpz.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jcn.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://wvk.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://yxy.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://gat.yj202588.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ewj.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://hpi.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jba.jlsjyb.cn

TS:   nested.flat();
来源：http://wco.aibaodan.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kgf.fanxiaobao.xyz

Go:   // 手写双层循环
来源：http://lih.cucudq.cn

Ruby: nested.flatten
来源：http://ozn.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://wdj.vehdjk.com

[D19] 按字段分组
来源：http://hjb.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fvv.zdbjq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fxn.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iak.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ldd.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lmq.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://xqt.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://iqq.aibaodan.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zwi.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://ylb.jqgfzy.top

Py:   Counter(arr)
来源：http://mcp.gogol.net.cn

PHP:  array_count_values($arr);
来源：http://trt.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hbw.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ibd.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lfb.yonumen.top

Go:   // 手写 map[T]int
来源：http://ztj.pengpengdd.cyou

Ruby: arr.tally
来源：http://wxv.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bup.ydzc1.top

[D21] 判断是否包含某元素
来源：http://taw.zhijiandao.cn

Py:   x in arr
来源：http://owk.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://rln.tanke756.top

JS:   arr.includes(x)
来源：http://jze.sufxvd.cn

TS:   arr.includes(x)
来源：http://dzc.shzxlz.cn

Java: list.contains(x)
来源：http://icq.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://lhc.cheryme.top

Ruby: arr.include?(x)
来源：http://avm.fengsongda.top

C#:   list.Contains(x)
来源：http://upk.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://yws.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cbu.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qgz.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uli.dianchejie.cn

TS:   [...arr];
来源：http://ovl.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://nol.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nyc.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://rmy.sweek.top

C#:   new List<int>(list);
来源：http://txt.wangshuangyany.cn

[D23] reduce 累积计算
来源：http://uvj.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zrd.jqgfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ntt.jyoumei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://egt.svipenyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovb.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cey.bbcook.cn

Go:   // 手写循环
来源：http://mrt.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kck.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hhy.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://esu.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fyu.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wxc.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rbc.hysaishi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ryn.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://imo.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tjg.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://asv.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aiv.nanxinkj.top

[D25] Set 集合去重与交并差
来源：http://xzr.chenjidiqi.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cqj.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cdj.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oxf.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gpy.pycfn.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sub.yuxming.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fwn.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nfe.feifeiyinyue.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uzj.havefunace.top

[D26] 数组转字符串
来源：http://xrr.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://eyl.havefunace.top

PHP:  implode(", ", $arr);
来源：http://thb.cheryme.top

JS:   arr.join(", ")
来源：http://sok.shuidangran.top

TS:   arr.join(", ")
来源：http://gxq.sweek.top

Java: String.join(", ", list)
来源：http://rdz.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://ckr.svipenyu.cn

Ruby: arr.join(", ")
来源：http://lge.gzhubu.top

C#:   string.Join(", ", list)
来源：http://oxb.snrcjt.cn

================================================================================
来源：http://can.cqqwz.cn

E. 字符串处理
来源：http://hue.c1oappe.top

================================================================================
来源：http://kcg.zhengqikj.top

[E01] 拼接字符串
来源：http://nlg.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wjy.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zty.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lob.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nua.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wom.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://afr.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kxo.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dyq.xziqi.cn

[E02] 重复字符串
来源：http://lgy.vqdsnc.cn

Py:   "ab" * 3
来源：http://wrp.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://iqu.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://oab.yfazqb.com

TS:   "ab".repeat(3)
来源：http://mxu.ppjwa.cn

Java: "ab".repeat(3)
来源：http://agb.zhaomingkeji.xyz

Go:   strings.Repeat("ab", 3)
来源：http://srs.jinqigfzy.top

Ruby: "ab" * 3
来源：http://nzk.birdmap.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jtw.jyoumei.cn

[E03] 截取子串
来源：http://zuh.yj20258888.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bqg.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dmd.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jaf.sweek.top

TS:   s.slice(1, 4)
来源：http://njv.fzhhl.top

Java: s.substring(1, 4)
来源：http://dyg.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blo.daxiang520.top

Ruby: s[1, 3];  s[1..3]
来源：http://jrw.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://ysd.guowangkeji.top

[E04] 查找子串位置
来源：http://jgf.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://ayl.redwolf501.top

PHP:  strpos($s, "x");
来源：http://fdk.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vgg.andypj.xyz

TS:   s.indexOf("x")
来源：http://bcz.snrcjt.cn

Java: s.indexOf("x")
来源：http://wan.yfazqb.com


<!-- 参考信息 -->