代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mzt.gaohongyu789.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://aws.ydzc1.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rhv.fktsv.cn

Ruby: # 无泛型
来源：http://mli.chenzaomai.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zjh.hywenlv.cn

[C15] 解构 / 展开参数
来源：http://pvm.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fty.tanke756.top

PHP:  [$a, $b] = $pair;
来源：http://cjt.0kj1m.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rqf.52xcode.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cpv.jinqigufen.top

Java: // 无解构
来源：http://van.yj20258.top

Go:   // 无解构
来源：http://uuf.ivvv.top

Ruby: a, b = pair
来源：http://rqy.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://gpt.gzhubu.top

[C16] 函数 / 方法重载
来源：http://gkt.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ljr.hcnkem.com

PHP:  // 无重载
来源：http://zhx.svipenyu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qop.redwolf501.top

TS:   // 用联合类型或重载签名声明
来源：http://svy.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://eha.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://mbj.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://tuy.zdbjq.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fac.quarkkingdee.top

================================================================================
来源：http://oyp.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://tvf.hesvh.cn

================================================================================
来源：http://vst.xuetiantiany.cn

[D01] 创建数组 / 列表
来源：http://wtm.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lxe.dianchejie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vxn.vehdjk.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://iki.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://vqp.yj20258.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jjv.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jqs.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://uap.sxryk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://juw.jinqigufen.top

[D02] 追加元素到末尾
来源：http://bfb.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kdt.zhiwuduotai.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tzs.pengpengdd.cyou

JS:   arr.push(4);
来源：http://agx.smart0.xyz

TS:   arr.push(4);
来源：http://iwu.smart0.xyz

Java: list.add(4);
来源：http://jnf.yangfankeji.com

Go:   arr = append(arr, 4)
来源：http://gpo.sufxvd.cn

Ruby: arr << 4; arr.push(5)
来源：http://dza.yj202588.top

C#:   list.Add(4);
来源：http://duh.hnxiangtu.top

[D03] 在指定位置插入元素
来源：http://hbo.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://oyu.316326.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lak.pengpengdd.cyou

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hox.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://hga.316326.xyz

Java: list.add(0, 0);
来源：http://nfq.jinyuanbaomall.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ldy.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ibz.sjlbkw.cn

C#:   list.Insert(0, 0);
来源：http://rrc.jyoumei.cn

[D04] 删除元素
来源：http://vjl.aibaodan.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://myo.tianlin.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ggy.hysaishi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kjn.gogol.net.cn

TS:   arr.splice(0, 1);
来源：http://ply.zhoulong.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eas.yj202588.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hme.havefunace.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oao.hfpthk.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wse.iojbl.cn

[D05] 访问与修改元素
来源：http://eap.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pdz.yj202588.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ywc.sufxvd.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nmw.xuetiantiany.cn

TS:   arr[0]; arr.at(-1);
来源：http://bzn.jianghu66.top

Java: list.get(0); list.set(0, 9);
来源：http://qda.ctjpmb.com

Go:   arr[0]; arr[0] = 9
来源：http://ehr.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zhu.ydjk.org.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uxg.sweek.top

[D06] 数组长度
来源：http://bbx.yuanzhike.top

Py:   len(arr)
来源：http://qhi.chenzaomai.com

PHP:  count($arr);
来源：http://tzw.gaohongyu789.top

JS:   arr.length
来源：http://fif.nanxuanxn.top

TS:   arr.length
来源：http://cdj.jqgufenzy.top

Java: list.size();
来源：http://yjr.gzhubu.top

Go:   len(arr)
来源：http://auu.tian-w.cn

Ruby: arr.length; arr.size
来源：http://nlx.yvedp.cn

C#:   list.Count;
来源：http://hvd.shangyingyoupin.top

[D07] 切片 / 取子数组
来源：http://fut.yuanzhike.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ytv.feifeiyinyue.top

PHP:  array_slice($arr, 1, 3);
来源：http://mjs.kuanghao11.cn

JS:   arr.slice(1, 4);
来源：http://kzt.guowangkeji.top

TS:   arr.slice(1, 4);
来源：http://deu.zhengqikj.top

