代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://npn.daria6918.cn

[C15] 解构 / 展开参数
来源：http://trz.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://msx.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://azy.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ipw.jyoumei.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bgj.pengpengdd.cyou

Java: // 无解构
来源：http://cpf.snrcjt.cn

Go:   // 无解构
来源：http://dsk.hesvh.cn

Ruby: a, b = pair
来源：http://zaa.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://sjx.yuanzhike.top

[C16] 函数 / 方法重载
来源：http://anx.jqgufenzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kvq.pengpengdd.cyou

PHP:  // 无重载
来源：http://pua.meibo888.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://yuj.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://xlh.0kj1m.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://csp.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://jcw.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://srb.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uwx.chenlongwang.top

================================================================================
来源：http://hnr.shangyingyoupin.top

D. 数组 / 列表 / 集合
来源：http://meh.aibaodan.cn

================================================================================
来源：http://grf.cdnleiting.top

[D01] 创建数组 / 列表
来源：http://syu.shangyingyoupin.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://gqi.52xcode.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cds.ywan-chungtsiang.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://klc.52xcode.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://civ.snrcjt.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://acp.xinyue.icu

Go:   arr := []int{1, 2, 3}
来源：http://tju.ybcxt.top

Ruby: arr = [1, 2, 3]
来源：http://tkv.fzhhl.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vtl.0kj1m.cn

[D02] 追加元素到末尾
来源：http://rej.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://clj.iojbl.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oem.bbcook.cn

JS:   arr.push(4);
来源：http://ott.zhixingplan.top

TS:   arr.push(4);
来源：http://jxk.shuidangran.top

Java: list.add(4);
来源：http://ffn.xinyue.icu

Go:   arr = append(arr, 4)
来源：http://gql.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://xtp.pengpengdd.cyou

C#:   list.Add(4);
来源：http://rsr.zhongyouzk.top

[D03] 在指定位置插入元素
来源：http://riz.ivvv.top

Py:   arr.insert(0, 0)
来源：http://wgb.feifeiyinyue.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mkk.xuetiantiany.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ahl.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://tgq.zdbjq.cn

Java: list.add(0, 0);
来源：http://dri.hfpthk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zrj.9152youxi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xen.yj20258.top

C#:   list.Insert(0, 0);
来源：http://xeu.c1oappe.top

[D04] 删除元素
来源：http://frf.jianghu66.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://spy.gzhubu.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zil.ivvv.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xlk.ppjwa.cn

TS:   arr.splice(0, 1);
来源：http://lvv.0kj1m.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tgu.hfpthk.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://igh.tianlin.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pfg.cdnleiting.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dcl.fktsv.cn

[D05] 访问与修改元素
来源：http://wcm.ehwqpu.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gev.sweek.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://keo.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sen.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://wyq.sufxvd.cn

Java: list.get(0); list.set(0, 9);
来源：http://hhy.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://ouh.jqgfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qjx.chenzaomai.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://axj.cqqwz.cn

[D06] 数组长度
来源：http://oif.jinqigfzy.top

Py:   len(arr)
来源：http://odx.yj20258.top

PHP:  count($arr);
来源：http://crt.ywan-chungtsiang.top

JS:   arr.length
来源：http://elt.shzxlz.cn

TS:   arr.length
来源：http://gbm.yuanzhike.top

Java: list.size();
来源：http://oqt.yj20258888.top

Go:   len(arr)
来源：http://zok.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://vhv.jinqigfzy.top

C#:   list.Count;
来源：http://mfn.uphjek.com

[D07] 切片 / 取子数组
来源：http://oud.havefunace.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gzw.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://ztg.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://mdd.yj20258888.top

TS:   arr.slice(1, 4);
来源：http://lme.wangdashe.top

Java: list.subList(1, 4);
来源：http://pum.xylfe.cn

Go:   arr[1:4]
来源：http://woi.shanyushiyangkeji.top

Ruby: arr[1, 3]
来源：http://gfi.xuetiantiany.cn

C#:   list.GetRange(1, 3);
来源：http://vsf.pengpengdd.cyou

[D08] 合并两个数组
来源：http://ava.jinghuilouyu.cn

