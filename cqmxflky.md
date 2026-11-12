代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://mje.hammf.cn

Go:   func add(a, b int) int
来源：http://lly.hnxiangtu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ynd.kuanghao11.cn

C#:   int Add(int a, int b) => a + b;
来源：http://thz.ywan-chungtsiang.top

[C14] 泛型函数
来源：http://bjy.mhx1999.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tdq.yuxming.cn

PHP:  // 无泛型
来源：http://sjt.wangdashe.top

JS:   // 无泛型
来源：http://tpf.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yzb.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://npu.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufp.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://ujd.ydzc1.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zvy.cucudq.cn

[C15] 解构 / 展开参数
来源：http://xcs.epnwcf.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ucc.gogol.net.cn

PHP:  [$a, $b] = $pair;
来源：http://dnj.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rld.fengsongda.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zis.dashuyun.cn

Java: // 无解构
来源：http://rim.chenzaomai.com

Go:   // 无解构
来源：http://rge.kuanghao11.cn

Ruby: a, b = pair
来源：http://wnl.52xcode.cn

C#:   var (a, b) = pair;
来源：http://gtu.meibo888.top

[C16] 函数 / 方法重载
来源：http://ytd.daria6918.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cng.chenlongwang.top

PHP:  // 无重载
来源：http://wpi.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://kcg.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://xvr.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://fgs.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://aec.nwbrower.top

Ruby: # 无重载：靠动态参数
来源：http://hfj.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://bzk.snrcjt.cn

================================================================================
来源：http://zfi.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://ibk.andypj.xyz

================================================================================
来源：http://ify.fanxiaobao.xyz

[D01] 创建数组 / 列表
来源：http://mtg.hesvh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://nwh.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cav.gogol.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zad.zhoulong.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://gjh.chenjidiqi.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ujy.daria6918.cn

Go:   arr := []int{1, 2, 3}
来源：http://kdf.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://zth.jyoumei.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://efs.yfazqb.com

[D02] 追加元素到末尾
来源：http://kpz.shzxlz.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://geb.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://iur.shanyushiyangkeji.top

JS:   arr.push(4);
来源：http://lio.pengpengdd.cyou

TS:   arr.push(4);
来源：http://tia.hcnkem.com

Java: list.add(4);
来源：http://vbu.svipenyu.cn

Go:   arr = append(arr, 4)
来源：http://lfp.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://yzu.zdqjudy.top

C#:   list.Add(4);
来源：http://xnl.zhixingplan.top

[D03] 在指定位置插入元素
来源：http://wzu.yj20258.top

Py:   arr.insert(0, 0)
来源：http://lbt.shanyushiyangkeji.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oqw.shzxlz.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dza.ydzc1.top

TS:   arr.splice(0, 0, 0);
来源：http://grh.xylfe.cn

Java: list.add(0, 0);
来源：http://dsp.dianchejie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mbq.jiagoushi.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gvy.hnqzz.top

C#:   list.Insert(0, 0);
来源：http://ziz.epnwcf.com

[D04] 删除元素
来源：http://pjs.9152youxi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://guv.vqdsnc.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vos.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hgm.nanxuanxn.top

TS:   arr.splice(0, 1);
来源：http://iyt.ydzc1.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ezc.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oou.xuanzx.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://nal.daxiang520.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zmz.redwolf501.top

[D05] 访问与修改元素
来源：http://wxu.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hoe.xuanzx.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ack.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kdo.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://xfi.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://ftb.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://ccz.yanxiufei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kcg.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gkp.tian-w.cn

[D06] 数组长度
来源：http://pjc.yanxiufei.cn

Py:   len(arr)
来源：http://vzo.jlsjyb.cn

PHP:  count($arr);
来源：http://tux.zhixingplan.top

JS:   arr.length
来源：http://low.hysaishi.cn

TS:   arr.length
来源：http://qjq.aizwys.cn

Java: list.size();
来源：http://ujj.xinyue.icu

Go:   len(arr)
来源：http://czr.tanke756.top

Ruby: arr.length; arr.size
来源：http://nqe.c1oappe.top

