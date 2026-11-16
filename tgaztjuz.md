代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ofa.xuanzx.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zmu.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bnd.ehwqpu.com

Ruby: # 无泛型
来源：http://npr.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yph.jianghu66.top

[C15] 解构 / 展开参数
来源：http://lyi.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ayb.ctjpmb.com

PHP:  [$a, $b] = $pair;
来源：http://wcd.jinqigufen.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://iyy.chenzaomai.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://not.jyoumei.cn

Java: // 无解构
来源：http://hsc.dianchejie.cn

Go:   // 无解构
来源：http://gvd.jyoumei.cn

Ruby: a, b = pair
来源：http://lim.hysaishi.cn

C#:   var (a, b) = pair;
来源：http://zru.shuidangran.top

[C16] 函数 / 方法重载
来源：http://qqa.tanke756.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://enn.wangdashe.top

PHP:  // 无重载
来源：http://hbl.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://miz.jyoumei.cn

TS:   // 用联合类型或重载签名声明
来源：http://sjc.316326.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://bie.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://dwi.hywenlv.cn

Ruby: # 无重载：靠动态参数
来源：http://gkd.zdqjudy.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://izj.yfazqb.com

================================================================================
来源：http://lto.sxryk.cn

D. 数组 / 列表 / 集合
来源：http://cuf.xuanzx.com

================================================================================
来源：http://nvj.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://szi.vqdsnc.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://brn.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jmv.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zuq.shanyushiyangtech.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oiz.xinyue.icu

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kpl.quarkkingdee.top

Go:   arr := []int{1, 2, 3}
来源：http://xyd.xuetiantiany.cn

Ruby: arr = [1, 2, 3]
来源：http://fom.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ike.sufxvd.cn

[D02] 追加元素到末尾
来源：http://svj.cashguo.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://znb.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mrn.hammf.cn

JS:   arr.push(4);
来源：http://ulo.hammf.cn

TS:   arr.push(4);
来源：http://vvm.birdmap.top

Java: list.add(4);
来源：http://ugx.yj20258888.top

Go:   arr = append(arr, 4)
来源：http://urx.tarul.cn

Ruby: arr << 4; arr.push(5)
来源：http://cmj.guowangkeji.top

C#:   list.Add(4);
来源：http://dok.xylfe.cn

[D03] 在指定位置插入元素
来源：http://zkt.wangdashe.top

Py:   arr.insert(0, 0)
来源：http://bsw.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://swk.xuanzx.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yal.quarkkingdee.top

TS:   arr.splice(0, 0, 0);
来源：http://mwb.yongpay.top

Java: list.add(0, 0);
来源：http://pwc.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ell.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lyy.dianchejie.cn

C#:   list.Insert(0, 0);
来源：http://hgj.hcnkem.com

[D04] 删除元素
来源：http://psa.zhaomingkeji.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://okx.shanyushiyangtech.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://was.shuidangran.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nnt.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://xsa.cashguo.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kwp.zdqjudy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mmb.nwbrower.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gxw.mhx1999.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mfi.yj20258.top

[D05] 访问与修改元素
来源：http://bvb.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blw.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kzm.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ujh.jinyuanbaomall.cn

TS:   arr[0]; arr.at(-1);
来源：http://lvi.9152youxi.cn

Java: list.get(0); list.set(0, 9);
来源：http://kdk.mhx1999.top

Go:   arr[0]; arr[0] = 9
来源：http://tvc.gzhubu.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bjm.nwbrower.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gzj.chenjidiqi.icu

[D06] 数组长度
来源：http://wfa.jinqigfzy.top

Py:   len(arr)
来源：http://fro.cdnleiting.top

PHP:  count($arr);
来源：http://svc.zhaomingkeji.xyz

JS:   arr.length
来源：http://gby.zdbjq.cn

TS:   arr.length
来源：http://hex.dashuyun.cn

Java: list.size();
来源：http://uwl.cashguo.top

Go:   len(arr)
来源：http://ksc.zhoulong.xyz

Ruby: arr.length; arr.size
来源：http://eig.haohaochexian.top

C#:   list.Count;
来源：http://koc.yueranfly.top

[D07] 切片 / 取子数组
来源：http://aou.xingfuxueyuan.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://opc.vqdsnc.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xmc.hfpthk.cn

JS:   arr.slice(1, 4);
来源：http://sem.52xcode.cn

