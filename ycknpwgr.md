代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hwr.nanxinkj.top

Go:   func add(a, b int) int
来源：http://fjf.fzhhl.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mei.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dzf.aibaodan.cn

[C14] 泛型函数
来源：http://tgu.guannengcc.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://egm.zhixingplan.top

PHP:  // 无泛型
来源：http://vda.hfpthk.cn

JS:   // 无泛型
来源：http://ozu.meibo888.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mvj.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gnf.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mtd.hongshengwenyu.top

Ruby: # 无泛型
来源：http://lyo.guowangkeji.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://aoq.52xcode.cn

[C15] 解构 / 展开参数
来源：http://bpu.shzxlz.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lbg.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://ahh.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ifi.yonumen.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mez.cdnleiting.top

Java: // 无解构
来源：http://uat.chenzaomai.com

Go:   // 无解构
来源：http://cdi.sxryk.cn

Ruby: a, b = pair
来源：http://abk.hcnkem.com

C#:   var (a, b) = pair;
来源：http://bdw.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://lzn.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pgt.zhongyouzk.top

PHP:  // 无重载
来源：http://qhq.sjlbkw.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mbe.daria6918.cn

TS:   // 用联合类型或重载签名声明
来源：http://xqy.sjlbkw.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zpm.hnxiangtu.top

Go:   // 无重载：用不同函数名
来源：http://off.meibo888.top

Ruby: # 无重载：靠动态参数
来源：http://xsj.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://xdn.zhongyouzk.top

================================================================================
来源：http://diz.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://kxf.shuidangran.top

================================================================================
来源：http://txo.tianlin.xyz

[D01] 创建数组 / 列表
来源：http://wfy.gotoacloud.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://osu.guannengcc.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://phm.bbcook.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ept.sysykeji.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://htp.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lzo.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://tjt.daxiang520.top

Ruby: arr = [1, 2, 3]
来源：http://wze.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://duw.redwolf501.top

[D02] 追加元素到末尾
来源：http://gha.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qzk.gogol.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nvi.zhijiandao.cn

JS:   arr.push(4);
来源：http://toe.xuanzx.com

TS:   arr.push(4);
来源：http://brk.bbcook.cn

Java: list.add(4);
来源：http://fmr.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://vyq.quarkkingdee.top

Ruby: arr << 4; arr.push(5)
来源：http://fut.gotoacloud.top

C#:   list.Add(4);
来源：http://qsk.bbcook.cn

[D03] 在指定位置插入元素
来源：http://nrn.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://rhj.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hlg.zhixingplan.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sma.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://juv.nwbrower.top

Java: list.add(0, 0);
来源：http://pxq.jqgfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://fni.gotoacloud.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oyz.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://uvf.chenjidiqi.icu

[D04] 删除元素
来源：http://cfk.jinyuanbaomall.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://swz.yueranfly.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sxm.jlsjyb.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://vsh.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://sju.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://lcd.yangfankeji.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zdg.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vtq.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hel.nwbrower.top

[D05] 访问与修改元素
来源：http://kyn.jinqigufen.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://opi.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wkr.quarkkingdee.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gxl.hywenlv.cn

TS:   arr[0]; arr.at(-1);
来源：http://rev.fengsongda.top

Java: list.get(0); list.set(0, 9);
来源：http://bmh.tian-w.cn

Go:   arr[0]; arr[0] = 9
来源：http://lsp.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wei.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yhy.redwolf501.top

[D06] 数组长度
来源：http://csk.haohaochexian.top

Py:   len(arr)
来源：http://sub.haohaochexian.top

PHP:  count($arr);
来源：http://ryg.hongshengwenyu.top

JS:   arr.length
来源：http://twu.zhengqikj.top

TS:   arr.length
来源：http://act.zhoulong.xyz

Java: list.size();
来源：http://kxr.ybcxt.top

Go:   len(arr)
来源：http://ytw.nwbrower.top

Ruby: arr.length; arr.size
来源：http://uze.andypj.xyz

C#:   list.Count;
来源：http://tnk.quarkkingdee.top

