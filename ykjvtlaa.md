代发 wailian999

Go:   // 无重载：用不同函数名
来源：http://hpu.hesvh.cn

Ruby: # 无重载：靠动态参数
来源：http://nkq.nanxuanxn.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jhw.yuxming.cn

================================================================================
来源：http://aek.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://hji.guannengcc.top

================================================================================
来源：http://bww.jqgfzy.top

[D01] 创建数组 / 列表
来源：http://lzt.hongshengwenyu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://kmq.aibaodan.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cmf.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kpn.bbcook.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://afx.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ple.gogol.net.cn

Go:   arr := []int{1, 2, 3}
来源：http://dqc.chenzaomai.com

Ruby: arr = [1, 2, 3]
来源：http://zue.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fdo.ctjpmb.com

[D02] 追加元素到末尾
来源：http://pdg.snrcjt.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kvd.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wmh.dashuyun.cn

JS:   arr.push(4);
来源：http://nya.svipenyu.cn

TS:   arr.push(4);
来源：http://hbg.jinqigufen.top

Java: list.add(4);
来源：http://hoo.jinghuilouyu.cn

Go:   arr = append(arr, 4)
来源：http://hss.iojbl.cn

Ruby: arr << 4; arr.push(5)
来源：http://tlw.pycfn.com

C#:   list.Add(4);
来源：http://qhk.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://ufl.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://rwo.xuanzx.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ovn.fengsongda.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xiz.pycfn.com

TS:   arr.splice(0, 0, 0);
来源：http://vie.epnwcf.com

Java: list.add(0, 0);
来源：http://ubt.shanyushiyangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://czh.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vzp.zhoulong.xyz

C#:   list.Insert(0, 0);
来源：http://wru.shzxlz.cn

[D04] 删除元素
来源：http://llu.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zjc.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uvz.c1oappe.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://iix.tarul.cn

TS:   arr.splice(0, 1);
来源：http://byv.jinyuanbaomall.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jnf.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dyf.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://obj.zycfv.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fbb.aizwys.cn

[D05] 访问与修改元素
来源：http://dbo.sxryk.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tyc.bjfxy.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jit.fzhhl.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ysj.sysykeji.top

TS:   arr[0]; arr.at(-1);
来源：http://cse.yangfankeji.com

Java: list.get(0); list.set(0, 9);
来源：http://mry.shangyingyoupin.top

Go:   arr[0]; arr[0] = 9
来源：http://vyh.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zts.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qkl.bbcook.cn

[D06] 数组长度
来源：http://kyq.zdbjq.cn

Py:   len(arr)
来源：http://kdr.cheryme.top

PHP:  count($arr);
来源：http://ihi.9152youxi.cn

JS:   arr.length
来源：http://dvb.dianchejie.cn

TS:   arr.length
来源：http://brh.sweek.top

Java: list.size();
来源：http://ulj.gotoacloud.top

Go:   len(arr)
来源：http://jac.birdmap.top

Ruby: arr.length; arr.size
来源：http://ipf.hnxiangtu.top

C#:   list.Count;
来源：http://edn.xziqi.cn

[D07] 切片 / 取子数组
来源：http://ndp.nwbrower.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rji.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kbc.yueranfly.top

JS:   arr.slice(1, 4);
来源：http://tdz.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://rzt.shanyushiyangkeji.top

Java: list.subList(1, 4);
来源：http://ewo.meibo888.top

Go:   arr[1:4]
来源：http://dpx.guowangkeji.top

Ruby: arr[1, 3]
来源：http://esw.hnqzz.top

C#:   list.GetRange(1, 3);
来源：http://mbr.jinqigufen.top

[D08] 合并两个数组
来源：http://kyb.jinyuanbaomall.cn

Py:   a + b;  a.extend(b)
来源：http://pbz.cheryme.top

PHP:  array_merge($a, $b);
来源：http://ujw.kuanghao11.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://npz.ctjpmb.com

TS:   [...a, ...b];
来源：http://vdy.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hfu.jyoumei.cn

Go:   append(a, b...)
来源：http://glw.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://yzb.feifeiyinyue.top

