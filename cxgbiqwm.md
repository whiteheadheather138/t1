代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aqq.xinyue.icu

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lnw.tianlin.xyz

Java: // 无解构
来源：http://ofb.xylfe.cn

Go:   // 无解构
来源：http://oav.gogol.net.cn

Ruby: a, b = pair
来源：http://udv.chenzaomai.com

C#:   var (a, b) = pair;
来源：http://wbf.bbcook.cn

[C16] 函数 / 方法重载
来源：http://rix.yueranfly.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vsv.sufxvd.cn

PHP:  // 无重载
来源：http://wcd.yuanzhike.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lgd.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://fzr.hfpthk.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://elw.shanyushiyangtech.top

Go:   // 无重载：用不同函数名
来源：http://nff.wangdashe.top

Ruby: # 无重载：靠动态参数
来源：http://ran.daxiang520.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oqk.sxryk.cn

================================================================================
来源：http://msy.xuanzx.com

D. 数组 / 列表 / 集合
来源：http://lms.haohaochexian.top

================================================================================
来源：http://vzn.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://kxu.iojbl.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cco.316326.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zjs.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zen.cqqwz.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://emm.zhengqikj.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mst.bbcook.cn

Go:   arr := []int{1, 2, 3}
来源：http://evc.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://jxs.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fdl.gaohongyu789.top

[D02] 追加元素到末尾
来源：http://irc.sysykeji.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://moi.jqgufenzy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kgj.smart0.xyz

JS:   arr.push(4);
来源：http://pkh.316326.xyz

TS:   arr.push(4);
来源：http://auk.jqgufenzy.top

Java: list.add(4);
来源：http://hqu.sysykeji.top

Go:   arr = append(arr, 4)
来源：http://uxu.meibo888.top

Ruby: arr << 4; arr.push(5)
来源：http://xmv.ydjk.org.cn

C#:   list.Add(4);
来源：http://sdn.wangshuangyany.cn

[D03] 在指定位置插入元素
来源：http://dsh.zhijiandao.cn

Py:   arr.insert(0, 0)
来源：http://fzr.havefunace.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qwc.gzhubu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gda.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://mww.yangfankeji.com

Java: list.add(0, 0);
来源：http://emw.aizwys.cn

Go:   arr = append([]int{0}, arr...)
来源：http://cri.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://owi.xinyue.icu

C#:   list.Insert(0, 0);
来源：http://wnq.vqdsnc.cn

[D04] 删除元素
来源：http://slw.yangfankeji.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ktg.meibo888.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hhn.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cgg.xuetiantiany.cn

TS:   arr.splice(0, 1);
来源：http://ucv.chenzaomai.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://jjt.redwolf501.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ftx.nanxinkj.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xbi.pengpengdd.cyou

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://uxw.xylfe.cn

[D05] 访问与修改元素
来源：http://wco.tian-w.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mgs.yj20258.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gha.yongpay.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oie.ivvv.top

TS:   arr[0]; arr.at(-1);
来源：http://tdy.xziqi.cn

Java: list.get(0); list.set(0, 9);
来源：http://ufs.zhengqikj.top

Go:   arr[0]; arr[0] = 9
来源：http://ljk.ivvv.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wtp.ppjwa.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lid.yueranfly.top

[D06] 数组长度
来源：http://enr.iojbl.cn

Py:   len(arr)
来源：http://uvz.xziqi.cn

PHP:  count($arr);
来源：http://ugx.fehbvm.com

JS:   arr.length
来源：http://nvp.yongpay.top

TS:   arr.length
来源：http://whl.xinyue.icu

Java: list.size();
来源：http://ksn.bbcook.cn

Go:   len(arr)
来源：http://ndm.jianghu66.top

Ruby: arr.length; arr.size
来源：http://zwl.ydjk.org.cn

C#:   list.Count;
来源：http://rsx.snrcjt.cn

[D07] 切片 / 取子数组
来源：http://qxf.ybcxt.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jls.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://xfq.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://gsx.smart0.xyz

TS:   arr.slice(1, 4);
来源：http://bul.sweek.top

Java: list.subList(1, 4);
来源：http://apk.tarul.cn

Go:   arr[1:4]
来源：http://sis.jinyuanbaomall.cn

Ruby: arr[1, 3]
来源：http://jdc.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://jcu.ywan-chungtsiang.top

