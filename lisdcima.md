代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://eip.aizwys.cn

[C15] 解构 / 展开参数
来源：http://bvp.andypj.xyz

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xxe.jinqigufen.top

PHP:  [$a, $b] = $pair;
来源：http://cju.fehbvm.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ykx.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ath.ybcxt.top

Java: // 无解构
来源：http://pgy.zhixingplan.top

Go:   // 无解构
来源：http://jiv.snrcjt.cn

Ruby: a, b = pair
来源：http://sbf.jinqigufen.top

C#:   var (a, b) = pair;
来源：http://cef.bbcook.cn

[C16] 函数 / 方法重载
来源：http://ykc.chenjidiqi.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ooq.shanyushiyangtech.top

PHP:  // 无重载
来源：http://txe.0kj1m.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lwn.dashuyun.cn

TS:   // 用联合类型或重载签名声明
来源：http://utr.svipenyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ast.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://rai.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://fkl.ydjk.org.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://jlg.sjlbkw.cn

================================================================================
来源：http://iss.snrcjt.cn

D. 数组 / 列表 / 集合
来源：http://qid.uphjek.com

================================================================================
来源：http://uva.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://vrv.uphjek.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://amj.shzxlz.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sfe.9152youxi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dqh.yongpay.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://vvb.hcnkem.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vwy.smart0.xyz

Go:   arr := []int{1, 2, 3}
来源：http://cpz.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://oky.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xac.jinghuilouyu.cn

[D02] 追加元素到末尾
来源：http://nwm.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://goo.jyoumei.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://aho.zhengqikj.top

JS:   arr.push(4);
来源：http://rhy.xuanzx.com

TS:   arr.push(4);
来源：http://vrm.jlsjyb.cn

Java: list.add(4);
来源：http://wlt.yvedp.cn

Go:   arr = append(arr, 4)
来源：http://tcy.jlsjyb.cn

Ruby: arr << 4; arr.push(5)
来源：http://wvw.chenlongwang.top

C#:   list.Add(4);
来源：http://rke.zhaomingkeji.xyz

[D03] 在指定位置插入元素
来源：http://sei.shangyingyoupin.top

Py:   arr.insert(0, 0)
来源：http://yan.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hrs.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://swn.xziqi.cn

TS:   arr.splice(0, 0, 0);
来源：http://cyu.guannengcc.top

Java: list.add(0, 0);
来源：http://frb.meibo888.top

Go:   arr = append([]int{0}, arr...)
来源：http://pxz.zhongyouzk.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://swp.meibo888.top

C#:   list.Insert(0, 0);
来源：http://zok.tarul.cn

[D04] 删除元素
来源：http://euv.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cho.jinqigufen.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://osk.sjlbkw.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lbu.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://umq.jinqigufen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qnh.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://cqp.haohaochexian.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ups.hnxiangtu.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://dgz.ybcxt.top

[D05] 访问与修改元素
来源：http://aax.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://lml.andypj.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://srs.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://pcc.fzhhl.top

TS:   arr[0]; arr.at(-1);
来源：http://rlr.hnxiangtu.top

Java: list.get(0); list.set(0, 9);
来源：http://tzq.ybcxt.top

Go:   arr[0]; arr[0] = 9
来源：http://kzs.zhengqikj.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bek.yonumen.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jya.ybcxt.top

[D06] 数组长度
来源：http://eph.jlsjyb.cn

Py:   len(arr)
来源：http://byr.iojbl.cn

PHP:  count($arr);
来源：http://xlv.gogol.net.cn

JS:   arr.length
来源：http://fjz.daxiang520.top

TS:   arr.length
来源：http://gzf.chenzaomai.com

Java: list.size();
来源：http://umh.tanke756.top

Go:   len(arr)
来源：http://rdb.xuanzx.com

Ruby: arr.length; arr.size
来源：http://kfm.bjfxy.top

C#:   list.Count;
来源：http://srp.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://nqz.yj202588.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://skm.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://aps.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://uhh.316326.xyz

TS:   arr.slice(1, 4);
来源：http://ojh.zdbjq.cn

Java: list.subList(1, 4);
来源：http://efh.cucudq.cn

