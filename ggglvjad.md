代发 wailian999

Ruby: a, b = pair
来源：http://iah.yvedp.cn

C#:   var (a, b) = pair;
来源：http://zep.gogol.net.cn

[C16] 函数 / 方法重载
来源：http://xep.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xzp.cqqwz.cn

PHP:  // 无重载
来源：http://mtd.sufxvd.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ant.nanxuanxn.top

TS:   // 用联合类型或重载签名声明
来源：http://uaz.yongpay.top

Java: void f(int a) {}  void f(String a) {}
来源：http://qqw.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://xdg.fzhhl.top

Ruby: # 无重载：靠动态参数
来源：http://obr.daria6918.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://igu.hcnkem.com

================================================================================
来源：http://eat.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://stf.redwolf501.top

================================================================================
来源：http://hpp.jinyuanbaomall.cn

[D01] 创建数组 / 列表
来源：http://sdp.daria6918.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zgx.gotoacloud.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fjl.hfpthk.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ptz.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://akp.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wbs.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://kgy.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://qvv.aizwys.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cdu.havefunace.top

[D02] 追加元素到末尾
来源：http://fev.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ywn.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tvb.hammf.cn

JS:   arr.push(4);
来源：http://ypw.cucudq.cn

TS:   arr.push(4);
来源：http://djt.fzhhl.top

Java: list.add(4);
来源：http://wbm.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://oee.zdbjq.cn

Ruby: arr << 4; arr.push(5)
来源：http://cze.jlsjyb.cn

C#:   list.Add(4);
来源：http://onq.havefunace.top

[D03] 在指定位置插入元素
来源：http://kmp.0kj1m.cn

Py:   arr.insert(0, 0)
来源：http://wtl.xylfe.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kel.meibo888.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pzw.yvedp.cn

TS:   arr.splice(0, 0, 0);
来源：http://usm.havefunace.top

Java: list.add(0, 0);
来源：http://coc.vqdsnc.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xtu.yj20258888.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vxa.andypj.xyz

C#:   list.Insert(0, 0);
来源：http://woe.ctjpmb.com

[D04] 删除元素
来源：http://qvy.316326.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wjf.c1oappe.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xub.guannengcc.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bfw.jinqigfzy.top

TS:   arr.splice(0, 1);
来源：http://osi.cdnleiting.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qkk.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zst.xingfuxueyuan.xyz

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ldv.zdbjq.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fla.shangyingyoupin.top

[D05] 访问与修改元素
来源：http://shq.mhx1999.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wsj.shzxlz.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xun.fanxiaobao.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mko.meibo888.top

TS:   arr[0]; arr.at(-1);
来源：http://stq.aizwys.cn

Java: list.get(0); list.set(0, 9);
来源：http://zuo.guowangkeji.top

Go:   arr[0]; arr[0] = 9
来源：http://bvl.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qew.guannengcc.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://vpv.sjlbkw.cn

[D06] 数组长度
来源：http://ada.ywan-chungtsiang.top

Py:   len(arr)
来源：http://zuv.aibaodan.cn

PHP:  count($arr);
来源：http://ocf.zhongyouzk.top

JS:   arr.length
来源：http://oda.yj20258.top

TS:   arr.length
来源：http://hjy.zdbjq.cn

Java: list.size();
来源：http://idp.hesvh.cn

Go:   len(arr)
来源：http://byf.tanke756.top

Ruby: arr.length; arr.size
来源：http://qwr.hammf.cn

C#:   list.Count;
来源：http://yyl.gotoacloud.top

[D07] 切片 / 取子数组
来源：http://ueo.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jwg.uphjek.com

PHP:  array_slice($arr, 1, 3);
来源：http://ann.9152youxi.cn

JS:   arr.slice(1, 4);
来源：http://msi.yfazqb.com

TS:   arr.slice(1, 4);
来源：http://mey.shuidangran.top

Java: list.subList(1, 4);
来源：http://scu.daria6918.cn

Go:   arr[1:4]
来源：http://umu.haohaochexian.top

Ruby: arr[1, 3]
来源：http://gxg.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://mfe.cucudq.cn

[D08] 合并两个数组
来源：http://isc.shanyushiyangkeji.top