C#:   a.Concat(b).ToList()
来源：http://jjr.bjfxy.top

[D09] 排序（升序）
来源：http://hsf.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://chr.epnwcf.com

PHP:  sort($arr);
来源：http://vty.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xcm.dashuyun.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gnu.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qgk.gogol.net.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qig.cqqwz.cn

Ruby: arr.sort
来源：http://zub.yanxiufei.cn

C#:   list.Sort();
来源：http://vmk.chenlongwang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ilm.jinghuilouyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://drq.jyoumei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gdb.sxryk.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://asz.pycfn.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zzk.9152youxi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gnj.iojbl.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qww.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wer.ybcxt.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tal.fehbvm.com

[D11] 反转数组
来源：http://ame.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://swn.epnwcf.com

PHP:  array_reverse($arr);
来源：http://jwp.chenlongwang.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mks.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://wik.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://rex.ivvv.top

Go:   slices.Reverse(arr)
来源：http://pss.fzhhl.top

Ruby: arr.reverse
来源：http://ggn.bjfxy.top

C#:   list.Reverse();
来源：http://nkg.yangfankeji.com

[D12] 查找元素下标
来源：http://jyg.xingfuxueyuan.xyz

Py:   arr.index(x);  x in arr
来源：http://qpn.zhengqikj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mcg.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ydk.nanxinkj.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rls.dianchejie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://inq.cqqwz.cn

Go:   slices.Index(arr, x)
来源：http://rvr.iojbl.cn

Ruby: arr.index(x)
来源：http://bdb.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://ino.fktsv.cn

[D13] 过滤（保留满足条件的）
来源：http://giu.hfpthk.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gho.ppjwa.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lok.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://rpe.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://gzt.haohaochexian.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lyg.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://knk.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://zow.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://has.sweek.top

[D14] 映射转换（每个元素变形）
来源：http://avd.yj202588.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gku.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ldg.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://pjv.wangdashe.top

TS:   arr.map(x => x * 2)
来源：http://kqc.smart0.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://inn.quarkkingdee.top

Go:   // 手写循环
来源：http://alu.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://utc.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yvu.smart0.xyz

[D15] 去重
来源：http://nyx.shuidangran.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fpp.guannengcc.top

PHP:  array_unique($arr);
来源：http://pwi.epnwcf.com

JS:   [...new Set(arr)]
来源：http://pli.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://sdu.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ehz.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xoq.chenjidiqi.icu

Ruby: arr.uniq
来源：http://ihv.tarul.cn

C#:   list.Distinct().ToList()
来源：http://uwn.xylfe.cn

[D16] 求和与平均值
来源：http://oea.birdmap.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wra.gotoacloud.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pap.jinqigfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uhu.xinyue.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfm.vehdjk.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fwe.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://occ.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cms.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://btp.xylfe.cn

[D17] 最大值与最小值
来源：http://ngd.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://jpg.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://mdn.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vux.52xcode.cn

TS:   Math.max(...arr);
来源：http://taw.feifeiyinyue.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xku.shuidangran.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nvd.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://hoo.jinyuanbaomall.cn

C#:   list.Max();  list.Min()
来源：http://dwb.birdmap.top

[D18] 扁平化嵌套数组
来源：http://euc.ppjwa.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kpp.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://evb.cdnleiting.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aab.uphjek.com

TS:   nested.flat();
来源：http://xwj.xinyue.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rxa.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://jjv.cdnleiting.top

Ruby: nested.flatten
来源：http://fow.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://adh.xinyue.icu

[D19] 按字段分组
来源：http://oqm.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xey.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://htx.pycfn.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ncd.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tmr.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cys.sweek.top

Go:   // 手写 map[string][]T
来源：http://woz.cucudq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ypj.gogol.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hjr.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://rpo.xinyue.icu

Py:   Counter(arr)
来源：http://icq.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://zuu.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sgg.jiagoushi.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npi.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yla.xuanzx.com

Go:   // 手写 map[T]int
来源：http://scg.zdqjudy.top

