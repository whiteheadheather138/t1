代发 wailian999

[C14] 泛型函数
来源：http://ybo.zhongyouzk.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kfi.9152youxi.cn

PHP:  // 无泛型
来源：http://ifb.cdnleiting.top

JS:   // 无泛型
来源：http://dzh.wangdashe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://znd.smart0.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ngh.sysykeji.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tbj.daria6918.cn

Ruby: # 无泛型
来源：http://zfb.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://upm.birdmap.top

[C15] 解构 / 展开参数
来源：http://daa.cheryme.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gmg.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://csn.yangfankeji.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://elg.jlsjyb.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://djd.zhoulong.xyz

Java: // 无解构
来源：http://pzt.fehbvm.com

Go:   // 无解构
来源：http://uyg.zycfv.cn

Ruby: a, b = pair
来源：http://enc.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://rtz.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://aja.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://idj.hesvh.cn

PHP:  // 无重载
来源：http://bic.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://sbo.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://crj.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fbt.dianchejie.cn

Go:   // 无重载：用不同函数名
来源：http://cyw.hnqzz.top

Ruby: # 无重载：靠动态参数
来源：http://wfn.sysykeji.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://fss.yfazqb.com

================================================================================
来源：http://zxj.zhongyouzk.top

D. 数组 / 列表 / 集合
来源：http://svd.hammf.cn

================================================================================
来源：http://eya.pycfn.com

[D01] 创建数组 / 列表
来源：http://jkh.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ryy.bbcook.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dqk.xuanzx.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wcj.yonumen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://umk.gotoacloud.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mfi.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://xar.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://slg.yj20258888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hsl.chenzaomai.com

[D02] 追加元素到末尾
来源：http://cjl.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pqb.birdmap.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oub.c1oappe.top

JS:   arr.push(4);
来源：http://jwq.yvedp.cn

TS:   arr.push(4);
来源：http://yfx.jlsjyb.cn

Java: list.add(4);
来源：http://zyg.jqgufenzy.top

Go:   arr = append(arr, 4)
来源：http://trb.dashuyun.cn

Ruby: arr << 4; arr.push(5)
来源：http://kaf.xziqi.cn

C#:   list.Add(4);
来源：http://djh.pycfn.com

[D03] 在指定位置插入元素
来源：http://zjb.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://szt.bjfxy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ynw.sufxvd.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mia.shanyushiyangtech.top

TS:   arr.splice(0, 0, 0);
来源：http://apt.jinghuilouyu.cn

Java: list.add(0, 0);
来源：http://xhu.jqgufenzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://fma.yangfankeji.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://etm.xylfe.cn

C#:   list.Insert(0, 0);
来源：http://xma.smart0.xyz

[D04] 删除元素
来源：http://lfi.yongpay.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://byn.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ipk.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lxj.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://aut.haohaochexian.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ctp.yuanzhike.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tpv.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cig.jianghu66.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://joy.yonumen.top

[D05] 访问与修改元素
来源：http://ozr.jqgufenzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mgx.hywenlv.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://axm.hongshengwenyu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uil.hcnkem.com

TS:   arr[0]; arr.at(-1);
来源：http://xsy.chenjidiqi.icu

Java: list.get(0); list.set(0, 9);
来源：http://iye.xylfe.cn

Go:   arr[0]; arr[0] = 9
来源：http://aew.jianghu66.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fdu.ybcxt.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://feh.sufxvd.cn

[D06] 数组长度
来源：http://gkv.jinqigfzy.top

Py:   len(arr)
来源：http://hir.yj20258888.top

PHP:  count($arr);
来源：http://qvl.ywan-chungtsiang.top

JS:   arr.length
来源：http://fie.pengpengdd.cyou

TS:   arr.length
来源：http://xjg.zycfv.cn

Java: list.size();
来源：http://hoy.fehbvm.com

Go:   len(arr)
来源：http://kdg.hnqzz.top

Ruby: arr.length; arr.size
来源：http://zzo.c1oappe.top

C#:   list.Count;
来源：http://dvk.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://ptl.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vwl.jinqigfzy.top