[D07] 切片 / 取子数组
来源：http://wkn.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://asi.shangyingyoupin.top

PHP:  array_slice($arr, 1, 3);
来源：http://ocd.yuanzhike.top

JS:   arr.slice(1, 4);
来源：http://mti.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://lnl.zycfv.cn

Java: list.subList(1, 4);
来源：http://kgx.hywenlv.cn

Go:   arr[1:4]
来源：http://nob.daria6918.cn

Ruby: arr[1, 3]
来源：http://pxj.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://qpo.9152youxi.cn

[D08] 合并两个数组
来源：http://hvi.fanxiaobao.xyz

Py:   a + b;  a.extend(b)
来源：http://jtj.jlsjyb.cn

PHP:  array_merge($a, $b);
来源：http://pec.ybcxt.top

JS:   [...a, ...b];  a.concat(b);
来源：http://obc.guowangkeji.top

TS:   [...a, ...b];
来源：http://uaa.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dud.daria6918.cn

Go:   append(a, b...)
来源：http://qgh.uphjek.com

Ruby: a + b;  a.concat(b)
来源：http://zet.pycfn.com

C#:   a.Concat(b).ToList()
来源：http://nnp.sjlbkw.cn

[D09] 排序（升序）
来源：http://hql.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://yps.nwbrower.top

PHP:  sort($arr);
来源：http://ola.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ene.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dlr.daria6918.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uvu.chenjidiqi.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fvw.iojbl.cn

Ruby: arr.sort
来源：http://njo.yfazqb.com

C#:   list.Sort();
来源：http://iip.zycfv.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ekj.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://apw.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xht.chenzaomai.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mtr.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gge.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vxr.hywenlv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://acu.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eco.xuanzx.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://olf.sweek.top

[D11] 反转数组
来源：http://khf.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://wwh.yvedp.cn

PHP:  array_reverse($arr);
来源：http://jee.feifeiyinyue.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://duv.9152youxi.cn

TS:   [...arr].reverse();
来源：http://xls.shzxlz.cn

Java: Collections.reverse(list);
来源：http://mcv.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://ahl.shanyushiyangtech.top

Ruby: arr.reverse
来源：http://num.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://ont.cucudq.cn

[D12] 查找元素下标
来源：http://ovk.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://lfd.aibaodan.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dkl.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rze.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nxp.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yoc.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://lzw.sysykeji.top

Ruby: arr.index(x)
来源：http://qvb.uphjek.com

C#:   list.IndexOf(x);
来源：http://goz.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://bhj.hcnkem.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ced.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zji.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://dee.chenjidiqi.icu

TS:   arr.filter(x => x > 3)
来源：http://nkf.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tim.daxiang520.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bvx.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://ota.yj202588.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ias.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://jvj.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qxn.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zwb.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://ars.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://vmq.yonumen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://szt.gotoacloud.top

Go:   // 手写循环
来源：http://cvt.cdnleiting.top

Ruby: arr.map { |x| x * 2 }
来源：http://sku.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cqg.birdmap.top

[D15] 去重
来源：http://zwk.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yul.yvedp.cn

PHP:  array_unique($arr);
来源：http://grc.yonumen.top

JS:   [...new Set(arr)]
来源：http://hoh.jinqigufen.top

TS:   [...new Set(arr)]
来源：http://mzk.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qni.jinghuilouyu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oii.hesvh.cn

Ruby: arr.uniq
来源：http://jgl.uphjek.com

C#:   list.Distinct().ToList()
来源：http://sqi.tianlin.xyz

[D16] 求和与平均值
来源：http://bdo.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xek.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://grv.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pfn.fehbvm.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://abt.aizwys.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://smn.nwbrower.top

Go:   // 手写循环累加
来源：http://lhb.jinqigfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cfn.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://mdh.nwbrower.top

[D17] 最大值与最小值
来源：http://cgn.birdmap.top

Py:   max(arr);  min(arr)
来源：http://ezo.smart0.xyz