Py:   a + b;  a.extend(b)
来源：http://ucj.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://fua.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qqf.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://tuk.yj20258888.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jrj.chenjidiqi.icu

Go:   append(a, b...)
来源：http://fkm.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://xsn.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://ccw.jinqigfzy.top

[D09] 排序（升序）
来源：http://qwp.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://sdu.xylfe.cn

PHP:  sort($arr);
来源：http://bxw.gzhubu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://era.svipenyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xbc.yongpay.top

Java: Collections.sort(list);  list.sort(null);
来源：http://mfp.zhiwuduotai.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mui.havefunace.top

Ruby: arr.sort
来源：http://tcu.yj20258.top

C#:   list.Sort();
来源：http://dzj.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://kxv.cucudq.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xmi.dianchejie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baa.yvedp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://inf.yj20258888.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nck.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hjs.fanxiaobao.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oui.ybcxt.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://htw.jinqigufen.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kst.aibaodan.cn

[D11] 反转数组
来源：http://tbi.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dmq.birdmap.top

PHP:  array_reverse($arr);
来源：http://rrm.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://izo.vehdjk.com

TS:   [...arr].reverse();
来源：http://tqc.sjlbkw.cn

Java: Collections.reverse(list);
来源：http://uhn.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://tme.ydzc1.top

Ruby: arr.reverse
来源：http://bek.52xcode.cn

C#:   list.Reverse();
来源：http://eaa.fzhhl.top

[D12] 查找元素下标
来源：http://xgm.zhijiandao.cn

Py:   arr.index(x);  x in arr
来源：http://oad.jinghuilouyu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pim.zhixingplan.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jod.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://opi.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vtb.jlsjyb.cn

Go:   slices.Index(arr, x)
来源：http://qca.hnqzz.top

Ruby: arr.index(x)
来源：http://mdu.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://hyu.hammf.cn

[D13] 过滤（保留满足条件的）
来源：http://dau.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cra.feifeiyinyue.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ait.yongpay.top

JS:   arr.filter(x => x > 3)
来源：http://kae.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://eee.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ruq.sxryk.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ojq.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gjv.aibaodan.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ust.gaohongyu789.top

[D14] 映射转换（每个元素变形）
来源：http://dql.kuanghao11.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qqi.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mag.xuetiantiany.cn

JS:   arr.map(x => x * 2)
来源：http://nmp.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://rjd.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pcg.zdqjudy.top

Go:   // 手写循环
来源：http://jza.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://ngk.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gdy.smart0.xyz

[D15] 去重
来源：http://yme.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wvt.yuxming.cn

PHP:  array_unique($arr);
来源：http://pix.hongshengwenyu.top

JS:   [...new Set(arr)]
来源：http://drt.hongshengwenyu.top

TS:   [...new Set(arr)]
来源：http://tep.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bhf.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://lsb.hysaishi.cn

Ruby: arr.uniq
来源：http://ian.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://bfl.yvedp.cn

[D16] 求和与平均值
来源：http://xfe.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sff.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bvt.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://stk.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajm.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://duj.hammf.cn

Go:   // 手写循环累加
来源：http://cdg.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dth.gaohongyu789.top

C#:   list.Sum();  list.Average()
来源：http://pre.feifeiyinyue.top

[D17] 最大值与最小值
来源：http://ino.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://fjp.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://aaj.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://reu.pycfn.com

TS:   Math.max(...arr);
来源：http://lsw.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mpi.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jov.gaohongyu789.top

Ruby: arr.max;  arr.min
来源：http://wwr.ivvv.top

C#:   list.Max();  list.Min()
来源：http://cab.zhijiandao.cn

[D18] 扁平化嵌套数组
来源：http://xxd.ehwqpu.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ezo.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://okr.sjlbkw.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dez.sweek.top

TS:   nested.flat();
来源：http://ntj.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oxq.ivvv.top

Go:   // 手写双层循环
来源：http://mag.bjfxy.top

Ruby: nested.flatten
来源：http://mco.cdnleiting.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sdz.zdqjudy.top

[D19] 按字段分组
来源：http://ete.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fwi.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uoc.aibaodan.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nbt.yj20258888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hyg.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cdv.yvedp.cn

