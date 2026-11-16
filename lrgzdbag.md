代发 wailian999

D. 数组 / 列表 / 集合
来源：http://dzz.haohaochexian.top

================================================================================
来源：http://qoh.zhongyouzk.top

[D01] 创建数组 / 列表
来源：http://jvt.ivvv.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ohh.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://klp.aibaodan.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gzi.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ozd.shanyushiyangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qha.wangdashe.top

Go:   arr := []int{1, 2, 3}
来源：http://nex.tarul.cn

Ruby: arr = [1, 2, 3]
来源：http://pbe.gaohongyu789.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iol.yanxiufei.cn

[D02] 追加元素到末尾
来源：http://gna.dianchejie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rfe.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hmo.xylfe.cn

JS:   arr.push(4);
来源：http://zmq.jiagoushi.top

TS:   arr.push(4);
来源：http://dbm.xinyue.icu

Java: list.add(4);
来源：http://kye.yueranfly.top

Go:   arr = append(arr, 4)
来源：http://tqi.fanxiaobao.xyz

Ruby: arr << 4; arr.push(5)
来源：http://lxe.gotoacloud.top

C#:   list.Add(4);
来源：http://ajz.fktsv.cn

[D03] 在指定位置插入元素
来源：http://bge.hammf.cn

Py:   arr.insert(0, 0)
来源：http://mvr.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wmj.hfpthk.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://txe.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://fnz.bbcook.cn

Java: list.add(0, 0);
来源：http://tsy.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dqb.fanxiaobao.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wun.zhongyouzk.top

C#:   list.Insert(0, 0);
来源：http://pze.jinqigufen.top

[D04] 删除元素
来源：http://fmo.yuanzhike.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kby.tanke756.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ktn.gogol.net.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zhs.shanyushiyangtech.top

TS:   arr.splice(0, 1);
来源：http://iom.mhx1999.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hqz.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://knp.vqdsnc.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pdg.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lgj.quarkkingdee.top

[D05] 访问与修改元素
来源：http://ofq.jiagoushi.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xwr.yanxiufei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://taj.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sgx.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://mim.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://xxf.bbcook.cn

Go:   arr[0]; arr[0] = 9
来源：http://gtc.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jql.hesvh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vck.jqgfzy.top

[D06] 数组长度
来源：http://jzb.birdmap.top

Py:   len(arr)
来源：http://sxu.tianlin.xyz

PHP:  count($arr);
来源：http://snh.hnqzz.top

JS:   arr.length
来源：http://grh.yj20258.top

TS:   arr.length
来源：http://ctj.hammf.cn

Java: list.size();
来源：http://vhd.gogol.net.cn

Go:   len(arr)
来源：http://qkb.sweek.top

Ruby: arr.length; arr.size
来源：http://bqv.zhiwuduotai.top

C#:   list.Count;
来源：http://xtr.9152youxi.cn

[D07] 切片 / 取子数组
来源：http://owb.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://vry.xylfe.cn

PHP:  array_slice($arr, 1, 3);
来源：http://azb.chenlongwang.top

JS:   arr.slice(1, 4);
来源：http://qja.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://kxh.hcnkem.com

Java: list.subList(1, 4);
来源：http://rae.nanxuanxn.top

Go:   arr[1:4]
来源：http://ewn.havefunace.top

Ruby: arr[1, 3]
来源：http://afe.snrcjt.cn

C#:   list.GetRange(1, 3);
来源：http://imy.ehwqpu.com

[D08] 合并两个数组
来源：http://emr.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://nyd.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://rua.sysykeji.top

JS:   [...a, ...b];  a.concat(b);
来源：http://asu.zhiwuduotai.top

TS:   [...a, ...b];
来源：http://gbm.xylfe.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://upz.smart0.xyz

Go:   append(a, b...)
来源：http://edn.pycfn.com

Ruby: a + b;  a.concat(b)
来源：http://bdj.9152youxi.cn

C#:   a.Concat(b).ToList()
来源：http://vgq.tian-w.cn

[D09] 排序（升序）
来源：http://ivv.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://ocv.pycfn.com