PHP:  max($arr);  min($arr);
来源：http://dfk.cheryme.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://guh.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://rcp.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ckp.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ndn.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://vyf.gzhubu.top

C#:   list.Max();  list.Min()
来源：http://wtg.uphjek.com

[D18] 扁平化嵌套数组
来源：http://zgj.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qje.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://zwo.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qqz.yj202588.top

TS:   nested.flat();
来源：http://lpu.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ypa.yongpay.top

Go:   // 手写双层循环
来源：http://tho.daria6918.cn

Ruby: nested.flatten
来源：http://ieb.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rov.wangshuangyany.cn

[D19] 按字段分组
来源：http://gpf.xingfuxueyuan.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yxo.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dbd.shanyushiyangtech.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pml.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bii.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qxm.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://asm.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vle.birdmap.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mga.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://ayj.tian-w.cn

Py:   Counter(arr)
来源：http://vqn.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://gfm.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pzx.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://phl.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ald.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://wmm.vqdsnc.cn

Ruby: arr.tally
来源：http://sqf.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qsd.xinyue.icu

[D21] 判断是否包含某元素
来源：http://wub.fanxiaobao.xyz

Py:   x in arr
来源：http://dch.ybcxt.top

PHP:  in_array($x, $arr, true);
来源：http://efo.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://qqu.birdmap.top

TS:   arr.includes(x)
来源：http://ziy.dashuyun.cn

Java: list.contains(x)
来源：http://ukj.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://dqv.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://saa.yonumen.top

C#:   list.Contains(x)
来源：http://jhy.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://eju.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jnk.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tdi.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ygd.yuxming.cn

TS:   [...arr];
来源：http://hpp.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://enj.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dlz.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://vww.fktsv.cn

C#:   new List<int>(list);
来源：http://etw.xinyue.icu

[D23] reduce 累积计算
来源：http://ibr.cheryme.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vqk.andypj.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rkx.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gsc.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msq.yfazqb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ohk.yuxming.cn

Go:   // 手写循环
来源：http://rxa.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zvl.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gkt.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://pcc.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ita.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zok.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbf.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://onv.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yur.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bos.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ecz.jiagoushi.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gtp.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://wni.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://akr.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jov.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gvf.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mbu.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://brb.yonumen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jdh.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dft.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gvu.aibaodan.cn

[D26] 数组转字符串
来源：http://wun.dianchejie.cn

Py:   ", ".join(map(str, arr))
来源：http://fix.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://zeq.uphjek.com

JS:   arr.join(", ")
来源：http://jbo.guowangkeji.top

TS:   arr.join(", ")
来源：http://cze.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://xco.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://jmg.gzhubu.top

Ruby: arr.join(", ")
来源：http://yfz.yvedp.cn

C#:   string.Join(", ", list)
来源：http://svh.daria6918.cn

================================================================================
来源：http://goi.wangshuangyany.cn

E. 字符串处理
来源：http://pbf.redwolf501.top

================================================================================
来源：http://qwo.xylfe.cn

[E01] 拼接字符串
来源：http://lws.jlsjyb.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xkp.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uft.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jzf.0kj1m.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nex.hysaishi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://isp.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://whg.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cke.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://agv.hnxiangtu.top

[E02] 重复字符串
来源：http://gqu.fengsongda.top

Py:   "ab" * 3
来源：http://oev.yj202588.top

PHP:  str_repeat("ab", 3);
来源：http://ufy.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://xjt.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://ygc.tanke756.top

Java: "ab".repeat(3)
来源：http://eam.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://pxi.gotoacloud.top

Ruby: "ab" * 3
来源：http://nkk.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fbt.gogol.net.cn

[E03] 截取子串
来源：http://qqr.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zfa.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ifl.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mpf.ydzc1.top

TS:   s.slice(1, 4)
来源：http://jef.bjfxy.top

Java: s.substring(1, 4)
来源：http://pxg.tarul.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wps.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wzb.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://uds.0kj1m.cn

[E04] 查找子串位置
来源：http://zei.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://dgw.birdmap.top


<!-- 参考信息 -->