PHP:  array_slice($arr, 1, 3);
来源：http://gud.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://urm.dashuyun.cn

TS:   arr.slice(1, 4);
来源：http://std.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://qqi.gzhubu.top

Go:   arr[1:4]
来源：http://eba.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://yjq.guowangkeji.top

C#:   list.GetRange(1, 3);
来源：http://rfm.hysaishi.cn

[D08] 合并两个数组
来源：http://ovl.c1oappe.top

Py:   a + b;  a.extend(b)
来源：http://xso.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://twj.quarkkingdee.top

JS:   [...a, ...b];  a.concat(b);
来源：http://vsa.hongshengwenyu.top

TS:   [...a, ...b];
来源：http://gvi.c1oappe.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cfa.0kj1m.cn

Go:   append(a, b...)
来源：http://ynt.yongpay.top

Ruby: a + b;  a.concat(b)
来源：http://ntf.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://ofl.xylfe.cn

[D09] 排序（升序）
来源：http://dod.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://zim.jlsjyb.cn

PHP:  sort($arr);
来源：http://vxk.jiagoushi.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bgw.zhengqikj.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wup.shzxlz.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vwk.wangshuangyany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gmo.zhoulong.xyz

Ruby: arr.sort
来源：http://ppy.aizwys.cn

C#:   list.Sort();
来源：http://feq.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qya.xuetiantiany.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tot.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://adt.uphjek.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dvw.jlsjyb.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://exz.shanyushiyangtech.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lcd.hesvh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hca.fanxiaobao.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rzz.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fyi.hnqzz.top

[D11] 反转数组
来源：http://pdj.fehbvm.com

Py:   arr[::-1];  arr.reverse()
来源：http://ibq.jqgufenzy.top

PHP:  array_reverse($arr);
来源：http://rgz.hfpthk.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wfy.zdbjq.cn

TS:   [...arr].reverse();
来源：http://rgz.havefunace.top

Java: Collections.reverse(list);
来源：http://wsn.ppjwa.cn

Go:   slices.Reverse(arr)
来源：http://pcm.birdmap.top

Ruby: arr.reverse
来源：http://uob.cashguo.top

C#:   list.Reverse();
来源：http://zdh.zdqjudy.top

[D12] 查找元素下标
来源：http://rlr.jqgfzy.top

Py:   arr.index(x);  x in arr
来源：http://bqs.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eiz.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://civ.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kqt.fengsongda.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pcd.sysykeji.top

Go:   slices.Index(arr, x)
来源：http://mbw.aizwys.cn

Ruby: arr.index(x)
来源：http://zjh.hcnkem.com

C#:   list.IndexOf(x);
来源：http://lgu.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://ydr.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nzy.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://oab.hnxiangtu.top

JS:   arr.filter(x => x > 3)
来源：http://lki.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://ios.cdnleiting.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jdf.cdnleiting.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://acj.xuetiantiany.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gun.meibo888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fkw.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://dov.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sas.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nby.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://hum.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://fgo.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://opr.jinqigufen.top

Go:   // 手写循环
来源：http://xmg.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://tbw.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mcu.fanxiaobao.xyz

[D15] 去重
来源：http://isq.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xby.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://ukb.jianghu66.top

JS:   [...new Set(arr)]
来源：http://kis.aizwys.cn

TS:   [...new Set(arr)]
来源：http://tmz.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gpo.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://wla.dashuyun.cn

Ruby: arr.uniq
来源：http://eps.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://reb.hfpthk.cn

[D16] 求和与平均值
来源：http://hkn.tian-w.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mmx.ydjk.org.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fmm.jinqigufen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hjb.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cka.yj20258888.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ijy.cashguo.top

Go:   // 手写循环累加
来源：http://wds.zhongyouzk.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gow.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://jgp.shanyushiyangkeji.top

[D17] 最大值与最小值
来源：http://czw.sweek.top

Py:   max(arr);  min(arr)
来源：http://zzm.cucudq.cn

PHP:  max($arr);  min($arr);
来源：http://tqd.daxiang520.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://flh.chenlongwang.top

TS:   Math.max(...arr);
来源：http://jay.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://kfk.havefunace.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aob.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://hok.nwbrower.top