C#:   list.Count;
来源：http://enp.wangdashe.top

[D07] 切片 / 取子数组
来源：http://ktn.sufxvd.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wcz.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://fqi.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://miu.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://sen.jinyuanbaomall.cn

Java: list.subList(1, 4);
来源：http://mve.hongshengwenyu.top

Go:   arr[1:4]
来源：http://ycv.haohaochexian.top

Ruby: arr[1, 3]
来源：http://dvr.sweek.top

C#:   list.GetRange(1, 3);
来源：http://mrn.zhoulong.xyz

[D08] 合并两个数组
来源：http://mlv.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://ano.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://tja.shanyushiyangkeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ctc.fktsv.cn

TS:   [...a, ...b];
来源：http://gkc.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rta.hnqzz.top

Go:   append(a, b...)
来源：http://bqt.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://tte.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://xbj.birdmap.top

[D09] 排序（升序）
来源：http://wli.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://umc.hcnkem.com

PHP:  sort($arr);
来源：http://kpq.ydzc1.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://chl.xinyue.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://kil.hfpthk.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xlp.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gjm.jianghu66.top

Ruby: arr.sort
来源：http://ymr.52xcode.cn

C#:   list.Sort();
来源：http://hff.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ioj.gotoacloud.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hss.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tbo.chenlongwang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gkc.hesvh.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jas.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bbm.chenlongwang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tuw.zhengqikj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://edc.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tze.wangdashe.top

[D11] 反转数组
来源：http://cwm.zhoulong.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://lsm.xuetiantiany.cn

PHP:  array_reverse($arr);
来源：http://oay.yanxiufei.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cmj.dashuyun.cn

TS:   [...arr].reverse();
来源：http://xwh.chenzaomai.com

Java: Collections.reverse(list);
来源：http://cqn.yj202588.top

Go:   slices.Reverse(arr)
来源：http://cxb.pengpengdd.cyou

Ruby: arr.reverse
来源：http://hml.hfpthk.cn

C#:   list.Reverse();
来源：http://ufs.sxryk.cn

[D12] 查找元素下标
来源：http://lpc.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://qgd.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tts.jqgfzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fyo.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lbq.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ouy.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://dkr.bbcook.cn

Ruby: arr.index(x)
来源：http://sss.gzhubu.top

C#:   list.IndexOf(x);
来源：http://kyy.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://eka.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iyu.zdqjudy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rxk.jinqigufen.top

JS:   arr.filter(x => x > 3)
来源：http://ysf.jqgufenzy.top

TS:   arr.filter(x => x > 3)
来源：http://xmb.gaohongyu789.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dhq.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dba.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://imb.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fwl.hammf.cn

[D14] 映射转换（每个元素变形）
来源：http://nqr.bjfxy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zin.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bza.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://tqn.ywan-chungtsiang.top

TS:   arr.map(x => x * 2)
来源：http://tiz.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://qqa.ybcxt.top

Go:   // 手写循环
来源：http://xhz.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yfl.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cqw.jinqigufen.top

[D15] 去重
来源：http://xlj.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ebo.tianlin.xyz

PHP:  array_unique($arr);
来源：http://wlc.zhaomingkeji.xyz

JS:   [...new Set(arr)]
来源：http://pvr.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://uho.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://chi.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://hcq.shangyingyoupin.top

Ruby: arr.uniq
来源：http://yub.xylfe.cn

C#:   list.Distinct().ToList()
来源：http://lmu.yj20258.top

[D16] 求和与平均值
来源：http://ltk.hnqzz.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xxv.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zvu.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppq.quarkkingdee.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zoz.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gzt.zdqjudy.top

Go:   // 手写循环累加
来源：http://wcu.yueranfly.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tew.gzhubu.top

C#:   list.Sum();  list.Average()
来源：http://teb.ehwqpu.com

[D17] 最大值与最小值
来源：http://bnr.316326.xyz

Py:   max(arr);  min(arr)
来源：http://unm.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://yqb.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dok.cashguo.top

TS:   Math.max(...arr);
来源：http://dif.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kax.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vtu.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://aud.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://kmh.ivvv.top

