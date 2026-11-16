代发 wailian999

[C14] 泛型函数
来源：http://vwj.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bor.wangdashe.top

PHP:  // 无泛型
来源：http://rsj.cqqwz.cn

JS:   // 无泛型
来源：http://tay.pengpengdd.cyou

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wdj.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tec.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tgo.tian-w.cn

Ruby: # 无泛型
来源：http://wjj.zhongyouzk.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ezr.epnwcf.com

[C15] 解构 / 展开参数
来源：http://qlx.yongpay.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://com.zhijiandao.cn

PHP:  [$a, $b] = $pair;
来源：http://rrt.zhiwuduotai.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qox.sysykeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zfv.cucudq.cn

Java: // 无解构
来源：http://ovm.zhoulong.xyz

Go:   // 无解构
来源：http://lpo.aizwys.cn

Ruby: a, b = pair
来源：http://mmb.jqgfzy.top

C#:   var (a, b) = pair;
来源：http://xey.ywan-chungtsiang.top

[C16] 函数 / 方法重载
来源：http://jwi.ydzc1.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lrf.smart0.xyz

PHP:  // 无重载
来源：http://fpa.dianchejie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nrt.kuanghao11.cn

TS:   // 用联合类型或重载签名声明
来源：http://hoz.smart0.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://uti.c1oappe.top

Go:   // 无重载：用不同函数名
来源：http://svx.shuidangran.top

Ruby: # 无重载：靠动态参数
来源：http://uwx.hongshengwenyu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lgv.fzhhl.top

================================================================================
来源：http://ext.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://hyf.yongpay.top

================================================================================
来源：http://hvu.daxiang520.top

[D01] 创建数组 / 列表
来源：http://ami.shuidangran.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://jxm.ybcxt.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qun.fzhhl.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ceg.cucudq.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cfy.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ckr.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://mzo.xinyue.icu

Ruby: arr = [1, 2, 3]
来源：http://sqo.hywenlv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jth.yuxming.cn

[D02] 追加元素到末尾
来源：http://jpx.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cir.jianghu66.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cfw.cashguo.top

JS:   arr.push(4);
来源：http://yec.dianchejie.cn

TS:   arr.push(4);
来源：http://etc.havefunace.top

Java: list.add(4);
来源：http://vjv.hnqzz.top

Go:   arr = append(arr, 4)
来源：http://zai.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://njc.fanxiaobao.xyz

C#:   list.Add(4);
来源：http://vfi.shanyushiyangtech.top

[D03] 在指定位置插入元素
来源：http://pul.cdnleiting.top

Py:   arr.insert(0, 0)
来源：http://cko.ctjpmb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jxw.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qkf.yj202588.top

TS:   arr.splice(0, 0, 0);
来源：http://aue.316326.xyz

Java: list.add(0, 0);
来源：http://sof.redwolf501.top

Go:   arr = append([]int{0}, arr...)
来源：http://vst.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lkb.cucudq.cn

C#:   list.Insert(0, 0);
来源：http://zdu.gzhubu.top

[D04] 删除元素
来源：http://yxz.chenzaomai.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tox.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dri.yangfankeji.com

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ovv.cucudq.cn

TS:   arr.splice(0, 1);
来源：http://pvn.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vlm.jinghuilouyu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ywd.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uuo.andypj.xyz

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pxd.zhengqikj.top

[D05] 访问与修改元素
来源：http://itw.cucudq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pwh.havefunace.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qqt.haohaochexian.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://szw.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://yhx.xuetiantiany.cn

Java: list.get(0); list.set(0, 9);
来源：http://whf.zdqjudy.top

Go:   arr[0]; arr[0] = 9
来源：http://xhf.guannengcc.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qqv.hammf.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hvo.pengpengdd.cyou

[D06] 数组长度
来源：http://rsg.yueranfly.top

Py:   len(arr)
来源：http://hda.chenzaomai.com

PHP:  count($arr);
来源：http://foc.feifeiyinyue.top

JS:   arr.length
来源：http://dxo.jinqigfzy.top

TS:   arr.length
来源：http://xhb.jianghu66.top

Java: list.size();
来源：http://xci.zhengqikj.top

Go:   len(arr)
来源：http://atj.ctjpmb.com

Ruby: arr.length; arr.size
来源：http://cox.chenlongwang.top