PHP:  sort($arr);
来源：http://yqk.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ozp.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bwg.zhixingplan.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pak.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wzv.dashuyun.cn

Ruby: arr.sort
来源：http://bza.fktsv.cn

C#:   list.Sort();
来源：http://nuh.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fmi.chenlongwang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mmz.yj20258.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tbj.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yob.dashuyun.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://swp.snrcjt.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kbo.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://iap.dashuyun.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yky.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zhv.zhixingplan.top

[D11] 反转数组
来源：http://lpq.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://enu.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://vjg.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ioo.hysaishi.cn

TS:   [...arr].reverse();
来源：http://spy.52xcode.cn

Java: Collections.reverse(list);
来源：http://qif.fengsongda.top

Go:   slices.Reverse(arr)
来源：http://bno.gotoacloud.top

Ruby: arr.reverse
来源：http://ckm.yj202588.top

C#:   list.Reverse();
来源：http://nli.zdqjudy.top

[D12] 查找元素下标
来源：http://miu.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://njw.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xgl.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pry.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hws.redwolf501.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xzk.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://dbh.fengsongda.top

Ruby: arr.index(x)
来源：http://bud.shangyingyoupin.top

C#:   list.IndexOf(x);
来源：http://fdg.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://hac.aizwys.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vte.vehdjk.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gbq.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://opq.zdbjq.cn

TS:   arr.filter(x => x > 3)
来源：http://fpl.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bog.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gtw.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://qto.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sle.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://cds.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xfy.ydzc1.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dmw.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://gaq.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://vuf.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tmy.jinghuilouyu.cn

Go:   // 手写循环
来源：http://xvy.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://hew.hcnkem.com

C#:   list.Select(x => x * 2).ToList()
来源：http://orr.ehwqpu.com

[D15] 去重
来源：http://clg.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fso.ybcxt.top

PHP:  array_unique($arr);
来源：http://hnk.bbcook.cn

JS:   [...new Set(arr)]
来源：http://faj.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://stg.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dno.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://ywb.xuetiantiany.cn

Ruby: arr.uniq
来源：http://pfd.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://pff.birdmap.top

[D16] 求和与平均值
来源：http://phv.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ror.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rqr.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://egv.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wtq.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ptx.pengpengdd.cyou

Go:   // 手写循环累加
来源：http://xra.mhx1999.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jpc.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://nmx.dianchejie.cn

[D17] 最大值与最小值
来源：http://kos.ywan-chungtsiang.top

Py:   max(arr);  min(arr)
来源：http://tns.gogol.net.cn

PHP:  max($arr);  min($arr);
来源：http://zww.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dsn.jyoumei.cn

TS:   Math.max(...arr);
来源：http://rdi.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://yzo.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ntz.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://xbm.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://iwk.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://cet.fehbvm.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lck.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://fto.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sbr.bbcook.cn

TS:   nested.flat();
来源：http://cst.gzhubu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://adu.sufxvd.cn

Go:   // 手写双层循环
来源：http://ovn.yuxming.cn

Ruby: nested.flatten
来源：http://ttk.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sxb.cdnleiting.top

[D19] 按字段分组
来源：http://jvm.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lqw.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hap.mhx1999.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kgy.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://tvd.gotoacloud.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pzk.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://eqa.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://egw.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://idv.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://jda.feifeiyinyue.top

Py:   Counter(arr)
来源：http://tqh.wangshuangyany.cn

PHP:  array_count_values($arr);
来源：http://qgs.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hpr.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jeb.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://avm.mhx1999.top

Go:   // 手写 map[T]int
来源：http://kbm.vehdjk.com

Ruby: arr.tally
来源：http://tcp.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xtc.mhx1999.top

[D21] 判断是否包含某元素
来源：http://mru.yuanzhike.top

Py:   x in arr
来源：http://fmm.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://wfu.havefunace.top

JS:   arr.includes(x)
来源：http://tas.cashguo.top

TS:   arr.includes(x)
来源：http://siy.fanxiaobao.xyz

Java: list.contains(x)
来源：http://npr.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://bwu.316326.xyz

Ruby: arr.include?(x)
来源：http://zpk.dianchejie.cn