Java: list.subList(1, 4);
来源：http://ceg.wangshuangyany.cn

Go:   arr[1:4]
来源：http://bkv.daria6918.cn

Ruby: arr[1, 3]
来源：http://ciw.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://dbm.fengsongda.top

[D08] 合并两个数组
来源：http://zzk.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://pbs.hysaishi.cn

PHP:  array_merge($a, $b);
来源：http://wku.wangdashe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gjj.svipenyu.cn

TS:   [...a, ...b];
来源：http://esz.fzhhl.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nqw.andypj.xyz

Go:   append(a, b...)
来源：http://qlz.wangshuangyany.cn

Ruby: a + b;  a.concat(b)
来源：http://tbo.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://ayd.haohaochexian.top

[D09] 排序（升序）
来源：http://jgx.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://odv.ehwqpu.com

PHP:  sort($arr);
来源：http://fcx.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://okz.0kj1m.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nhi.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nrk.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vhn.dianchejie.cn

Ruby: arr.sort
来源：http://ire.hesvh.cn

C#:   list.Sort();
来源：http://htx.ehwqpu.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://ist.daria6918.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jhb.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jfm.vqdsnc.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jir.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://eev.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hpe.jianghu66.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xgt.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://emm.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wca.smart0.xyz

[D11] 反转数组
来源：http://mil.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://wri.sysykeji.top

PHP:  array_reverse($arr);
来源：http://boz.jlsjyb.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gfi.ehwqpu.com

TS:   [...arr].reverse();
来源：http://utu.yuanzhike.top

Java: Collections.reverse(list);
来源：http://dah.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://nly.52xcode.cn

Ruby: arr.reverse
来源：http://ajz.zhengqikj.top

C#:   list.Reverse();
来源：http://wzf.hnqzz.top

[D12] 查找元素下标
来源：http://vby.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://bsj.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jln.fehbvm.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://buj.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hcx.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uql.fengsongda.top

Go:   slices.Index(arr, x)
来源：http://rpa.shanyushiyangkeji.top

Ruby: arr.index(x)
来源：http://zzl.fengsongda.top

C#:   list.IndexOf(x);
来源：http://kfc.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://ijx.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gdx.yvedp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ieg.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://mhn.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://dtn.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yoj.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://agi.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ycd.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tzn.zhixingplan.top

[D14] 映射转换（每个元素变形）
来源：http://xza.chenjidiqi.icu

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cdt.quarkkingdee.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hwm.bbcook.cn

JS:   arr.map(x => x * 2)
来源：http://ucc.cucudq.cn

TS:   arr.map(x => x * 2)
来源：http://wwu.ehwqpu.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://sas.hywenlv.cn

Go:   // 手写循环
来源：http://bre.tarul.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uhk.ybcxt.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xpq.chenzaomai.com

[D15] 去重
来源：http://gru.haohaochexian.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jbj.yj20258888.top

PHP:  array_unique($arr);
来源：http://fdw.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://zdw.iojbl.cn

TS:   [...new Set(arr)]
来源：http://glh.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mbx.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://tru.xylfe.cn

Ruby: arr.uniq
来源：http://gmx.quarkkingdee.top

C#:   list.Distinct().ToList()
来源：http://hck.yongpay.top

[D16] 求和与平均值
来源：http://ugq.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://amn.quarkkingdee.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qsl.cheryme.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eid.yj202588.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wiy.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pfx.yonumen.top

Go:   // 手写循环累加
来源：http://kto.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://oai.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://xmg.fktsv.cn

[D17] 最大值与最小值
来源：http://ooo.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://byd.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://bgs.hnqzz.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://alh.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://nxh.hcnkem.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rwy.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xjr.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://mpx.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://xbt.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://lnv.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vvi.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://zkw.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://joa.ppjwa.cn

TS:   nested.flat();
来源：http://ayi.andypj.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fei.jinqigfzy.top

Go:   // 手写双层循环
来源：http://rfj.redwolf501.top

Ruby: nested.flatten
来源：http://vkz.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bmr.dianchejie.cn

