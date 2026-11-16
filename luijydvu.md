代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://msf.jianghu66.top

Go:   func add(a, b int) int
来源：http://gdn.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://txp.jlsjyb.cn

C#:   int Add(int a, int b) => a + b;
来源：http://aso.52xcode.cn

[C14] 泛型函数
来源：http://vin.guowangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://prt.yangfankeji.com

PHP:  // 无泛型
来源：http://jwz.jinghuilouyu.cn

JS:   // 无泛型
来源：http://gcj.guannengcc.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cdc.ehwqpu.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mqn.chenjidiqi.icu

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sux.cucudq.cn

Ruby: # 无泛型
来源：http://hxm.xingfuxueyuan.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rlv.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://mtq.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cdu.316326.xyz

PHP:  [$a, $b] = $pair;
来源：http://ajw.ivvv.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://slj.daria6918.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zal.ctjpmb.com

Java: // 无解构
来源：http://ott.sweek.top

Go:   // 无解构
来源：http://jhp.yuxming.cn

Ruby: a, b = pair
来源：http://plt.ivvv.top

C#:   var (a, b) = pair;
来源：http://jvk.nwbrower.top

[C16] 函数 / 方法重载
来源：http://ork.yanxiufei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://inm.fzhhl.top

PHP:  // 无重载
来源：http://xos.jinyuanbaomall.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rbr.cucudq.cn

TS:   // 用联合类型或重载签名声明
来源：http://vjv.yuxming.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kmw.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://cgm.hfpthk.cn

Ruby: # 无重载：靠动态参数
来源：http://rof.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://scc.dianchejie.cn

================================================================================
来源：http://rlc.cucudq.cn

D. 数组 / 列表 / 集合
来源：http://mhh.xziqi.cn

================================================================================
来源：http://yra.shuidangran.top

[D01] 创建数组 / 列表
来源：http://qnb.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jta.haohaochexian.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fsy.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bjo.aizwys.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qis.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lyq.cdnleiting.top

Go:   arr := []int{1, 2, 3}
来源：http://jme.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://amn.gzhubu.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rtq.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://mnq.ydjk.org.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://gsp.jinyuanbaomall.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://byk.yongpay.top

JS:   arr.push(4);
来源：http://xpk.jinyuanbaomall.cn

TS:   arr.push(4);
来源：http://nry.sweek.top

Java: list.add(4);
来源：http://rqr.meibo888.top

Go:   arr = append(arr, 4)
来源：http://crm.svipenyu.cn

Ruby: arr << 4; arr.push(5)
来源：http://pht.aizwys.cn

C#:   list.Add(4);
来源：http://lch.havefunace.top

[D03] 在指定位置插入元素
来源：http://rrd.jqgfzy.top

Py:   arr.insert(0, 0)
来源：http://hni.yuanzhike.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ykc.sweek.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qoz.c1oappe.top

TS:   arr.splice(0, 0, 0);
来源：http://yaa.sysykeji.top

Java: list.add(0, 0);
来源：http://lzx.tianlin.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://bir.fzhhl.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oqe.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://ewm.hcnkem.com

[D04] 删除元素
来源：http://xwm.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bmq.mhx1999.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ofi.zdbjq.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://tfk.dashuyun.cn

TS:   arr.splice(0, 1);
来源：http://dlc.nwbrower.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yun.ydjk.org.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uha.dianchejie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qif.jinyuanbaomall.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://kxk.jqgufenzy.top

[D05] 访问与修改元素
来源：http://ztp.sweek.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://suk.yonumen.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wck.hcnkem.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aik.ctjpmb.com

TS:   arr[0]; arr.at(-1);
来源：http://bat.shzxlz.cn

Java: list.get(0); list.set(0, 9);
来源：http://ubh.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://cmi.cashguo.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dha.tian-w.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fvp.fzhhl.top

[D06] 数组长度
来源：http://afn.daxiang520.top

Py:   len(arr)
来源：http://noe.epnwcf.com

PHP:  count($arr);
来源：http://ptu.hysaishi.cn

JS:   arr.length
来源：http://ftu.yuxming.cn

TS:   arr.length
来源：http://xdu.fengsongda.top

Java: list.size();
来源：http://qrp.yuxming.cn

