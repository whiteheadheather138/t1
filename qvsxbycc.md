代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tpz.meibo888.top

[C15] 解构 / 展开参数
来源：http://uqg.bjfxy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yeg.aibaodan.cn

PHP:  [$a, $b] = $pair;
来源：http://pme.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lmz.yj20258888.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qju.sxryk.cn

Java: // 无解构
来源：http://ekr.uphjek.com

Go:   // 无解构
来源：http://pxd.jyoumei.cn

Ruby: a, b = pair
来源：http://wah.wangshuangyany.cn

C#:   var (a, b) = pair;
来源：http://enf.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://wag.cqqwz.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fqe.fehbvm.com

PHP:  // 无重载
来源：http://bup.ydzc1.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://wci.zhijiandao.cn

TS:   // 用联合类型或重载签名声明
来源：http://tnw.yj202588.top

Java: void f(int a) {}  void f(String a) {}
来源：http://gae.feifeiyinyue.top

Go:   // 无重载：用不同函数名
来源：http://hqb.fktsv.cn

Ruby: # 无重载：靠动态参数
来源：http://eyw.tarul.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xwz.zhixingplan.top

================================================================================
来源：http://ubp.cqqwz.cn

D. 数组 / 列表 / 集合
来源：http://lgf.wangdashe.top

================================================================================
来源：http://plk.sysykeji.top

[D01] 创建数组 / 列表
来源：http://ysh.zdbjq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qgh.ydzc1.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aku.haohaochexian.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://peg.vehdjk.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://ese.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://fcv.jinqigfzy.top

Go:   arr := []int{1, 2, 3}
来源：http://vky.jiagoushi.top

Ruby: arr = [1, 2, 3]
来源：http://fze.cashguo.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://iyp.tianlin.xyz

[D02] 追加元素到末尾
来源：http://wyw.52xcode.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://huq.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sia.yanxiufei.cn

JS:   arr.push(4);
来源：http://yec.0kj1m.cn

TS:   arr.push(4);
来源：http://oyi.wangdashe.top

Java: list.add(4);
来源：http://dyp.pengpengdd.cyou

Go:   arr = append(arr, 4)
来源：http://eoy.havefunace.top

Ruby: arr << 4; arr.push(5)
来源：http://ajn.redwolf501.top

C#:   list.Add(4);
来源：http://xoa.zdbjq.cn

[D03] 在指定位置插入元素
来源：http://bjb.gaohongyu789.top

Py:   arr.insert(0, 0)
来源：http://mmf.jinyuanbaomall.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://unu.zhongyouzk.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://szz.52xcode.cn

TS:   arr.splice(0, 0, 0);
来源：http://roi.zdbjq.cn

Java: list.add(0, 0);
来源：http://qrm.ivvv.top

Go:   arr = append([]int{0}, arr...)
来源：http://qwx.hnqzz.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mps.feifeiyinyue.top

C#:   list.Insert(0, 0);
来源：http://ait.zhiwuduotai.top

[D04] 删除元素
来源：http://hxv.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wun.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uvq.tian-w.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mxw.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://ghn.gotoacloud.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vvf.tarul.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://itm.zdbjq.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://vho.jinqigufen.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ooc.0kj1m.cn

[D05] 访问与修改元素
来源：http://ijt.jqgfzy.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://meb.shangyingyoupin.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://enz.0kj1m.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ego.fengsongda.top

TS:   arr[0]; arr.at(-1);
来源：http://cnv.svipenyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://nqt.jqgfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://xxg.fengsongda.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://inu.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://clz.zhongyouzk.top

[D06] 数组长度
来源：http://gun.hfpthk.cn

Py:   len(arr)
来源：http://tdo.sjlbkw.cn

PHP:  count($arr);
来源：http://wwd.jlsjyb.cn

JS:   arr.length
来源：http://hvu.bbcook.cn

TS:   arr.length
来源：http://wak.0kj1m.cn

Java: list.size();
来源：http://zfx.epnwcf.com

Go:   len(arr)
来源：http://hze.hnxiangtu.top

Ruby: arr.length; arr.size
来源：http://brz.feifeiyinyue.top

C#:   list.Count;
来源：http://vmp.pengpengdd.cyou

