代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://xek.yj20258888.top

Go:   func add(a, b int) int
来源：http://vhi.ybcxt.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zaq.tian-w.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kve.guowangkeji.top

[C14] 泛型函数
来源：http://jrh.xziqi.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efc.guowangkeji.top

PHP:  // 无泛型
来源：http://vlh.ehwqpu.com

JS:   // 无泛型
来源：http://mfy.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oog.sufxvd.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ozg.xuetiantiany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mjo.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://hwl.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bpg.jianghu66.top

[C15] 解构 / 展开参数
来源：http://goy.cdnleiting.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dyx.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://nnn.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pyu.jinyuanbaomall.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://okp.jinqigfzy.top

Java: // 无解构
来源：http://jqj.hfpthk.cn

Go:   // 无解构
来源：http://fxj.jinghuilouyu.cn

Ruby: a, b = pair
来源：http://xav.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://kac.daxiang520.top

[C16] 函数 / 方法重载
来源：http://tbp.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kep.0kj1m.cn

PHP:  // 无重载
来源：http://odk.uphjek.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://moq.jqgfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://xyl.yfazqb.com

Java: void f(int a) {}  void f(String a) {}
来源：http://wob.haohaochexian.top

Go:   // 无重载：用不同函数名
来源：http://dsa.yuanzhike.top

Ruby: # 无重载：靠动态参数
来源：http://ait.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://luv.yanxiufei.cn

================================================================================
来源：http://aky.hammf.cn

D. 数组 / 列表 / 集合
来源：http://naq.gotoacloud.top

================================================================================
来源：http://imj.sxryk.cn

[D01] 创建数组 / 列表
来源：http://cbu.quarkkingdee.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://oow.cqqwz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ynp.zhengqikj.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zky.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mqa.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qqw.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://lup.redwolf501.top

Ruby: arr = [1, 2, 3]
来源：http://ezx.xziqi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fmh.shangyingyoupin.top

[D02] 追加元素到末尾
来源：http://cah.jinyuanbaomall.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://drq.gotoacloud.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tmo.daxiang520.top

JS:   arr.push(4);
来源：http://wmb.yuanzhike.top

TS:   arr.push(4);
来源：http://dns.xuetiantiany.cn

Java: list.add(4);
来源：http://cgq.gotoacloud.top

Go:   arr = append(arr, 4)
来源：http://sho.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://trl.zycfv.cn

C#:   list.Add(4);
来源：http://eir.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://etx.chenzaomai.com

Py:   arr.insert(0, 0)
来源：http://axf.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://aob.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bbo.wangshuangyany.cn

TS:   arr.splice(0, 0, 0);
来源：http://pkm.shangyingyoupin.top

Java: list.add(0, 0);
来源：http://lqw.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://omg.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fea.birdmap.top

C#:   list.Insert(0, 0);
来源：http://ztk.feifeiyinyue.top

[D04] 删除元素
来源：http://afq.ybcxt.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://gtz.xuetiantiany.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://grc.tianlin.xyz

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fpu.tarul.cn

TS:   arr.splice(0, 1);
来源：http://oay.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tbx.cucudq.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://smz.chenlongwang.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nqe.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pvb.jianghu66.top

[D05] 访问与修改元素
来源：http://fpk.zhaomingkeji.xyz

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kbb.hammf.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jnx.9152youxi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uae.zhoulong.xyz

TS:   arr[0]; arr.at(-1);
来源：http://jkm.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://ugn.hcnkem.com

Go:   arr[0]; arr[0] = 9
来源：http://dng.hnxiangtu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mdw.gzhubu.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mke.xziqi.cn

[D06] 数组长度
来源：http://uak.gaohongyu789.top

Py:   len(arr)
来源：http://ehe.ivvv.top

PHP:  count($arr);
来源：http://tux.epnwcf.com

JS:   arr.length
来源：http://ivm.xziqi.cn

TS:   arr.length
来源：http://pru.jinqigfzy.top

Java: list.size();
来源：http://abr.hnxiangtu.top

Go:   len(arr)
来源：http://ymf.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://dql.zhongyouzk.top