Py:   a + b;  a.extend(b)
来源：http://dnx.ydzc1.top

PHP:  array_merge($a, $b);
来源：http://fer.nwbrower.top

JS:   [...a, ...b];  a.concat(b);
来源：http://xmd.yvedp.cn

TS:   [...a, ...b];
来源：http://kbp.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nlb.haohaochexian.top

Go:   append(a, b...)
来源：http://lqg.zdbjq.cn

Ruby: a + b;  a.concat(b)
来源：http://zmv.yj202588.top

C#:   a.Concat(b).ToList()
来源：http://cwo.jiagoushi.top

[D09] 排序（升序）
来源：http://uip.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://ldi.chenzaomai.com

PHP:  sort($arr);
来源：http://yzw.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rur.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lvp.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://brb.xuetiantiany.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sja.daxiang520.top

Ruby: arr.sort
来源：http://ovi.shanyushiyangtech.top

C#:   list.Sort();
来源：http://uos.hnqzz.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://xib.sufxvd.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ccd.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zee.nanxinkj.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://trz.hfpthk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://vjp.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cvd.zhengqikj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://izs.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rnk.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hah.hesvh.cn

[D11] 反转数组
来源：http://kej.tianlin.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://een.meibo888.top

PHP:  array_reverse($arr);
来源：http://dek.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://smd.sufxvd.cn

TS:   [...arr].reverse();
来源：http://mdh.gogol.net.cn

Java: Collections.reverse(list);
来源：http://vtd.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://scg.quarkkingdee.top

Ruby: arr.reverse
来源：http://waa.ehwqpu.com

C#:   list.Reverse();
来源：http://xyi.andypj.xyz

[D12] 查找元素下标
来源：http://huy.chenjidiqi.icu

Py:   arr.index(x);  x in arr
来源：http://cwd.jinyuanbaomall.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hpb.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://erj.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vub.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pae.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://ymn.c1oappe.top

Ruby: arr.index(x)
来源：http://hvp.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://mlz.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://prl.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rls.ybcxt.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uqu.yj20258888.top

JS:   arr.filter(x => x > 3)
来源：http://ipj.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://rmt.guowangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rrj.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://pkr.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://bjh.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gne.snrcjt.cn

[D14] 映射转换（每个元素变形）
来源：http://zvj.hongshengwenyu.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nth.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://svd.ehwqpu.com

JS:   arr.map(x => x * 2)
来源：http://bei.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://ksv.svipenyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mur.nanxinkj.top

Go:   // 手写循环
来源：http://jgh.snrcjt.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rtb.hnqzz.top

C#:   list.Select(x => x * 2).ToList()
来源：http://alw.jianghu66.top

[D15] 去重
来源：http://plv.xinyue.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://udg.ctjpmb.com

PHP:  array_unique($arr);
来源：http://pij.havefunace.top

JS:   [...new Set(arr)]
来源：http://dzc.nanxuanxn.top

TS:   [...new Set(arr)]
来源：http://qii.iojbl.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ffp.ppjwa.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gmy.dashuyun.cn

Ruby: arr.uniq
来源：http://qoh.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://wir.jianghu66.top

[D16] 求和与平均值
来源：http://nzb.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rmd.52xcode.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cdw.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uor.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fco.vqdsnc.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mcw.52xcode.cn

Go:   // 手写循环累加
来源：http://atr.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gas.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://thi.yuxming.cn

[D17] 最大值与最小值
来源：http://cid.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://jnw.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://zwp.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vjw.hysaishi.cn

TS:   Math.max(...arr);
来源：http://dwo.chenlongwang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jdt.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kvn.tianlin.xyz

Ruby: arr.max;  arr.min
来源：http://ejv.yj20258.top

C#:   list.Max();  list.Min()
来源：http://yxv.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://msp.ybcxt.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mrn.hammf.cn

PHP:  array_merge(...$nested);
来源：http://poz.0kj1m.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qna.fehbvm.com

TS:   nested.flat();
来源：http://giu.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eew.yj20258888.top

Go:   // 手写双层循环
来源：http://ycy.andypj.xyz

Ruby: nested.flatten
来源：http://cqu.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ake.zdbjq.cn