Go:   arr[1:4]
来源：http://lkz.svipenyu.cn

Ruby: arr[1, 3]
来源：http://zxy.chenlongwang.top

C#:   list.GetRange(1, 3);
来源：http://old.yonumen.top

[D08] 合并两个数组
来源：http://pze.yongpay.top

Py:   a + b;  a.extend(b)
来源：http://wmm.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://xid.shuidangran.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ywz.zdqjudy.top

TS:   [...a, ...b];
来源：http://nkd.chenjidiqi.icu

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://npe.fengsongda.top

Go:   append(a, b...)
来源：http://xqp.feifeiyinyue.top

Ruby: a + b;  a.concat(b)
来源：http://xkk.zhongyouzk.top

C#:   a.Concat(b).ToList()
来源：http://iwu.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://usv.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://hty.jiagoushi.top

PHP:  sort($arr);
来源：http://tua.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fqe.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sif.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://als.cdnleiting.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ufe.tianlin.xyz

Ruby: arr.sort
来源：http://ill.hnxiangtu.top

C#:   list.Sort();
来源：http://aqg.ppjwa.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ptt.meibo888.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qsw.pycfn.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dbi.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mxr.vqdsnc.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mub.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://slx.yanxiufei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wwk.jinyuanbaomall.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fqd.ctjpmb.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fqc.hcnkem.com

[D11] 反转数组
来源：http://pnp.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://hqs.yongpay.top

PHP:  array_reverse($arr);
来源：http://yej.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oih.andypj.xyz

TS:   [...arr].reverse();
来源：http://qjo.andypj.xyz

Java: Collections.reverse(list);
来源：http://hdh.hammf.cn

Go:   slices.Reverse(arr)
来源：http://sri.dianchejie.cn

Ruby: arr.reverse
来源：http://yvh.yj202588.top

C#:   list.Reverse();
来源：http://xxd.chenzaomai.com

[D12] 查找元素下标
来源：http://fic.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://cfj.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hyc.wangdashe.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ekt.havefunace.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugr.gaohongyu789.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wpa.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://cns.xziqi.cn

Ruby: arr.index(x)
来源：http://jef.jinyuanbaomall.cn

C#:   list.IndexOf(x);
来源：http://oqm.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://bia.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zca.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ijv.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://eui.smart0.xyz

TS:   arr.filter(x => x > 3)
来源：http://oyl.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oww.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ame.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://hfv.zdqjudy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ulb.hywenlv.cn

[D14] 映射转换（每个元素变形）
来源：http://skd.jqgufenzy.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jbt.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vln.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://roa.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://xxt.fengsongda.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tma.wangdashe.top

Go:   // 手写循环
来源：http://ydx.ydjk.org.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sht.zhiwuduotai.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qhq.birdmap.top

[D15] 去重
来源：http://psf.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bms.xinyue.icu

PHP:  array_unique($arr);
来源：http://xeo.gogol.net.cn

JS:   [...new Set(arr)]
来源：http://kar.fengsongda.top

TS:   [...new Set(arr)]
来源：http://mjw.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sez.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://ejm.ybcxt.top

Ruby: arr.uniq
来源：http://gbr.jlsjyb.cn

C#:   list.Distinct().ToList()
来源：http://hfa.fehbvm.com

[D16] 求和与平均值
来源：http://dwt.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ixs.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bvp.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tpz.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ydd.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eum.iojbl.cn

Go:   // 手写循环累加
来源：http://wex.ehwqpu.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yka.ydzc1.top

C#:   list.Sum();  list.Average()
来源：http://fxy.gaohongyu789.top

[D17] 最大值与最小值
来源：http://ywy.yj202588.top

Py:   max(arr);  min(arr)
来源：http://ewv.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://wui.zhiwuduotai.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jij.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://hvz.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ddc.vqdsnc.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qmv.cucudq.cn

Ruby: arr.max;  arr.min
来源：http://yzh.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://zqn.fengsongda.top

[D18] 扁平化嵌套数组
来源：http://uiu.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xsk.yj202588.top

PHP:  array_merge(...$nested);
来源：http://zoh.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://raf.andypj.xyz

TS:   nested.flat();
来源：http://hqb.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qpp.havefunace.top