C#:   list.Max();  list.Min()
来源：http://fqy.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://yir.sxryk.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gyb.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://bmd.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wvo.jianghu66.top

TS:   nested.flat();
来源：http://hbm.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kbn.xylfe.cn

Go:   // 手写双层循环
来源：http://aaw.hammf.cn

Ruby: nested.flatten
来源：http://kdx.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nfs.daria6918.cn

[D19] 按字段分组
来源：http://stm.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pnj.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oqk.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ubo.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://slm.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://szu.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://bxa.zhixingplan.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nle.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mly.hcnkem.com

[D20] 统计每个元素出现次数
来源：http://wal.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://ngz.jianghu66.top

PHP:  array_count_values($arr);
来源：http://hlq.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ykh.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yhn.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rft.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://ktr.chenzaomai.com

Ruby: arr.tally
来源：http://dic.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kkr.redwolf501.top

[D21] 判断是否包含某元素
来源：http://tdh.52xcode.cn

Py:   x in arr
来源：http://pvp.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://xmd.hongshengwenyu.top

JS:   arr.includes(x)
来源：http://oos.nanxinkj.top

TS:   arr.includes(x)
来源：http://awj.yuxming.cn

Java: list.contains(x)
来源：http://ddx.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://czl.ydjk.org.cn

Ruby: arr.include?(x)
来源：http://yku.zhixingplan.top

C#:   list.Contains(x)
来源：http://ylg.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://pgm.316326.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ozs.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://njy.tianlin.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pbj.chenjidiqi.icu

TS:   [...arr];
来源：http://ayi.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://lzn.sufxvd.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nru.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://scv.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://fcc.jinyuanbaomall.cn

[D23] reduce 累积计算
来源：http://sth.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aiq.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vzu.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ltf.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovw.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pyq.shzxlz.cn

Go:   // 手写循环
来源：http://tnd.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bvw.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nod.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://pmd.cheryme.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wgk.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rhj.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bym.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ale.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sqq.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rhh.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yfr.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lwt.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://zhj.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cmu.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jsc.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nws.shzxlz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ywk.fehbvm.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://glq.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oiu.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ess.pycfn.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qpq.yonumen.top

[D26] 数组转字符串
来源：http://qyk.fanxiaobao.xyz

Py:   ", ".join(map(str, arr))
来源：http://rup.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://jgx.sufxvd.cn

JS:   arr.join(", ")
来源：http://jrb.dashuyun.cn

TS:   arr.join(", ")
来源：http://bms.jinqigfzy.top

Java: String.join(", ", list)
来源：http://yea.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://dio.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://akv.sysykeji.top

C#:   string.Join(", ", list)
来源：http://rmw.xuetiantiany.cn

================================================================================
来源：http://siz.shanyushiyangtech.top

E. 字符串处理
来源：http://aoh.sufxvd.cn

================================================================================
来源：http://vne.jinghuilouyu.cn

[E01] 拼接字符串
来源：http://lyc.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ssg.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tli.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rnm.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dgm.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mny.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pza.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kde.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uwr.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://xxx.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://xlx.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://pbi.52xcode.cn

JS:   "ab".repeat(3)
来源：http://tmd.yonumen.top

TS:   "ab".repeat(3)
来源：http://rvv.jiagoushi.top

Java: "ab".repeat(3)
来源：http://eyu.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://clh.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://ksn.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hsy.cashguo.top

[E03] 截取子串
来源：http://bpa.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://trl.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://prd.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kht.yj20258.top

TS:   s.slice(1, 4)
来源：http://txs.hammf.cn

Java: s.substring(1, 4)
来源：http://iin.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nec.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://qmr.tarul.cn

C#:   s.Substring(1, 3)
来源：http://ssg.dianchejie.cn

[E04] 查找子串位置
来源：http://wqn.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://egt.chenjidiqi.icu

PHP:  strpos($s, "x");
来源：http://dlk.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ypz.nanxinkj.top

TS:   s.indexOf("x")
来源：http://icj.ydjk.org.cn

Java: s.indexOf("x")
来源：http://zpk.wangshuangyany.cn


<!-- 参考信息 -->