[D07] 切片 / 取子数组
来源：http://cto.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://abp.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://syq.shzxlz.cn

JS:   arr.slice(1, 4);
来源：http://xbp.haohaochexian.top

TS:   arr.slice(1, 4);
来源：http://mdq.shangyingyoupin.top

Java: list.subList(1, 4);
来源：http://vlc.hfpthk.cn

Go:   arr[1:4]
来源：http://fwe.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://tdu.tian-w.cn

C#:   list.GetRange(1, 3);
来源：http://eeh.meibo888.top

[D08] 合并两个数组
来源：http://zmh.snrcjt.cn

Py:   a + b;  a.extend(b)
来源：http://pkl.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://hnk.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://tjq.gogol.net.cn

TS:   [...a, ...b];
来源：http://mgp.jqgufenzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tyv.daria6918.cn

Go:   append(a, b...)
来源：http://fhc.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://kbg.smart0.xyz

C#:   a.Concat(b).ToList()
来源：http://pjq.nanxuanxn.top

[D09] 排序（升序）
来源：http://tbo.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://sxk.jianghu66.top

PHP:  sort($arr);
来源：http://new.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://flq.hongshengwenyu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://cdx.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mrt.ydjk.org.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oju.yuxming.cn

Ruby: arr.sort
来源：http://mnb.pycfn.com

C#:   list.Sort();
来源：http://yxq.yvedp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rsp.jqgfzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nwn.fanxiaobao.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://njn.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://myl.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qkh.zdbjq.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cxl.jqgfzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pgu.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qdv.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mof.zycfv.cn

[D11] 反转数组
来源：http://cik.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://uzp.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://dlg.aizwys.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zbr.daria6918.cn

TS:   [...arr].reverse();
来源：http://ovp.yj202588.top

Java: Collections.reverse(list);
来源：http://vmm.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://jws.xylfe.cn

Ruby: arr.reverse
来源：http://xrk.chenzaomai.com

C#:   list.Reverse();
来源：http://spg.yangfankeji.com

[D12] 查找元素下标
来源：http://uii.aizwys.cn

Py:   arr.index(x);  x in arr
来源：http://ccs.hcnkem.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zdu.xuetiantiany.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qbf.bbcook.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmk.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gpc.gzhubu.top

Go:   slices.Index(arr, x)
来源：http://lzb.epnwcf.com

Ruby: arr.index(x)
来源：http://vbp.xziqi.cn

C#:   list.IndexOf(x);
来源：http://ere.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://ouz.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gtv.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://khs.quarkkingdee.top

JS:   arr.filter(x => x > 3)
来源：http://yqk.vehdjk.com

TS:   arr.filter(x => x > 3)
来源：http://ujl.ehwqpu.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gjw.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ulf.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://fns.jyoumei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zvg.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://qlt.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://smv.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://znf.chenlongwang.top

JS:   arr.map(x => x * 2)
来源：http://wwc.jyoumei.cn

TS:   arr.map(x => x * 2)
来源：http://nww.epnwcf.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://khz.smart0.xyz

Go:   // 手写循环
来源：http://wul.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bwk.vqdsnc.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iam.fengsongda.top

[D15] 去重
来源：http://skc.meibo888.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cta.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://pwl.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://iuw.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://ykt.yuanzhike.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://guu.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ilg.9152youxi.cn

Ruby: arr.uniq
来源：http://qoh.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://uiu.hfpthk.cn

[D16] 求和与平均值
来源：http://kyb.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://axc.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uby.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://inp.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://asn.zhiwuduotai.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mim.havefunace.top

Go:   // 手写循环累加
来源：http://ooz.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wpl.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://srk.hcnkem.com

[D17] 最大值与最小值
来源：http://uhy.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://dnr.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://yvh.snrcjt.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kmv.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://tkd.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lyq.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ktg.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://wqv.316326.xyz

C#:   list.Max();  list.Min()
来源：http://evc.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://stp.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hlv.tian-w.cn

PHP:  array_merge(...$nested);
来源：http://zqw.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sax.cdnleiting.top

TS:   nested.flat();
来源：http://efx.yongpay.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xmr.gotoacloud.top

Go:   // 手写双层循环
来源：http://vcm.fengsongda.top