C#:   list.Contains(x)
来源：http://afo.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://exi.hesvh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jqx.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbv.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rxg.kuanghao11.cn

TS:   [...arr];
来源：http://rag.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://ekd.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://ieh.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://wyj.iojbl.cn

C#:   new List<int>(list);
来源：http://sqy.fehbvm.com

[D23] reduce 累积计算
来源：http://xhr.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://roh.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tew.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yoh.9152youxi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nhp.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yyd.ehwqpu.com

Go:   // 手写循环
来源：http://tbx.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kds.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yki.vehdjk.com

[D24] 字典 / Map 基本操作
来源：http://izn.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jsj.chenjidiqi.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xwc.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lny.316326.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://drf.sjlbkw.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://als.jinyuanbaomall.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rlb.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uxy.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zzr.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://cux.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://thp.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oiq.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xdm.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jck.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fyu.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://few.jinqigfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hbl.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fur.zdbjq.cn

[D26] 数组转字符串
来源：http://jvw.havefunace.top

Py:   ", ".join(map(str, arr))
来源：http://sfn.zhaomingkeji.xyz

PHP:  implode(", ", $arr);
来源：http://xdy.zhengqikj.top

JS:   arr.join(", ")
来源：http://tsq.shzxlz.cn

TS:   arr.join(", ")
来源：http://qfg.yj202588.top

Java: String.join(", ", list)
来源：http://jby.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://ezy.ydzc1.top

Ruby: arr.join(", ")
来源：http://llw.zhongyouzk.top

C#:   string.Join(", ", list)
来源：http://zpz.0kj1m.cn

================================================================================
来源：http://fuh.quarkkingdee.top

E. 字符串处理
来源：http://wbs.xuanzx.com

================================================================================
来源：http://ehx.gogol.net.cn

[E01] 拼接字符串
来源：http://jxi.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owl.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lke.sufxvd.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://krn.gogol.net.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kaz.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pyc.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tan.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iaj.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vue.yuxming.cn

[E02] 重复字符串
来源：http://rcz.pengpengdd.cyou

Py:   "ab" * 3
来源：http://zdb.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://qtu.havefunace.top

JS:   "ab".repeat(3)
来源：http://lvk.bbcook.cn

TS:   "ab".repeat(3)
来源：http://the.52xcode.cn

Java: "ab".repeat(3)
来源：http://kpi.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://bpm.xziqi.cn

Ruby: "ab" * 3
来源：http://rlu.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://odw.ywan-chungtsiang.top

[E03] 截取子串
来源：http://wmd.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://deg.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tdf.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yoy.hesvh.cn

TS:   s.slice(1, 4)
来源：http://xtk.gogol.net.cn

Java: s.substring(1, 4)
来源：http://kxx.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gom.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://vpb.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://fkz.wangshuangyany.cn

[E04] 查找子串位置
来源：http://wxx.jianghu66.top

Py:   s.find("x");  s.index("x")
来源：http://gow.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://znc.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kdl.zhengqikj.top

TS:   s.indexOf("x")
来源：http://rgd.hywenlv.cn

Java: s.indexOf("x")
来源：http://vmt.tanke756.top

Go:   strings.Index(s, "x")
来源：http://hxj.fengsongda.top

Ruby: s.index("x")
来源：http://wxl.yfazqb.com

C#:   s.IndexOf("x")
来源：http://tqo.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://raf.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xpc.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://slf.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ely.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lal.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ski.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bpy.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ctd.vqdsnc.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cvl.zhiwuduotai.top

[E06] 替换子串
来源：http://dmx.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://act.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://rea.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qfn.chenjidiqi.icu

TS:   s.replaceAll("a", "b")
来源：http://mio.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rbq.snrcjt.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjn.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qfz.pycfn.com

C#:   s.Replace("a", "b")
来源：http://ssw.yvedp.cn

[E07] 按分隔符拆分
来源：http://kbx.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://egu.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://avg.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://njn.guannengcc.top

TS:   s.split(",")
来源：http://zta.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ofz.c1oappe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gwd.gotoacloud.top


<!-- 参考信息 -->