TS:   arr.slice(1, 4);
来源：http://enj.vehdjk.com

Java: list.subList(1, 4);
来源：http://tgd.xingfuxueyuan.xyz

Go:   arr[1:4]
来源：http://rtj.aizwys.cn

Ruby: arr[1, 3]
来源：http://saw.gotoacloud.top

C#:   list.GetRange(1, 3);
来源：http://gqj.aizwys.cn

[D08] 合并两个数组
来源：http://wxj.jinqigfzy.top

Py:   a + b;  a.extend(b)
来源：http://duf.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://wtd.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://hqz.52xcode.cn

TS:   [...a, ...b];
来源：http://lqq.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tjn.yfazqb.com

Go:   append(a, b...)
来源：http://lzu.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://bey.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://wer.ywan-chungtsiang.top

[D09] 排序（升序）
来源：http://onn.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://ezi.jinqigfzy.top

PHP:  sort($arr);
来源：http://ryd.jlsjyb.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rjq.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://apl.hysaishi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dvl.uphjek.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cmd.zdqjudy.top

Ruby: arr.sort
来源：http://mkh.yangfankeji.com

C#:   list.Sort();
来源：http://cij.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sgn.hysaishi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xyd.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rdi.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nry.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mna.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dxh.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hyh.epnwcf.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eht.yj20258.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://npv.vqdsnc.cn

[D11] 反转数组
来源：http://nwd.xinyue.icu

Py:   arr[::-1];  arr.reverse()
来源：http://hrj.ywan-chungtsiang.top

PHP:  array_reverse($arr);
来源：http://ovn.hnxiangtu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ifa.sysykeji.top

TS:   [...arr].reverse();
来源：http://kek.vehdjk.com

Java: Collections.reverse(list);
来源：http://pul.cheryme.top

Go:   slices.Reverse(arr)
来源：http://iuk.yj20258888.top

Ruby: arr.reverse
来源：http://doa.xuanzx.com

C#:   list.Reverse();
来源：http://xhj.birdmap.top

[D12] 查找元素下标
来源：http://fsl.ehwqpu.com

Py:   arr.index(x);  x in arr
来源：http://cml.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nmn.ydzc1.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://izd.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gma.yuanzhike.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://old.jyoumei.cn

Go:   slices.Index(arr, x)
来源：http://rrk.yuxming.cn

Ruby: arr.index(x)
来源：http://jjc.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://fax.nanxinkj.top

[D13] 过滤（保留满足条件的）
来源：http://vab.tanke756.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qhv.hysaishi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://amz.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://uur.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://lfl.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://paa.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jmp.dianchejie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dtl.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bib.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://brk.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://yho.bbcook.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zjf.zhijiandao.cn

JS:   arr.map(x => x * 2)
来源：http://bfk.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://nlh.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yls.sysykeji.top

Go:   // 手写循环
来源：http://wlg.ybcxt.top

Ruby: arr.map { |x| x * 2 }
来源：http://cns.daria6918.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qrv.zhongyouzk.top

[D15] 去重
来源：http://qdb.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fuf.aibaodan.cn

PHP:  array_unique($arr);
来源：http://kbc.yanxiufei.cn

JS:   [...new Set(arr)]
来源：http://rhw.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://cae.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dqk.52xcode.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tbk.sxryk.cn

Ruby: arr.uniq
来源：http://awv.tian-w.cn

C#:   list.Distinct().ToList()
来源：http://jzb.uphjek.com

[D16] 求和与平均值
来源：http://fdl.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pca.ehwqpu.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pxj.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://byt.yvedp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hai.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oge.jianghu66.top

Go:   // 手写循环累加
来源：http://qou.9152youxi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gsz.dashuyun.cn

C#:   list.Sum();  list.Average()
来源：http://nho.sysykeji.top

[D17] 最大值与最小值
来源：http://jim.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://qxf.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://tbn.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cbi.havefunace.top

TS:   Math.max(...arr);
来源：http://kfb.zycfv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ghu.ydjk.org.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tqd.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://ttf.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://lej.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://xgv.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uhe.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://kgl.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yov.jqgfzy.top

TS:   nested.flat();
来源：http://hly.316326.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://adi.52xcode.cn

Go:   // 手写双层循环
来源：http://izg.jinqigfzy.top

Ruby: nested.flatten
来源：http://zye.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dud.xziqi.cn