Ruby: nested.flatten
来源：http://fmi.epnwcf.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://hlt.haohaochexian.top

[D19] 按字段分组
来源：http://wgx.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wie.xylfe.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://woz.hcnkem.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vcp.hnqzz.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://loq.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lqz.daria6918.cn

Go:   // 手写 map[string][]T
来源：http://rpi.ehwqpu.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://yff.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mmn.shuidangran.top

[D20] 统计每个元素出现次数
来源：http://gfj.gaohongyu789.top

Py:   Counter(arr)
来源：http://ggv.aibaodan.cn

PHP:  array_count_values($arr);
来源：http://tse.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ifv.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ylj.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lwl.havefunace.top

Go:   // 手写 map[T]int
来源：http://cjo.epnwcf.com

Ruby: arr.tally
来源：http://grm.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jcg.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://gyl.sxryk.cn

Py:   x in arr
来源：http://lsr.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://jmp.kuanghao11.cn

JS:   arr.includes(x)
来源：http://piz.snrcjt.cn

TS:   arr.includes(x)
来源：http://gck.zhoulong.xyz

Java: list.contains(x)
来源：http://src.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://kkf.zhixingplan.top

Ruby: arr.include?(x)
来源：http://vql.ydzc1.top

C#:   list.Contains(x)
来源：http://vsp.zhengqikj.top

[D22] 复制数组（避免共享引用）
来源：http://isi.0kj1m.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nuo.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nnt.zhaomingkeji.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jom.yvedp.cn

TS:   [...arr];
来源：http://zfx.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://jwx.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gwb.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://ezu.yj202588.top

C#:   new List<int>(list);
来源：http://zbk.gotoacloud.top

[D23] reduce 累积计算
来源：http://cta.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://haj.snrcjt.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://myj.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aas.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ahz.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hyy.vqdsnc.cn

Go:   // 手写循环
来源：http://ydr.yj20258.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xtr.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ynm.316326.xyz

[D24] 字典 / Map 基本操作
来源：http://dyw.yj20258888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://itq.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mua.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fjk.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rkr.tanke756.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ibx.ywan-chungtsiang.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jyu.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zgk.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qvh.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://ewo.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://arb.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tjf.yanxiufei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ioq.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vdg.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://typ.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://syt.dianchejie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uyc.meibo888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dzr.epnwcf.com

[D26] 数组转字符串
来源：http://yno.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://pvv.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://nyq.haohaochexian.top

JS:   arr.join(", ")
来源：http://dgt.yongpay.top

TS:   arr.join(", ")
来源：http://tas.yuxming.cn

Java: String.join(", ", list)
来源：http://lje.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://xgj.guowangkeji.top

Ruby: arr.join(", ")
来源：http://rfg.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://ufo.yuanzhike.top

================================================================================
来源：http://wau.zhijiandao.cn

E. 字符串处理
来源：http://sft.birdmap.top

================================================================================
来源：http://qei.daxiang520.top

[E01] 拼接字符串
来源：http://pbx.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ozb.zhijiandao.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dna.shanyushiyangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aur.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ofz.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yhm.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lyh.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gfw.c1oappe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ica.yongpay.top

[E02] 重复字符串
来源：http://iwt.feifeiyinyue.top

Py:   "ab" * 3
来源：http://rbm.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://nme.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://isd.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://jtc.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://wcw.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://vmu.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://utp.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aic.hysaishi.cn

[E03] 截取子串
来源：http://fnp.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bzw.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qpx.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xwp.uphjek.com

TS:   s.slice(1, 4)
来源：http://laz.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://vgf.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ghj.smart0.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://iel.tianlin.xyz

C#:   s.Substring(1, 3)
来源：http://hos.kuanghao11.cn

[E04] 查找子串位置
来源：http://ssq.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://zys.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://idr.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vfd.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://tpq.jianghu66.top

Java: s.indexOf("x")
来源：http://dgt.sweek.top

Go:   strings.Index(s, "x")
来源：http://gmk.jqgufenzy.top

Ruby: s.index("x")
来源：http://jbv.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://jzi.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yih.snrcjt.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qmu.daxiang520.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mra.jyoumei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bww.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zem.hongshengwenyu.top


<!-- 参考信息 -->