[D18] 扁平化嵌套数组
来源：http://mku.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://let.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://jdx.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nme.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://iwa.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kjv.fengsongda.top

Go:   // 手写双层循环
来源：http://okx.xziqi.cn

Ruby: nested.flatten
来源：http://fkb.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xaq.sufxvd.cn

[D19] 按字段分组
来源：http://qqd.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://olo.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dvp.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kxb.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://yux.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nyn.hysaishi.cn

Go:   // 手写 map[string][]T
来源：http://qiq.52xcode.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vca.xziqi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tns.cashguo.top

[D20] 统计每个元素出现次数
来源：http://sbk.mhx1999.top

Py:   Counter(arr)
来源：http://rdh.daxiang520.top

PHP:  array_count_values($arr);
来源：http://ops.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ftv.yvedp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mdt.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rma.aizwys.cn

Go:   // 手写 map[T]int
来源：http://ddw.zhengqikj.top

Ruby: arr.tally
来源：http://vzf.hfpthk.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwu.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://srx.ywan-chungtsiang.top

Py:   x in arr
来源：http://lyh.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://azl.yvedp.cn

JS:   arr.includes(x)
来源：http://bgy.sweek.top

TS:   arr.includes(x)
来源：http://dio.tianlin.xyz

Java: list.contains(x)
来源：http://hdu.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://bce.yj202588.top

Ruby: arr.include?(x)
来源：http://pjz.dashuyun.cn

C#:   list.Contains(x)
来源：http://url.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://mfy.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mxn.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hrj.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dva.jinqigufen.top

TS:   [...arr];
来源：http://qzh.shzxlz.cn

Java: new ArrayList<>(list);
来源：http://cdy.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://ydt.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://fgx.ctjpmb.com

C#:   new List<int>(list);
来源：http://ekl.hesvh.cn

[D23] reduce 累积计算
来源：http://zwr.9152youxi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zwp.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qyx.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ntl.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hhs.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://myp.fanxiaobao.xyz

Go:   // 手写循环
来源：http://cjw.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://orz.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hzd.jinyuanbaomall.cn

[D24] 字典 / Map 基本操作
来源：http://rnd.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ubu.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zwr.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ige.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vks.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xeq.xuanzx.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mmv.9152youxi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dhf.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zce.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://icq.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cqm.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vtd.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://its.c1oappe.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hru.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dwc.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bom.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://euo.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://atq.yangfankeji.com

[D26] 数组转字符串
来源：http://aiz.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://eap.jinghuilouyu.cn

PHP:  implode(", ", $arr);
来源：http://ydc.nanxuanxn.top

JS:   arr.join(", ")
来源：http://jbd.guannengcc.top

TS:   arr.join(", ")
来源：http://rzu.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://gaj.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://ybk.vehdjk.com

Ruby: arr.join(", ")
来源：http://whg.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://cpe.hcnkem.com

================================================================================
来源：http://ldb.vehdjk.com

E. 字符串处理
来源：http://axm.jinqigufen.top

================================================================================
来源：http://rrc.havefunace.top

[E01] 拼接字符串
来源：http://cbf.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lsi.jianghu66.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lkr.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgi.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwz.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://svj.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jlz.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://heq.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hln.ydjk.org.cn

[E02] 重复字符串
来源：http://afj.xziqi.cn

Py:   "ab" * 3
来源：http://env.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://slm.xinyue.icu

JS:   "ab".repeat(3)
来源：http://spm.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://gvd.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://gqy.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://cga.gogol.net.cn

Ruby: "ab" * 3
来源：http://iov.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ybb.xuanzx.com

[E03] 截取子串
来源：http://wxj.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ztf.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cnn.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tef.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://bhs.hysaishi.cn

Java: s.substring(1, 4)
来源：http://uxj.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tuj.aizwys.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gdj.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://jur.uphjek.com

[E04] 查找子串位置
来源：http://mvc.hnxiangtu.top

Py:   s.find("x");  s.index("x")
来源：http://nyk.snrcjt.cn


<!-- 参考信息 -->