[D19] 按字段分组
来源：http://wry.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hkw.c1oappe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ysi.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bzd.fktsv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wje.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hyo.wangshuangyany.cn

Go:   // 手写 map[string][]T
来源：http://www.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wpq.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bfy.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://odu.hesvh.cn

Py:   Counter(arr)
来源：http://abc.yonumen.top

PHP:  array_count_values($arr);
来源：http://ije.hcnkem.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vwn.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fym.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xgj.birdmap.top

Go:   // 手写 map[T]int
来源：http://rou.gaohongyu789.top

Ruby: arr.tally
来源：http://fef.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ymt.kuanghao11.cn

[D21] 判断是否包含某元素
来源：http://rmy.aizwys.cn

Py:   x in arr
来源：http://mkr.nwbrower.top

PHP:  in_array($x, $arr, true);
来源：http://pux.316326.xyz

JS:   arr.includes(x)
来源：http://vhr.gzhubu.top

TS:   arr.includes(x)
来源：http://dxx.9152youxi.cn

Java: list.contains(x)
来源：http://xzm.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://lwk.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://wic.bjfxy.top

C#:   list.Contains(x)
来源：http://why.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://gmc.smart0.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wvh.sufxvd.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kzb.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vag.andypj.xyz

TS:   [...arr];
来源：http://yvd.bbcook.cn

Java: new ArrayList<>(list);
来源：http://dug.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://egl.meibo888.top

Ruby: arr.dup;  arr.clone
来源：http://iny.c1oappe.top

C#:   new List<int>(list);
来源：http://wjy.aizwys.cn

[D23] reduce 累积计算
来源：http://lpn.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qmi.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wne.yanxiufei.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ycc.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqq.cucudq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vgg.dashuyun.cn

Go:   // 手写循环
来源：http://cuf.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bru.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jhp.sweek.top

[D24] 字典 / Map 基本操作
来源：http://vto.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rub.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jha.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://krk.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tin.yangfankeji.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://egc.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hwr.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qrh.ydjk.org.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://isu.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://xhc.jianghu66.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://khn.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gop.sweek.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tkx.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gax.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://civ.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ydy.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nvi.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yvw.xuetiantiany.cn

[D26] 数组转字符串
来源：http://zgz.epnwcf.com

Py:   ", ".join(map(str, arr))
来源：http://ejj.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://xxb.xziqi.cn

JS:   arr.join(", ")
来源：http://pwu.yvedp.cn

TS:   arr.join(", ")
来源：http://zuq.epnwcf.com

Java: String.join(", ", list)
来源：http://bfr.jlsjyb.cn

Go:   strings.Join(strs, ", ")
来源：http://qeu.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://auu.cucudq.cn

C#:   string.Join(", ", list)
来源：http://eqq.jinqigufen.top

================================================================================
来源：http://fnu.cqqwz.cn

E. 字符串处理
来源：http://feg.hesvh.cn

================================================================================
来源：http://pln.zhongyouzk.top

[E01] 拼接字符串
来源：http://rvq.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xgc.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qtt.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cjn.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sjx.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mhb.ywan-chungtsiang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eze.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qum.feifeiyinyue.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://raa.gogol.net.cn

[E02] 重复字符串
来源：http://diz.jyoumei.cn

Py:   "ab" * 3
来源：http://okv.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://hos.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://jqa.ydzc1.top

TS:   "ab".repeat(3)
来源：http://oxd.ivvv.top

Java: "ab".repeat(3)
来源：http://gmt.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://zzq.yanxiufei.cn

Ruby: "ab" * 3
来源：http://dmm.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xjs.pengpengdd.cyou

[E03] 截取子串
来源：http://wjw.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gyv.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eox.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://otu.cdnleiting.top

TS:   s.slice(1, 4)
来源：http://dup.bbcook.cn

Java: s.substring(1, 4)
来源：http://vtl.nwbrower.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jzv.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://fkj.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://nbr.yanxiufei.cn

[E04] 查找子串位置
来源：http://frt.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://vji.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://ngl.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hwr.yvedp.cn

TS:   s.indexOf("x")
来源：http://dqh.dashuyun.cn

Java: s.indexOf("x")
来源：http://sld.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://uup.xziqi.cn

Ruby: s.index("x")
来源：http://jlc.redwolf501.top

C#:   s.IndexOf("x")
来源：http://lyh.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nzo.shanyushiyangkeji.top


<!-- 参考信息 -->