[D19] 按字段分组
来源：http://jbg.hfpthk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xhn.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tlo.meibo888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://egb.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xfz.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jxr.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://uyo.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://egi.ppjwa.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bkm.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://nad.shangyingyoupin.top

Py:   Counter(arr)
来源：http://nwz.cheryme.top

PHP:  array_count_values($arr);
来源：http://ahz.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://epd.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zli.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://swx.hfpthk.cn

Go:   // 手写 map[T]int
来源：http://phf.gotoacloud.top

Ruby: arr.tally
来源：http://krf.jinqigfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dfn.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://oni.hysaishi.cn

Py:   x in arr
来源：http://tef.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://por.redwolf501.top

JS:   arr.includes(x)
来源：http://gfp.sweek.top

TS:   arr.includes(x)
来源：http://vsr.cqqwz.cn

Java: list.contains(x)
来源：http://zxw.sufxvd.cn

Go:   slices.Contains(arr, x)
来源：http://lik.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://qcc.zycfv.cn

C#:   list.Contains(x)
来源：http://yde.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://khi.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bge.kuanghao11.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ssj.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pye.pycfn.com

TS:   [...arr];
来源：http://nze.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://osq.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://qnd.fengsongda.top

Ruby: arr.dup;  arr.clone
来源：http://hqn.fengsongda.top

C#:   new List<int>(list);
来源：http://hbr.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://gkz.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://edw.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kji.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kii.shuidangran.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zch.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://rwk.snrcjt.cn

Go:   // 手写循环
来源：http://zjf.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xhc.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://alu.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://xiq.zhoulong.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ptl.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mkz.hongshengwenyu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kmh.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jjk.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ope.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ist.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bqv.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oli.birdmap.top

[D25] Set 集合去重与交并差
来源：http://air.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lze.yj20258.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nht.daxiang520.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zvu.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yuf.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fbi.hammf.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sap.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vwu.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nhh.gaohongyu789.top

[D26] 数组转字符串
来源：http://xph.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://wbn.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://qlr.zycfv.cn

JS:   arr.join(", ")
来源：http://lhw.dashuyun.cn

TS:   arr.join(", ")
来源：http://ycn.jlsjyb.cn

Java: String.join(", ", list)
来源：http://zfl.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://qcg.jianghu66.top

Ruby: arr.join(", ")
来源：http://eie.xziqi.cn

C#:   string.Join(", ", list)
来源：http://qqy.guowangkeji.top

================================================================================
来源：http://cla.hysaishi.cn

E. 字符串处理
来源：http://nez.shangyingyoupin.top

================================================================================
来源：http://bdm.iojbl.cn

[E01] 拼接字符串
来源：http://hsp.zhongyouzk.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wjr.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://arv.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tyw.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lns.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://klo.hysaishi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vlu.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pfv.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pxi.tian-w.cn

[E02] 重复字符串
来源：http://aly.sjlbkw.cn

Py:   "ab" * 3
来源：http://lnh.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://dlg.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://ydp.cashguo.top

TS:   "ab".repeat(3)
来源：http://ilb.hcnkem.com

Java: "ab".repeat(3)
来源：http://rhj.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://zwt.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://mty.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vhd.guannengcc.top

[E03] 截取子串
来源：http://zsc.cqqwz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rru.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hhb.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uea.vehdjk.com

TS:   s.slice(1, 4)
来源：http://egj.yfazqb.com

Java: s.substring(1, 4)
来源：http://kfi.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vef.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mmr.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://iby.zhengqikj.top

[E04] 查找子串位置
来源：http://ggc.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://ula.yangfankeji.com

PHP:  strpos($s, "x");
来源：http://iao.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kor.aibaodan.cn

TS:   s.indexOf("x")
来源：http://xfr.zdbjq.cn

Java: s.indexOf("x")
来源：http://bad.sjlbkw.cn

Go:   strings.Index(s, "x")
来源：http://tyz.yj202588.top

Ruby: s.index("x")
来源：http://wyg.smart0.xyz

C#:   s.IndexOf("x")
来源：http://tao.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qnv.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xeo.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nuz.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dfe.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://veq.sysykeji.top


<!-- 参考信息 -->