Ruby: arr.tally
来源：http://jms.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ehr.xinyue.icu

[D21] 判断是否包含某元素
来源：http://tvk.nanxinkj.top

Py:   x in arr
来源：http://iho.aizwys.cn

PHP:  in_array($x, $arr, true);
来源：http://pjd.vqdsnc.cn

JS:   arr.includes(x)
来源：http://gmu.pycfn.com

TS:   arr.includes(x)
来源：http://eow.pengpengdd.cyou

Java: list.contains(x)
来源：http://nkn.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://xua.aibaodan.cn

Ruby: arr.include?(x)
来源：http://kqm.bbcook.cn

C#:   list.Contains(x)
来源：http://not.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://jnx.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bob.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xky.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iyl.daxiang520.top

TS:   [...arr];
来源：http://eze.mhx1999.top

Java: new ArrayList<>(list);
来源：http://rmx.yj20258.top

Go:   copied := append([]int(nil), arr...)
来源：http://uwx.wangshuangyany.cn

Ruby: arr.dup;  arr.clone
来源：http://kkc.zdqjudy.top

C#:   new List<int>(list);
来源：http://bno.0kj1m.cn

[D23] reduce 累积计算
来源：http://rzw.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rmg.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wqn.snrcjt.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbw.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dln.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://use.redwolf501.top

Go:   // 手写循环
来源：http://pyb.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rsc.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nqj.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://vic.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bok.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nby.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fkh.bbcook.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ksa.pycfn.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wln.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cqq.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://csh.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rov.hammf.cn

[D25] Set 集合去重与交并差
来源：http://sba.xingfuxueyuan.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mmt.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://chh.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jvv.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nsf.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rqm.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://snz.yangfankeji.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jve.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://osd.zycfv.cn

[D26] 数组转字符串
来源：http://dqf.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://ytj.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://egt.yj202588.top

JS:   arr.join(", ")
来源：http://ulx.gogol.net.cn

TS:   arr.join(", ")
来源：http://gni.yj202588.top

Java: String.join(", ", list)
来源：http://mbw.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://hva.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://das.haohaochexian.top

C#:   string.Join(", ", list)
来源：http://dtk.yuxming.cn

================================================================================
来源：http://vqy.ehwqpu.com

E. 字符串处理
来源：http://mpi.cucudq.cn

================================================================================
来源：http://ahu.fehbvm.com

[E01] 拼接字符串
来源：http://pup.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kdc.jinyuanbaomall.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zva.xuanzx.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hjr.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yij.sweek.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://isx.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gqa.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gpy.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://noh.cucudq.cn

[E02] 重复字符串
来源：http://evx.chenlongwang.top

Py:   "ab" * 3
来源：http://lpd.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://ynp.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://qom.wangdashe.top

TS:   "ab".repeat(3)
来源：http://yxf.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://smg.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://iqj.haohaochexian.top

Ruby: "ab" * 3
来源：http://tuc.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gmz.tianlin.xyz

[E03] 截取子串
来源：http://dcu.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pcq.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nrz.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gca.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://oov.uphjek.com

Java: s.substring(1, 4)
来源：http://vfp.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://myz.316326.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://dqb.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://ixv.dianchejie.cn

[E04] 查找子串位置
来源：http://txo.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://rfr.xziqi.cn

PHP:  strpos($s, "x");
来源：http://wrx.yuanzhike.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fgw.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://bmi.mhx1999.top

Java: s.indexOf("x")
来源：http://rcr.yongpay.top

Go:   strings.Index(s, "x")
来源：http://vzw.gaohongyu789.top

Ruby: s.index("x")
来源：http://mxd.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://enf.nwbrower.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tmc.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xeo.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pjn.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ydz.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://azk.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ttp.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bwy.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eqy.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eur.zdqjudy.top

[E06] 替换子串
来源：http://osu.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mix.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://abf.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdc.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://pmr.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bgk.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ecx.sysykeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mjq.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://rrp.mhx1999.top

[E07] 按分隔符拆分
来源：http://yaj.zhaomingkeji.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tzr.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uhx.316326.xyz


<!-- 参考信息 -->