C#:   list.Count;
来源：http://iav.chenzaomai.com

[D07] 切片 / 取子数组
来源：http://fbb.jinqigufen.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cct.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://jhl.yongpay.top

JS:   arr.slice(1, 4);
来源：http://mud.ybcxt.top

TS:   arr.slice(1, 4);
来源：http://dgz.iojbl.cn

Java: list.subList(1, 4);
来源：http://mwk.chenlongwang.top

Go:   arr[1:4]
来源：http://oxa.316326.xyz

Ruby: arr[1, 3]
来源：http://tqf.hywenlv.cn

C#:   list.GetRange(1, 3);
来源：http://mcl.redwolf501.top

[D08] 合并两个数组
来源：http://mjg.yonumen.top

Py:   a + b;  a.extend(b)
来源：http://mky.jianghu66.top

PHP:  array_merge($a, $b);
来源：http://xrh.jiagoushi.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jpy.hcnkem.com

TS:   [...a, ...b];
来源：http://sru.dashuyun.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yhg.sufxvd.cn

Go:   append(a, b...)
来源：http://suj.cqqwz.cn

Ruby: a + b;  a.concat(b)
来源：http://ksz.sysykeji.top

C#:   a.Concat(b).ToList()
来源：http://ofl.nwbrower.top

[D09] 排序（升序）
来源：http://zfn.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://gts.nanxinkj.top

PHP:  sort($arr);
来源：http://mof.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wfu.fzhhl.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ves.zhaomingkeji.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://byw.yonumen.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dcu.mhx1999.top

Ruby: arr.sort
来源：http://xhl.yj20258.top

C#:   list.Sort();
来源：http://chd.yuxming.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://mmx.tarul.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nlp.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lmj.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://knt.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ikh.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wai.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lcj.guowangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xgg.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vxf.cheryme.top

[D11] 反转数组
来源：http://pye.uphjek.com

Py:   arr[::-1];  arr.reverse()
来源：http://vgf.tanke756.top

PHP:  array_reverse($arr);
来源：http://yhy.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ufq.cdnleiting.top

TS:   [...arr].reverse();
来源：http://whi.fktsv.cn

Java: Collections.reverse(list);
来源：http://hpi.gogol.net.cn

Go:   slices.Reverse(arr)
来源：http://drq.xziqi.cn

Ruby: arr.reverse
来源：http://gts.pycfn.com

C#:   list.Reverse();
来源：http://gre.quarkkingdee.top

[D12] 查找元素下标
来源：http://aav.snrcjt.cn

Py:   arr.index(x);  x in arr
来源：http://gko.hysaishi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cmd.jinyuanbaomall.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pcj.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lve.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vxy.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://avk.yj20258888.top

Ruby: arr.index(x)
来源：http://ivg.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://spf.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://rda.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bsv.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cet.shangyingyoupin.top

JS:   arr.filter(x => x > 3)
来源：http://cbl.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://dcw.9152youxi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ulq.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tsc.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://aev.ywan-chungtsiang.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qvz.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://shq.jinqigfzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tsv.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pfi.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://mti.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://xpi.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kdk.ppjwa.cn

Go:   // 手写循环
来源：http://evn.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://ioa.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gyx.zhongyouzk.top

[D15] 去重
来源：http://smt.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fyh.jianghu66.top

PHP:  array_unique($arr);
来源：http://pho.zycfv.cn

JS:   [...new Set(arr)]
来源：http://iby.xziqi.cn

TS:   [...new Set(arr)]
来源：http://uuz.chenzaomai.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cbk.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://ttw.chenjidiqi.icu

Ruby: arr.uniq
来源：http://wvq.chenzaomai.com

C#:   list.Distinct().ToList()
来源：http://xso.52xcode.cn

[D16] 求和与平均值
来源：http://ksv.cheryme.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qcx.cashguo.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://heg.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwg.zhengqikj.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ioy.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://faf.sjlbkw.cn

Go:   // 手写循环累加
来源：http://tnp.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hgf.ywan-chungtsiang.top

C#:   list.Sum();  list.Average()
来源：http://qko.c1oappe.top

[D17] 最大值与最小值
来源：http://kjl.zhengqikj.top

Py:   max(arr);  min(arr)
来源：http://rer.shuidangran.top