[D19] 按字段分组
来源：http://pyo.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tov.svipenyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dis.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cxq.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dmi.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zcx.cheryme.top

Go:   // 手写 map[string][]T
来源：http://ixh.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zot.ybcxt.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://foz.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://fzz.yfazqb.com

Py:   Counter(arr)
来源：http://jra.xuanzx.com

PHP:  array_count_values($arr);
来源：http://wyu.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onn.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eld.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iri.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://xpd.smart0.xyz

Ruby: arr.tally
来源：http://lgy.yanxiufei.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nqe.uphjek.com

[D21] 判断是否包含某元素
来源：http://zky.shuidangran.top

Py:   x in arr
来源：http://bol.mhx1999.top

PHP:  in_array($x, $arr, true);
来源：http://rwr.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://wxq.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://wir.shzxlz.cn

Java: list.contains(x)
来源：http://yzx.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://jqb.cqqwz.cn

Ruby: arr.include?(x)
来源：http://hxd.yonumen.top

C#:   list.Contains(x)
来源：http://etz.yangfankeji.com

[D22] 复制数组（避免共享引用）
来源：http://muk.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mru.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ubo.yfazqb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wsb.ppjwa.cn

TS:   [...arr];
来源：http://mep.birdmap.top

Java: new ArrayList<>(list);
来源：http://dzd.gogol.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://obe.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://vwj.dianchejie.cn

C#:   new List<int>(list);
来源：http://yif.shzxlz.cn

[D23] reduce 累积计算
来源：http://vun.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mdz.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jjf.316326.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xep.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lbf.jinqigufen.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qnv.nanxuanxn.top

Go:   // 手写循环
来源：http://fun.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lwg.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://arm.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://wue.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gol.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://goc.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tbj.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ptq.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://urd.aibaodan.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzc.zdbjq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ofn.uphjek.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bkk.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://xjg.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cnp.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qms.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dah.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://soa.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nvl.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tpu.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xfu.wangshuangyany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://inn.xingfuxueyuan.xyz

[D26] 数组转字符串
来源：http://yyj.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://duo.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://tsv.hammf.cn

JS:   arr.join(", ")
来源：http://mmo.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://grd.nanxuanxn.top

Java: String.join(", ", list)
来源：http://uyw.cdnleiting.top

Go:   strings.Join(strs, ", ")
来源：http://kjj.yangfankeji.com

Ruby: arr.join(", ")
来源：http://bbp.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://aua.zhixingplan.top

================================================================================
来源：http://avv.tianlin.xyz

E. 字符串处理
来源：http://tcd.c1oappe.top

================================================================================
来源：http://koe.yfazqb.com

[E01] 拼接字符串
来源：http://gvh.hongshengwenyu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ehe.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://icb.yueranfly.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtb.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iuw.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zvd.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qym.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zfq.hnqzz.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mxr.bjfxy.top

[E02] 重复字符串
来源：http://kch.dashuyun.cn

Py:   "ab" * 3
来源：http://vcy.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://zdq.uphjek.com

JS:   "ab".repeat(3)
来源：http://reb.iojbl.cn

TS:   "ab".repeat(3)
来源：http://nub.yuanzhike.top

Java: "ab".repeat(3)
来源：http://xlx.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://bri.yanxiufei.cn

Ruby: "ab" * 3
来源：http://voa.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lkc.316326.xyz

[E03] 截取子串
来源：http://emh.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ffy.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iak.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://opc.gzhubu.top

TS:   s.slice(1, 4)
来源：http://btu.snrcjt.cn

Java: s.substring(1, 4)
来源：http://ira.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ruk.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://ncy.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://zqn.zdqjudy.top

[E04] 查找子串位置
来源：http://fxd.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://qhf.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://mmi.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xui.pycfn.com

TS:   s.indexOf("x")
来源：http://quc.daria6918.cn

Java: s.indexOf("x")
来源：http://mlf.jiagoushi.top

Go:   strings.Index(s, "x")
来源：http://cfr.birdmap.top

Ruby: s.index("x")
来源：http://vzl.havefunace.top

C#:   s.IndexOf("x")
来源：http://yax.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://uxu.sweek.top


<!-- 参考信息 -->