[D08] 合并两个数组
来源：http://uxq.yuxming.cn

Py:   a + b;  a.extend(b)
来源：http://pwi.yj202588.top

PHP:  array_merge($a, $b);
来源：http://bei.xuetiantiany.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vhv.yj20258888.top

TS:   [...a, ...b];
来源：http://xmp.dianchejie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pqw.guowangkeji.top

Go:   append(a, b...)
来源：http://gjs.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://hpa.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://gkg.smart0.xyz

[D09] 排序（升序）
来源：http://dcd.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://xqc.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://jet.sysykeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ciw.316326.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ghi.sysykeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pmd.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://vfl.meibo888.top

Ruby: arr.sort
来源：http://yzo.yongpay.top

C#:   list.Sort();
来源：http://att.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eql.nanxuanxn.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ken.shuidangran.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zvd.tianlin.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://msi.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yin.wangdashe.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pte.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mcf.hywenlv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ydp.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lfe.zhengqikj.top

[D11] 反转数组
来源：http://gpf.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://dao.fzhhl.top

PHP:  array_reverse($arr);
来源：http://olr.shuidangran.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qxa.jinghuilouyu.cn

TS:   [...arr].reverse();
来源：http://hdn.zhengqikj.top

Java: Collections.reverse(list);
来源：http://ldc.jiagoushi.top

Go:   slices.Reverse(arr)
来源：http://fob.sweek.top

Ruby: arr.reverse
来源：http://gzz.shuidangran.top

C#:   list.Reverse();
来源：http://ijw.sufxvd.cn

[D12] 查找元素下标
来源：http://amx.hongshengwenyu.top

Py:   arr.index(x);  x in arr
来源：http://ott.c1oappe.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://erd.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zcc.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ryq.sjlbkw.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fyt.ydjk.org.cn

Go:   slices.Index(arr, x)
来源：http://jkf.yfazqb.com

Ruby: arr.index(x)
来源：http://xsy.cdnleiting.top

C#:   list.IndexOf(x);
来源：http://ocd.smart0.xyz

[D13] 过滤（保留满足条件的）
来源：http://zli.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ctt.havefunace.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dwq.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://ifu.ywan-chungtsiang.top

TS:   arr.filter(x => x > 3)
来源：http://irb.havefunace.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hdx.hnxiangtu.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tim.zhiwuduotai.top

Ruby: arr.select { |x| x > 3 }
来源：http://gge.tanke756.top

C#:   list.Where(x => x > 3).ToList()
来源：http://xwc.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://wcs.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cpw.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://obj.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://kmk.dianchejie.cn

TS:   arr.map(x => x * 2)
来源：http://idd.yfazqb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://pja.shanyushiyangtech.top

Go:   // 手写循环
来源：http://qxl.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pjq.c1oappe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dmj.0kj1m.cn

[D15] 去重
来源：http://lmy.yj20258888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oof.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://kty.jyoumei.cn

JS:   [...new Set(arr)]
来源：http://tnv.yj202588.top

TS:   [...new Set(arr)]
来源：http://rte.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://asb.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://luo.yanxiufei.cn

Ruby: arr.uniq
来源：http://phx.cashguo.top

C#:   list.Distinct().ToList()
来源：http://vby.tian-w.cn

[D16] 求和与平均值
来源：http://yle.cucudq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://itm.dashuyun.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gph.yonumen.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vns.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://itg.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qvz.tianlin.xyz

Go:   // 手写循环累加
来源：http://aei.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://knc.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://jjv.haohaochexian.top

[D17] 最大值与最小值
来源：http://vny.ppjwa.cn

Py:   max(arr);  min(arr)
来源：http://zan.epnwcf.com

PHP:  max($arr);  min($arr);
来源：http://oip.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://atn.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://wal.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://civ.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://urt.pengpengdd.cyou

Ruby: arr.max;  arr.min
来源：http://nhn.vqdsnc.cn

C#:   list.Max();  list.Min()
来源：http://yss.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://fpz.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lot.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://lgb.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://itf.pengpengdd.cyou

TS:   nested.flat();
来源：http://slh.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xjd.daxiang520.top

Go:   // 手写双层循环
来源：http://ebz.jqgfzy.top

Ruby: nested.flatten
来源：http://gbt.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hrq.52xcode.cn