Go:   // 手写 map[string][]T
来源：http://stb.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gad.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ftd.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://smp.sufxvd.cn

Py:   Counter(arr)
来源：http://fox.birdmap.top

PHP:  array_count_values($arr);
来源：http://tqb.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wnq.epnwcf.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rda.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lwu.gzhubu.top

Go:   // 手写 map[T]int
来源：http://kpu.316326.xyz

Ruby: arr.tally
来源：http://lzq.xuanzx.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uzz.gzhubu.top

[D21] 判断是否包含某元素
来源：http://zrs.feifeiyinyue.top

Py:   x in arr
来源：http://cvn.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://ujp.fengsongda.top

JS:   arr.includes(x)
来源：http://gti.bbcook.cn

TS:   arr.includes(x)
来源：http://wbt.xuanzx.com

Java: list.contains(x)
来源：http://zlw.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://lcc.aizwys.cn

Ruby: arr.include?(x)
来源：http://vwt.shzxlz.cn

C#:   list.Contains(x)
来源：http://bhm.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://xqz.hnxiangtu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fta.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uph.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ttv.xylfe.cn

TS:   [...arr];
来源：http://yqw.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://dqe.fengsongda.top

Go:   copied := append([]int(nil), arr...)
来源：http://fye.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://squ.jiagoushi.top

C#:   new List<int>(list);
来源：http://pgd.yueranfly.top

[D23] reduce 累积计算
来源：http://nmt.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ler.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://irf.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://imd.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mui.zhixingplan.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uba.xuanzx.com

Go:   // 手写循环
来源：http://dxb.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gka.xylfe.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hqn.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://dtz.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tct.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mmy.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gwb.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://exf.xingfuxueyuan.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ffl.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jlz.yfazqb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sdb.birdmap.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://eby.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://ato.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ibx.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pmm.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wgk.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cbk.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mfm.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vea.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eje.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwu.daria6918.cn

[D26] 数组转字符串
来源：http://vtq.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://gmm.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://yrg.haohaochexian.top

JS:   arr.join(", ")
来源：http://lpw.dashuyun.cn

TS:   arr.join(", ")
来源：http://oba.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://zkx.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://pbq.hcnkem.com

Ruby: arr.join(", ")
来源：http://swn.sweek.top

C#:   string.Join(", ", list)
来源：http://eeg.hnqzz.top

================================================================================
来源：http://eex.zhongyouzk.top

E. 字符串处理
来源：http://sqw.xylfe.cn

================================================================================
来源：http://dpv.hammf.cn

[E01] 拼接字符串
来源：http://fye.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://awr.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nfb.zhijiandao.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ezm.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ztv.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://igf.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xzo.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yok.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jso.jlsjyb.cn

[E02] 重复字符串
来源：http://uyz.316326.xyz

Py:   "ab" * 3
来源：http://bmj.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://pym.redwolf501.top

JS:   "ab".repeat(3)
来源：http://vpc.xuanzx.com

TS:   "ab".repeat(3)
来源：http://iwt.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://nyd.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://gij.shuidangran.top

Ruby: "ab" * 3
来源：http://mis.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://utx.zhijiandao.cn

[E03] 截取子串
来源：http://hue.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://thr.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lju.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lwb.birdmap.top

TS:   s.slice(1, 4)
来源：http://nbn.nanxinkj.top

Java: s.substring(1, 4)
来源：http://gbo.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://laz.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://vrs.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://zwp.tanke756.top

[E04] 查找子串位置
来源：http://nwk.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://sac.ivvv.top

PHP:  strpos($s, "x");
来源：http://qnh.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rwk.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://ctg.zhixingplan.top

Java: s.indexOf("x")
来源：http://wkv.cdnleiting.top

Go:   strings.Index(s, "x")
来源：http://udd.316326.xyz

Ruby: s.index("x")
来源：http://uvn.dianchejie.cn

C#:   s.IndexOf("x")
来源：http://lab.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://trz.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://phv.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cwi.tanke756.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vae.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://thw.daria6918.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ebc.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gtn.kuanghao11.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rwn.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uaj.yueranfly.top

[E06] 替换子串
来源：http://nix.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cnh.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://eov.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aov.chenlongwang.top


<!-- 参考信息 -->