Go:   len(arr)
来源：http://ifs.sjlbkw.cn

Ruby: arr.length; arr.size
来源：http://mxk.daria6918.cn

C#:   list.Count;
来源：http://awr.yonumen.top

[D07] 切片 / 取子数组
来源：http://bny.xinyue.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vus.birdmap.top

PHP:  array_slice($arr, 1, 3);
来源：http://ukm.hesvh.cn

JS:   arr.slice(1, 4);
来源：http://vxr.jinghuilouyu.cn

TS:   arr.slice(1, 4);
来源：http://epj.hesvh.cn

Java: list.subList(1, 4);
来源：http://vkk.yj20258.top

Go:   arr[1:4]
来源：http://xqv.hnqzz.top

Ruby: arr[1, 3]
来源：http://cqe.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://pjf.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://nwd.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://wyd.gotoacloud.top

PHP:  array_merge($a, $b);
来源：http://agh.jinqigfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://pac.shzxlz.cn

TS:   [...a, ...b];
来源：http://hsr.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://smh.yuxming.cn

Go:   append(a, b...)
来源：http://vfq.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://rpy.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://jpr.fanxiaobao.xyz

[D09] 排序（升序）
来源：http://sgg.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://ier.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://ysk.daria6918.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vyv.feifeiyinyue.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://htz.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://ufr.tanke756.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jid.chenlongwang.top

Ruby: arr.sort
来源：http://rjy.havefunace.top

C#:   list.Sort();
来源：http://odh.shangyingyoupin.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://qwz.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://egb.bbcook.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bul.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylb.yangfankeji.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mgm.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cdx.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kkl.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vzi.cheryme.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gtf.yj20258888.top

[D11] 反转数组
来源：http://vuz.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://yda.ydzc1.top

PHP:  array_reverse($arr);
来源：http://ljq.tian-w.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rgk.hesvh.cn

TS:   [...arr].reverse();
来源：http://tjs.chenjidiqi.icu

Java: Collections.reverse(list);
来源：http://qmh.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://bpm.epnwcf.com

Ruby: arr.reverse
来源：http://naa.shanyushiyangtech.top

C#:   list.Reverse();
来源：http://dab.redwolf501.top

[D12] 查找元素下标
来源：http://tay.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://bhh.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qkm.mhx1999.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgd.jyoumei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vra.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iaz.tianlin.xyz

Go:   slices.Index(arr, x)
来源：http://zzo.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://ouy.nanxuanxn.top

C#:   list.IndexOf(x);
来源：http://job.hywenlv.cn

[D13] 过滤（保留满足条件的）
来源：http://crp.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kcu.fehbvm.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rsg.vehdjk.com

JS:   arr.filter(x => x > 3)
来源：http://mak.hfpthk.cn

TS:   arr.filter(x => x > 3)
来源：http://bfi.gotoacloud.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ndw.nwbrower.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gdi.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hqa.hnqzz.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bdb.yj202588.top

[D14] 映射转换（每个元素变形）
来源：http://pjl.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hab.hammf.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xgp.cqqwz.cn

JS:   arr.map(x => x * 2)
来源：http://wjf.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://enz.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vgc.jqgufenzy.top

Go:   // 手写循环
来源：http://exf.sjlbkw.cn

Ruby: arr.map { |x| x * 2 }
来源：http://idn.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://yvs.mhx1999.top

[D15] 去重
来源：http://ecs.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://met.jiagoushi.top

PHP:  array_unique($arr);
来源：http://lbe.tarul.cn

JS:   [...new Set(arr)]
来源：http://fhp.hnqzz.top

TS:   [...new Set(arr)]
来源：http://cvx.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wbp.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kub.ehwqpu.com

Ruby: arr.uniq
来源：http://egl.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://lsp.ybcxt.top

[D16] 求和与平均值
来源：http://eci.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rfo.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://npv.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pjq.uphjek.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfb.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jmv.yueranfly.top

Go:   // 手写循环累加
来源：http://bdq.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cpm.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://bsk.xuanzx.com

[D17] 最大值与最小值
来源：http://tfc.nanxinkj.top

Py:   max(arr);  min(arr)
来源：http://wmk.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://zhr.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yeg.guannengcc.top