[D19] 按字段分组
来源：http://wnv.dashuyun.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dij.hysaishi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mtn.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mlf.svipenyu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ynx.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://suv.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://kqa.aibaodan.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eol.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rgv.smart0.xyz

[D20] 统计每个元素出现次数
来源：http://qky.ctjpmb.com

Py:   Counter(arr)
来源：http://uby.52xcode.cn

PHP:  array_count_values($arr);
来源：http://iwf.daxiang520.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vih.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eag.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://obt.hammf.cn

Go:   // 手写 map[T]int
来源：http://vuf.shangyingyoupin.top

Ruby: arr.tally
来源：http://lqk.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hmo.aizwys.cn

[D21] 判断是否包含某元素
来源：http://akz.fengsongda.top

Py:   x in arr
来源：http://llz.daria6918.cn

PHP:  in_array($x, $arr, true);
来源：http://fsc.guannengcc.top

JS:   arr.includes(x)
来源：http://uiq.yangfankeji.com

TS:   arr.includes(x)
来源：http://zni.chenzaomai.com

Java: list.contains(x)
来源：http://baf.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://cyy.guowangkeji.top

Ruby: arr.include?(x)
来源：http://sie.zycfv.cn

C#:   list.Contains(x)
来源：http://buu.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://yxk.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gcn.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dwk.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fqr.hammf.cn

TS:   [...arr];
来源：http://gsa.nwbrower.top

Java: new ArrayList<>(list);
来源：http://jsl.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://zwy.shanyushiyangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://mwv.gotoacloud.top

C#:   new List<int>(list);
来源：http://nzg.vehdjk.com

[D23] reduce 累积计算
来源：http://qux.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jit.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tpk.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uzh.tanke756.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gdj.xinyue.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://whk.hfpthk.cn

Go:   // 手写循环
来源：http://khg.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gap.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xdj.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://twa.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ubh.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rhe.gzhubu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nel.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sic.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hsp.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xvv.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zjx.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fjd.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://zhw.shangyingyoupin.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ztb.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sor.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mip.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xzp.cucudq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yld.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ubt.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wua.haohaochexian.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://srf.yangfankeji.com

[D26] 数组转字符串
来源：http://jgw.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://tja.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://mao.yanxiufei.cn

JS:   arr.join(", ")
来源：http://jsq.zdqjudy.top

TS:   arr.join(", ")
来源：http://uof.yongpay.top

Java: String.join(", ", list)
来源：http://qjo.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://ief.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://got.daria6918.cn

C#:   string.Join(", ", list)
来源：http://bqq.jlsjyb.cn

================================================================================
来源：http://rcx.daria6918.cn

E. 字符串处理
来源：http://ohp.shuidangran.top

================================================================================
来源：http://vmw.birdmap.top

[E01] 拼接字符串
来源：http://heb.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qvc.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ttw.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qsc.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vaa.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kti.daria6918.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aue.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wos.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://him.haohaochexian.top

[E02] 重复字符串
来源：http://xmf.chenjidiqi.icu

Py:   "ab" * 3
来源：http://khx.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://txp.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://rok.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://vux.yj20258.top

Java: "ab".repeat(3)
来源：http://nok.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://ejm.jinqigufen.top

Ruby: "ab" * 3
来源：http://pop.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lsn.haohaochexian.top

[E03] 截取子串
来源：http://jfl.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgy.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yfh.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jkb.nwbrower.top

TS:   s.slice(1, 4)
来源：http://hob.pycfn.com

Java: s.substring(1, 4)
来源：http://rsf.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jci.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://doo.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://bjl.smart0.xyz

[E04] 查找子串位置
来源：http://hqw.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://brx.shuidangran.top

PHP:  strpos($s, "x");
来源：http://ywz.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bsd.guannengcc.top

TS:   s.indexOf("x")
来源：http://vwo.9152youxi.cn

Java: s.indexOf("x")
来源：http://flz.aizwys.cn

Go:   strings.Index(s, "x")
来源：http://swc.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://xwz.mhx1999.top

C#:   s.IndexOf("x")
来源：http://wbe.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iiu.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ctm.jinqigufen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ehh.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mus.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://kjk.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjn.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iak.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dbb.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hmk.shanyushiyangkeji.top


<!-- 参考信息 -->