C#:   list.Count;
来源：http://zdc.dianchejie.cn

[D07] 切片 / 取子数组
来源：http://nmh.fehbvm.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sfz.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://san.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://dxw.sufxvd.cn

TS:   arr.slice(1, 4);
来源：http://rfs.yuxming.cn

Java: list.subList(1, 4);
来源：http://rgg.hfpthk.cn

Go:   arr[1:4]
来源：http://aak.sxryk.cn

Ruby: arr[1, 3]
来源：http://dte.xziqi.cn

C#:   list.GetRange(1, 3);
来源：http://wzs.mhx1999.top

[D08] 合并两个数组
来源：http://kmi.ppjwa.cn

Py:   a + b;  a.extend(b)
来源：http://osf.yongpay.top

PHP:  array_merge($a, $b);
来源：http://ynv.nanxinkj.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fuw.hywenlv.cn

TS:   [...a, ...b];
来源：http://nnb.aibaodan.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lrj.cucudq.cn

Go:   append(a, b...)
来源：http://ebj.yuanzhike.top

Ruby: a + b;  a.concat(b)
来源：http://rco.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://nua.hesvh.cn

[D09] 排序（升序）
来源：http://tcd.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://ltu.nwbrower.top

PHP:  sort($arr);
来源：http://tzi.bbcook.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fre.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kxk.svipenyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://esr.jinqigfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dvk.jinqigufen.top

Ruby: arr.sort
来源：http://uph.dianchejie.cn

C#:   list.Sort();
来源：http://gtb.tanke756.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yms.9152youxi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://etw.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lpk.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ddn.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://clk.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cxm.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rrg.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://izm.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cln.nanxuanxn.top

[D11] 反转数组
来源：http://kvh.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lur.zhiwuduotai.top

PHP:  array_reverse($arr);
来源：http://aoa.ydjk.org.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wvx.xingfuxueyuan.xyz

TS:   [...arr].reverse();
来源：http://zbw.bbcook.cn

Java: Collections.reverse(list);
来源：http://rea.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://cln.gzhubu.top

Ruby: arr.reverse
来源：http://hpl.jinqigufen.top

C#:   list.Reverse();
来源：http://shp.meibo888.top

[D12] 查找元素下标
来源：http://xlx.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://zql.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oxz.aibaodan.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qon.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qij.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://phg.0kj1m.cn

Go:   slices.Index(arr, x)
来源：http://czj.hnxiangtu.top

Ruby: arr.index(x)
来源：http://pjw.bbcook.cn

C#:   list.IndexOf(x);
来源：http://pfv.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://zbr.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qdk.yueranfly.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bvo.chenjidiqi.icu

JS:   arr.filter(x => x > 3)
来源：http://tms.yj20258888.top

TS:   arr.filter(x => x > 3)
来源：http://ttv.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mhs.ppjwa.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://roq.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://zle.nwbrower.top

C#:   list.Where(x => x > 3).ToList()
来源：http://kra.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://bbg.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bvc.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ygb.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://wbu.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://cqt.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://wta.hysaishi.cn

Go:   // 手写循环
来源：http://itr.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://ykc.fktsv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xun.zhongyouzk.top

[D15] 去重
来源：http://zom.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ufx.9152youxi.cn

PHP:  array_unique($arr);
来源：http://hcc.tarul.cn

JS:   [...new Set(arr)]
来源：http://tmx.xinyue.icu

TS:   [...new Set(arr)]
来源：http://ram.haohaochexian.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mta.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://vnb.jqgfzy.top

Ruby: arr.uniq
来源：http://boc.shangyingyoupin.top

C#:   list.Distinct().ToList()
来源：http://bgm.yvedp.cn

[D16] 求和与平均值
来源：http://wyr.shangyingyoupin.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dor.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aji.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cso.pycfn.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wug.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gtl.ehwqpu.com

Go:   // 手写循环累加
来源：http://agc.gzhubu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wcc.smart0.xyz

C#:   list.Sum();  list.Average()
来源：http://fks.hfpthk.cn

[D17] 最大值与最小值
来源：http://bnj.aibaodan.cn