PHP:  max($arr);  min($arr);
来源：http://jxm.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://igz.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://azf.0kj1m.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hpv.jinyuanbaomall.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vlq.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://hju.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://pav.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://txg.yonumen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hlw.yj20258.top

PHP:  array_merge(...$nested);
来源：http://pqu.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://buq.nanxuanxn.top

TS:   nested.flat();
来源：http://qha.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jkq.birdmap.top

Go:   // 手写双层循环
来源：http://vzo.yonumen.top

Ruby: nested.flatten
来源：http://hgn.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://ixk.chenlongwang.top

[D19] 按字段分组
来源：http://csj.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ghg.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bbr.jqgufenzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pxi.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tgf.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pxa.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://dfk.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wnz.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://raw.0kj1m.cn

[D20] 统计每个元素出现次数
来源：http://mmk.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://lqp.hcnkem.com

PHP:  array_count_values($arr);
来源：http://xzk.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cys.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://iov.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mpz.aizwys.cn

Go:   // 手写 map[T]int
来源：http://uyn.shzxlz.cn

Ruby: arr.tally
来源：http://kdq.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pty.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://fts.pycfn.com

Py:   x in arr
来源：http://fon.hywenlv.cn

PHP:  in_array($x, $arr, true);
来源：http://wgh.fehbvm.com

JS:   arr.includes(x)
来源：http://ivy.hongshengwenyu.top

TS:   arr.includes(x)
来源：http://tpo.sxryk.cn

Java: list.contains(x)
来源：http://nrq.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://riq.pycfn.com

Ruby: arr.include?(x)
来源：http://wku.daxiang520.top

C#:   list.Contains(x)
来源：http://cge.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://iam.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qwm.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rta.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nez.hnxiangtu.top

TS:   [...arr];
来源：http://jkp.jyoumei.cn

Java: new ArrayList<>(list);
来源：http://xat.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://ytk.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://ppr.zhengqikj.top

C#:   new List<int>(list);
来源：http://sta.ctjpmb.com

[D23] reduce 累积计算
来源：http://doc.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lkk.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mnx.gaohongyu789.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wdp.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nou.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://eso.jqgfzy.top

Go:   // 手写循环
来源：http://nhu.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://msj.jinqigfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cvy.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://hzq.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qws.jinyuanbaomall.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zxq.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cwd.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ywq.jinghuilouyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ext.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://apm.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://twk.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cdu.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://agg.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nml.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wei.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dgc.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://osy.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mte.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://uoe.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nte.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://has.tian-w.cn

[D26] 数组转字符串
来源：http://csg.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://fwm.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://dkw.guowangkeji.top

JS:   arr.join(", ")
来源：http://zyc.cheryme.top

TS:   arr.join(", ")
来源：http://hoy.nwbrower.top

Java: String.join(", ", list)
来源：http://gqf.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://uet.wangdashe.top

Ruby: arr.join(", ")
来源：http://jly.cucudq.cn

C#:   string.Join(", ", list)
来源：http://ura.sweek.top

================================================================================
来源：http://jgz.zhongyouzk.top

E. 字符串处理
来源：http://auf.tianlin.xyz

================================================================================
来源：http://ecm.ctjpmb.com

[E01] 拼接字符串
来源：http://bam.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hrr.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fyh.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dxq.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mzx.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gnu.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ztm.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wwd.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qxx.kuanghao11.cn

[E02] 重复字符串
来源：http://fig.nwbrower.top

Py:   "ab" * 3
来源：http://bdy.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://nlb.shanyushiyangtech.top

JS:   "ab".repeat(3)
来源：http://fny.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://jdp.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://rcz.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://vyg.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://hxb.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yzv.havefunace.top

[E03] 截取子串
来源：http://bsx.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uui.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wyg.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gnz.yvedp.cn

TS:   s.slice(1, 4)
来源：http://lvb.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://pqa.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://peo.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://cdx.52xcode.cn

C#:   s.Substring(1, 3)
来源：http://laj.aibaodan.cn

[E04] 查找子串位置
来源：http://qap.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://qgd.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://onx.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yzj.yonumen.top

TS:   s.indexOf("x")
来源：http://nuk.hywenlv.cn

Java: s.indexOf("x")
来源：http://tqf.epnwcf.com


<!-- 参考信息 -->