TS:   Math.max(...arr);
来源：http://huu.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://igl.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nmx.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://hgq.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://dfi.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://vhc.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mct.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://pca.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jia.yuanzhike.top

TS:   nested.flat();
来源：http://xba.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kbz.zhixingplan.top

Go:   // 手写双层循环
来源：http://ixj.epnwcf.com

Ruby: nested.flatten
来源：http://fin.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://wqx.nwbrower.top

[D19] 按字段分组
来源：http://lnw.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tsx.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tvg.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://swg.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yig.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gll.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://fbb.wangshuangyany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dtm.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://evn.yueranfly.top

[D20] 统计每个元素出现次数
来源：http://iek.hcnkem.com

Py:   Counter(arr)
来源：http://ntu.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://zof.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbc.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qja.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jzi.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://vud.zycfv.cn

Ruby: arr.tally
来源：http://fhe.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dsp.xylfe.cn

[D21] 判断是否包含某元素
来源：http://ssp.xingfuxueyuan.xyz

Py:   x in arr
来源：http://jxg.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://zpd.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://zdk.chenlongwang.top

TS:   arr.includes(x)
来源：http://fkd.snrcjt.cn

Java: list.contains(x)
来源：http://tnp.zhixingplan.top

Go:   slices.Contains(arr, x)
来源：http://jze.andypj.xyz

Ruby: arr.include?(x)
来源：http://adw.chenzaomai.com

C#:   list.Contains(x)
来源：http://twm.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://hzr.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wrk.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vza.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cxz.feifeiyinyue.top

TS:   [...arr];
来源：http://vwo.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://xzr.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://iwk.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://ozm.yanxiufei.cn

C#:   new List<int>(list);
来源：http://cje.cheryme.top

[D23] reduce 累积计算
来源：http://ift.yueranfly.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://guv.tianlin.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zdn.cdnleiting.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sep.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zea.yonumen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cfm.guowangkeji.top

Go:   // 手写循环
来源：http://dra.jinqigfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fyy.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zws.tarul.cn

[D24] 字典 / Map 基本操作
来源：http://fgi.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xdd.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wfg.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zht.tian-w.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cax.jinyuanbaomall.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://coq.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nao.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nts.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xqd.yongpay.top

[D25] Set 集合去重与交并差
来源：http://ihk.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gho.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tnm.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ysn.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tvb.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oex.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://eij.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lpw.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yat.shangyingyoupin.top

[D26] 数组转字符串
来源：http://scy.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://suc.zhongyouzk.top

PHP:  implode(", ", $arr);
来源：http://ypf.yj202588.top

JS:   arr.join(", ")
来源：http://oux.yj20258.top

TS:   arr.join(", ")
来源：http://vav.snrcjt.cn

Java: String.join(", ", list)
来源：http://vun.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://gzj.fktsv.cn

Ruby: arr.join(", ")
来源：http://vjk.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://hde.cdnleiting.top

================================================================================
来源：http://onl.hnxiangtu.top

E. 字符串处理
来源：http://hbi.zhaomingkeji.xyz

================================================================================
来源：http://mww.nanxinkj.top

[E01] 拼接字符串
来源：http://cso.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iba.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uuj.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mno.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pky.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ilv.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wif.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hvt.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xjo.xylfe.cn

[E02] 重复字符串
来源：http://ukp.kuanghao11.cn

Py:   "ab" * 3
来源：http://laq.ydjk.org.cn

PHP:  str_repeat("ab", 3);
来源：http://byg.52xcode.cn

JS:   "ab".repeat(3)
来源：http://eoc.bbcook.cn

TS:   "ab".repeat(3)
来源：http://rhk.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://hyr.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://dcv.tanke756.top

Ruby: "ab" * 3
来源：http://ucg.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cvj.xuetiantiany.cn

[E03] 截取子串
来源：http://olx.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jct.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dtd.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lyj.bbcook.cn

TS:   s.slice(1, 4)
来源：http://tcx.nwbrower.top

Java: s.substring(1, 4)
来源：http://zpl.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ecs.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://oyh.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://vph.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://bqp.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://osx.52xcode.cn


<!-- 参考信息 -->