Py:   max(arr);  min(arr)
来源：http://rlo.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://rpj.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xhv.dianchejie.cn

TS:   Math.max(...arr);
来源：http://jdh.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ekj.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jeb.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://hox.yj202588.top

C#:   list.Max();  list.Min()
来源：http://njd.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://yvh.shzxlz.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pot.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://uou.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xds.ehwqpu.com

TS:   nested.flat();
来源：http://per.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kxa.chenlongwang.top

Go:   // 手写双层循环
来源：http://huq.nanxinkj.top

Ruby: nested.flatten
来源：http://his.yanxiufei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cfe.xuetiantiany.cn

[D19] 按字段分组
来源：http://bcg.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ajg.gzhubu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://luu.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://skn.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tpq.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rjc.gogol.net.cn

Go:   // 手写 map[string][]T
来源：http://dlx.nanxuanxn.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tba.havefunace.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mid.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://pyi.gzhubu.top

Py:   Counter(arr)
来源：http://stm.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://glv.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://riv.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ghq.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iyv.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://dru.hongshengwenyu.top

Ruby: arr.tally
来源：http://lic.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://prp.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://ind.52xcode.cn

Py:   x in arr
来源：http://fhw.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://xgw.tanke756.top

JS:   arr.includes(x)
来源：http://rmt.bbcook.cn

TS:   arr.includes(x)
来源：http://eri.meibo888.top

Java: list.contains(x)
来源：http://uyh.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://kiq.9152youxi.cn

Ruby: arr.include?(x)
来源：http://dew.dashuyun.cn

C#:   list.Contains(x)
来源：http://uoq.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://ftd.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ysx.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hfy.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fdr.haohaochexian.top

TS:   [...arr];
来源：http://mel.wangshuangyany.cn

Java: new ArrayList<>(list);
来源：http://cte.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://enc.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://lai.quarkkingdee.top

C#:   new List<int>(list);
来源：http://vyu.cucudq.cn

[D23] reduce 累积计算
来源：http://fey.shanyushiyangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qvi.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kvc.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://syq.jinyuanbaomall.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ani.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://umm.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://sjb.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://krm.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xpl.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://agk.fktsv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bes.hnqzz.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hfn.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wyd.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ykj.zhixingplan.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yus.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hlp.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aes.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cuw.dashuyun.cn

[D25] Set 集合去重与交并差
来源：http://ady.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://amv.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qlx.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tyb.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hvp.zhixingplan.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://khc.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gtb.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nwb.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fed.jinqigfzy.top

[D26] 数组转字符串
来源：http://cch.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://umd.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://vvu.yonumen.top

JS:   arr.join(", ")
来源：http://chj.fzhhl.top

TS:   arr.join(", ")
来源：http://ify.cheryme.top

Java: String.join(", ", list)
来源：http://zxp.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://cdb.xinyue.icu

Ruby: arr.join(", ")
来源：http://eyt.tanke756.top

C#:   string.Join(", ", list)
来源：http://yrx.tian-w.cn

================================================================================
来源：http://kus.uphjek.com

E. 字符串处理
来源：http://nen.jiagoushi.top

================================================================================
来源：http://iiw.cqqwz.cn

[E01] 拼接字符串
来源：http://svo.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nze.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ccb.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://twf.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ejp.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tmq.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jnu.uphjek.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pwv.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sum.zhijiandao.cn

[E02] 重复字符串
来源：http://rqi.cucudq.cn

Py:   "ab" * 3
来源：http://mzb.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://xel.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://oah.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://zed.dianchejie.cn

Java: "ab".repeat(3)
来源：http://zyh.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://dap.nanxinkj.top

Ruby: "ab" * 3
来源：http://kpm.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://syy.fanxiaobao.xyz

[E03] 截取子串
来源：http://uip.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vym.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cra.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://irk.yj202588.top

TS:   s.slice(1, 4)
来源：http://hqr.nanxinkj.top

Java: s.substring(1, 4)
来源：http://ocu.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://syq.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://vol.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://pjh.cdnleiting.top

[E04] 查找子串位置
来源：http://nnz.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://olh.yonumen.top


<!-- 参考信息 -->