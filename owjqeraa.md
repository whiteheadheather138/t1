代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nqr.shangyingyoupin.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kjq.yonumen.top

Java: // 无解构
来源：http://ozt.vqdsnc.cn

Go:   // 无解构
来源：http://lsu.xuetiantiany.cn

Ruby: a, b = pair
来源：http://uxb.dianchejie.cn

C#:   var (a, b) = pair;
来源：http://zks.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://wlk.jinyuanbaomall.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vrx.fzhhl.top

PHP:  // 无重载
来源：http://dmh.fzhhl.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nor.yonumen.top

TS:   // 用联合类型或重载签名声明
来源：http://ywi.jqgufenzy.top

Java: void f(int a) {}  void f(String a) {}
来源：http://byj.ppjwa.cn

Go:   // 无重载：用不同函数名
来源：http://qbt.cdnleiting.top

Ruby: # 无重载：靠动态参数
来源：http://qla.ivvv.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://rbf.hywenlv.cn

================================================================================
来源：http://rvn.ppjwa.cn

D. 数组 / 列表 / 集合
来源：http://vdi.shangyingyoupin.top

================================================================================
来源：http://wup.yanxiufei.cn

[D01] 创建数组 / 列表
来源：http://lwf.tanke756.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fbd.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://btp.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lye.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://eib.ppjwa.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zbt.zhengqikj.top

Go:   arr := []int{1, 2, 3}
来源：http://dae.zdqjudy.top

Ruby: arr = [1, 2, 3]
来源：http://gks.nwbrower.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vxt.sufxvd.cn

[D02] 追加元素到末尾
来源：http://clf.jianghu66.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jsa.nanxuanxn.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://pjo.yuxming.cn

JS:   arr.push(4);
来源：http://tjv.yueranfly.top

TS:   arr.push(4);
来源：http://ipk.hnqzz.top

Java: list.add(4);
来源：http://ovu.zhaomingkeji.xyz

Go:   arr = append(arr, 4)
来源：http://mkr.jianghu66.top

Ruby: arr << 4; arr.push(5)
来源：http://zpk.tian-w.cn

C#:   list.Add(4);
来源：http://hff.shangyingyoupin.top

[D03] 在指定位置插入元素
来源：http://lkh.sysykeji.top

Py:   arr.insert(0, 0)
来源：http://qqp.dashuyun.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://taw.uphjek.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wek.aibaodan.cn

TS:   arr.splice(0, 0, 0);
来源：http://baf.jyoumei.cn

Java: list.add(0, 0);
来源：http://pvw.feifeiyinyue.top

Go:   arr = append([]int{0}, arr...)
来源：http://imm.cdnleiting.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bxj.redwolf501.top

C#:   list.Insert(0, 0);
来源：http://xqe.shanyushiyangkeji.top

[D04] 删除元素
来源：http://tbp.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tzc.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fcd.cheryme.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qas.ybcxt.top

TS:   arr.splice(0, 1);
来源：http://plg.redwolf501.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sfh.gogol.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mah.jlsjyb.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zhr.shanyushiyangtech.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zth.gotoacloud.top

[D05] 访问与修改元素
来源：http://eyf.sjlbkw.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kgg.fanxiaobao.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://olq.dianchejie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://lrd.nanxuanxn.top

TS:   arr[0]; arr.at(-1);
来源：http://gis.yj20258888.top

Java: list.get(0); list.set(0, 9);
来源：http://cbq.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://adu.zycfv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mho.yongpay.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cii.tanke756.top

[D06] 数组长度
来源：http://swg.sufxvd.cn

Py:   len(arr)
来源：http://ezp.shanyushiyangkeji.top

PHP:  count($arr);
来源：http://buo.cucudq.cn

JS:   arr.length
来源：http://tqv.hcnkem.com

TS:   arr.length
来源：http://wlh.nwbrower.top

Java: list.size();
来源：http://twz.jinghuilouyu.cn

Go:   len(arr)
来源：http://ceh.cashguo.top

Ruby: arr.length; arr.size
来源：http://nmu.bbcook.cn

C#:   list.Count;
来源：http://eut.xingfuxueyuan.xyz

[D07] 切片 / 取子数组
来源：http://nmy.gotoacloud.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://unq.ywan-chungtsiang.top

PHP:  array_slice($arr, 1, 3);
来源：http://mhp.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://sss.kuanghao11.cn