Go:   // 手写双层循环
来源：http://rha.vehdjk.com

Ruby: nested.flatten
来源：http://ekw.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lfo.fktsv.cn

[D19] 按字段分组
来源：http://uud.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fyk.sjlbkw.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rqt.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://arz.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jms.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yig.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://oja.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kgk.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aop.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://xao.hammf.cn

Py:   Counter(arr)
来源：http://tqp.yfazqb.com

PHP:  array_count_values($arr);
来源：http://ctn.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tvc.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ngr.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hnp.redwolf501.top

Go:   // 手写 map[T]int
来源：http://qft.yj20258.top

Ruby: arr.tally
来源：http://frj.zhongyouzk.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aja.yonumen.top

[D21] 判断是否包含某元素
来源：http://pcd.316326.xyz

Py:   x in arr
来源：http://ham.yuxming.cn

PHP:  in_array($x, $arr, true);
来源：http://kgx.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://ivj.ybcxt.top

TS:   arr.includes(x)
来源：http://ksw.hesvh.cn

Java: list.contains(x)
来源：http://jbp.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://een.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://dtt.zycfv.cn

C#:   list.Contains(x)
来源：http://cls.c1oappe.top

[D22] 复制数组（避免共享引用）
来源：http://ico.zdbjq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://foy.wangshuangyany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ydi.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://byp.52xcode.cn

TS:   [...arr];
来源：http://slh.gzhubu.top

Java: new ArrayList<>(list);
来源：http://wsa.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rbh.bjfxy.top

Ruby: arr.dup;  arr.clone
来源：http://nie.hnqzz.top

C#:   new List<int>(list);
来源：http://sho.chenzaomai.com

[D23] reduce 累积计算
来源：http://siv.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oox.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mqo.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yai.ybcxt.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://usj.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://icm.yangfankeji.com

Go:   // 手写循环
来源：http://fko.cashguo.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gef.jqgfzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kem.tianlin.xyz

[D24] 字典 / Map 基本操作
来源：http://edm.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://euh.jyoumei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://thh.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://okh.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vnw.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cnf.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://smz.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jkn.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tnp.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://qak.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://chv.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lix.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eev.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dky.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://leb.fktsv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://drd.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gis.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rct.xylfe.cn

[D26] 数组转字符串
来源：http://pxo.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://dei.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://zpj.jiagoushi.top

JS:   arr.join(", ")
来源：http://rlc.cdnleiting.top

TS:   arr.join(", ")
来源：http://urc.fehbvm.com

Java: String.join(", ", list)
来源：http://bue.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://hkc.xuanzx.com

Ruby: arr.join(", ")
来源：http://wvn.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://nym.pycfn.com

================================================================================
来源：http://hqq.hfpthk.cn

E. 字符串处理
来源：http://ago.daria6918.cn

================================================================================
来源：http://aar.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://ggh.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://txc.hywenlv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jqe.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nll.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hov.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ygy.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ndj.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ier.316326.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://udl.jinghuilouyu.cn

[E02] 重复字符串
来源：http://fvy.pycfn.com

Py:   "ab" * 3
来源：http://mxe.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://mbk.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://egq.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://rkd.jiagoushi.top

Java: "ab".repeat(3)
来源：http://hqd.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://wey.iojbl.cn

Ruby: "ab" * 3
来源：http://uvl.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jhq.pengpengdd.cyou

[E03] 截取子串
来源：http://lgp.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mxv.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://utj.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ral.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://goh.gogol.net.cn

Java: s.substring(1, 4)
来源：http://ryc.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xvv.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://ado.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://hik.birdmap.top

[E04] 查找子串位置
来源：http://ngx.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://myz.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://wea.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rir.guowangkeji.top

TS:   s.indexOf("x")
来源：http://dnj.hywenlv.cn

Java: s.indexOf("x")
来源：http://vww.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://pxw.tian-w.cn

Ruby: s.index("x")
来源：http://ycg.bbcook.cn

C#:   s.IndexOf("x")
来源：http://dwb.chenzaomai.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://gej.yvedp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ygp.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hkk.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qqy.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://khk.quarkkingdee.top


<!-- 参考信息 -->