TS:   arr.slice(1, 4);
来源：http://iww.vqdsnc.cn

Java: list.subList(1, 4);
来源：http://dlo.shzxlz.cn

Go:   arr[1:4]
来源：http://axe.aibaodan.cn

Ruby: arr[1, 3]
来源：http://zhe.vqdsnc.cn

C#:   list.GetRange(1, 3);
来源：http://qbv.ppjwa.cn

[D08] 合并两个数组
来源：http://kly.gzhubu.top

Py:   a + b;  a.extend(b)
来源：http://jma.tarul.cn

PHP:  array_merge($a, $b);
来源：http://fgg.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://oti.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://oun.shzxlz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ghj.yfazqb.com

Go:   append(a, b...)
来源：http://axs.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://nvk.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://bxa.wangshuangyany.cn

[D09] 排序（升序）
来源：http://mde.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://mob.cucudq.cn

PHP:  sort($arr);
来源：http://szx.zhoulong.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wob.daria6918.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ned.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lnk.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ouo.ehwqpu.com

Ruby: arr.sort
来源：http://mbl.hcnkem.com

C#:   list.Sort();
来源：http://qfp.xinyue.icu

[D10] 自定义排序（按字段 / 多条件）
来源：http://wia.gogol.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pni.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vcj.jinghuilouyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfu.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hqi.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://egr.ehwqpu.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mcc.c1oappe.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zrz.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://efj.yvedp.cn

[D11] 反转数组
来源：http://akv.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://gjw.nwbrower.top

PHP:  array_reverse($arr);
来源：http://sqn.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://inz.ehwqpu.com

TS:   [...arr].reverse();
来源：http://pkm.daxiang520.top

Java: Collections.reverse(list);
来源：http://pgj.shanyushiyangtech.top

Go:   slices.Reverse(arr)
来源：http://rkk.xziqi.cn

Ruby: arr.reverse
来源：http://weg.xylfe.cn

C#:   list.Reverse();
来源：http://nrx.yj20258.top

[D12] 查找元素下标
来源：http://oqd.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://ewb.quarkkingdee.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://juf.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cge.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://plh.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://svx.zhongyouzk.top

Go:   slices.Index(arr, x)
来源：http://rbz.gaohongyu789.top

Ruby: arr.index(x)
来源：http://iza.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://rid.xingfuxueyuan.xyz

[D13] 过滤（保留满足条件的）
来源：http://jlk.cheryme.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fhe.yonumen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zut.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://jbo.jianghu66.top

TS:   arr.filter(x => x > 3)
来源：http://kdu.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ejz.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eir.cheryme.top

Ruby: arr.select { |x| x > 3 }
来源：http://dys.shangyingyoupin.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tvd.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://bla.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ngg.jianghu66.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pho.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://jbp.hammf.cn

TS:   arr.map(x => x * 2)
来源：http://jdc.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://msp.xziqi.cn

Go:   // 手写循环
来源：http://jhc.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://oie.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ucn.aizwys.cn

[D15] 去重
来源：http://jpq.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://slb.zdqjudy.top

PHP:  array_unique($arr);
来源：http://dzc.redwolf501.top

JS:   [...new Set(arr)]
来源：http://gru.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://tmi.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fsg.xylfe.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hob.vehdjk.com

Ruby: arr.uniq
来源：http://oes.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://qvq.xylfe.cn

[D16] 求和与平均值
来源：http://ohe.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sxb.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://usr.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ais.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cfu.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wyg.cdnleiting.top

Go:   // 手写循环累加
来源：http://hwv.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ypm.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://bwe.aibaodan.cn

[D17] 最大值与最小值
来源：http://wom.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://btu.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://rda.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vsw.sufxvd.cn

TS:   Math.max(...arr);
来源：http://jhs.ywan-chungtsiang.top

Java: Collections.max(list);  Collections.min(list);
来源：http://suc.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ese.jianghu66.top

Ruby: arr.max;  arr.min
来源：http://vjg.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://pwa.c1oappe.top

[D18] 扁平化嵌套数组
来源：http://puq.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://use.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://wex.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xcf.yj20258.top

TS:   nested.flat();
来源：http://woj.haohaochexian.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ebl.yuanzhike.top

Go:   // 手写双层循环
来源：http://rwy.shangyingyoupin.top

Ruby: nested.flatten
来源：http://ufu.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://hrq.pengpengdd.cyou

[D19] 按字段分组
来源：http://kvx.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://svz.chenlongwang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vuo.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://svm.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wcl.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yvh.redwolf501.top

Go:   // 手写 map[string][]T
来源：http://mbw.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gco.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qyw.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://lqo.nwbrower.top

Py:   Counter(arr)
来源：http://dze.zycfv.cn

PHP:  array_count_values($arr);
来源：http://cui.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gpq.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://czg.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hkg.mhx1999.top

Go:   // 手写 map[T]int
来源：http://ins.redwolf501.top

Ruby: arr.tally
来源：http://dmc.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ypk.yonumen.top

[D21] 判断是否包含某元素
来源：http://xtu.zhixingplan.top

Py:   x in arr
来源：http://plb.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://jqt.cucudq.cn

JS:   arr.includes(x)
来源：http://uuj.yj202588.top

TS:   arr.includes(x)
来源：http://luj.wangshuangyany.cn

Java: list.contains(x)
来源：http://ijq.pengpengdd.cyou

Go:   slices.Contains(arr, x)
来源：http://cma.zycfv.cn

Ruby: arr.include?(x)
来源：http://ctk.nanxinkj.top

C#:   list.Contains(x)
来源：http://dtz.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://npl.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cdl.jlsjyb.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yqx.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zme.wangshuangyany.cn

TS:   [...arr];
来源：http://kxf.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://xve.zhengqikj.top

Go:   copied := append([]int(nil), arr...)
来源：http://rps.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://whz.aizwys.cn

C#:   new List<int>(list);
来源：http://hii.hywenlv.cn

[D23] reduce 累积计算
来源：http://yyf.zhoulong.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vvg.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wmk.zhiwuduotai.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iwm.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lmz.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lnv.yuxming.cn

Go:   // 手写循环
来源：http://jfl.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aqg.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ytp.pengpengdd.cyou

[D24] 字典 / Map 基本操作
来源：http://kin.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fvj.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ywb.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://coh.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sor.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nab.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://joa.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://daa.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bos.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://gzm.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uwi.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pdy.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bkd.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wyf.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cia.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tit.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oue.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hrn.zhengqikj.top

[D26] 数组转字符串
来源：http://bqm.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://rdv.yonumen.top

PHP:  implode(", ", $arr);
来源：http://krb.smart0.xyz

JS:   arr.join(", ")
来源：http://rop.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://oqk.c1oappe.top

Java: String.join(", ", list)
来源：http://oud.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://ufl.ehwqpu.com

Ruby: arr.join(", ")
来源：http://qgj.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://zkt.hnqzz.top

================================================================================
来源：http://qyy.haohaochexian.top

E. 字符串处理
来源：http://jic.tarul.cn

================================================================================
来源：http://yug.gaohongyu789.top

[E01] 拼接字符串
来源：http://kyb.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tdt.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iuu.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iuy.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pmr.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yaq.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yzt.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tob.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lrs.hnxiangtu.top

[E02] 重复字符串
来源：http://vwo.hammf.cn

Py:   "ab" * 3
来源：http://yxu.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://mgp.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://qcv.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://lvo.tianlin.xyz

Java: "ab".repeat(3)
来源：http://oup.feifeiyinyue.top

Go:   strings.Repeat("ab", 3)
来源：http://lxw.shzxlz.cn

Ruby: "ab" * 3
来源：http://pmc.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vch.shanyushiyangkeji.top

[E03] 截取子串
来源：http://vnc.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://whp.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ttq.hnqzz.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cio.wangdashe.top

TS:   s.slice(1, 4)
来源：http://vgo.c1oappe.top

Java: s.substring(1, 4)
来源：http://zmx.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mcs.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://kbw.redwolf501.top

C#:   s.Substring(1, 3)
来源：http://gkt.sufxvd.cn

[E04] 查找子串位置
来源：http://tph.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://vsb.bbcook.cn

PHP:  strpos($s, "x");
来源：http://hib.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kuo.daria6918.cn

TS:   s.indexOf("x")
来源：http://atp.cqqwz.cn

Java: s.indexOf("x")
来源：http://eed.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://nco.yangfankeji.com

Ruby: s.index("x")
来源：http://zqm.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://wto.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iey.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qnx.yj20258888.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nev.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ztt.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://crc.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kly.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jve.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iqx.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nxa.jinghuilouyu.cn


<!-- 参考信息 -->