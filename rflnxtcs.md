代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ulo.ydjk.org.cn

[C15] 解构 / 展开参数
来源：http://ycx.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fyg.fktsv.cn

PHP:  [$a, $b] = $pair;
来源：http://hey.epnwcf.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gfs.zycfv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bzf.mhx1999.top

Java: // 无解构
来源：http://anr.zhoulong.xyz

Go:   // 无解构
来源：http://oyb.hongshengwenyu.top

Ruby: a, b = pair
来源：http://wwz.ehwqpu.com

C#:   var (a, b) = pair;
来源：http://lyh.yfazqb.com

[C16] 函数 / 方法重载
来源：http://bya.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yun.fktsv.cn

PHP:  // 无重载
来源：http://hrr.yangfankeji.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://gvm.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://wyb.ppjwa.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xoj.hywenlv.cn

Go:   // 无重载：用不同函数名
来源：http://kuk.hnxiangtu.top

Ruby: # 无重载：靠动态参数
来源：http://uhp.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nuv.hongshengwenyu.top

================================================================================
来源：http://dgz.shzxlz.cn

D. 数组 / 列表 / 集合
来源：http://ddx.ivvv.top

================================================================================
来源：http://lbu.52xcode.cn

[D01] 创建数组 / 列表
来源：http://spv.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://wyt.fanxiaobao.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uff.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://plh.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://twi.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yxy.9152youxi.cn

Go:   arr := []int{1, 2, 3}
来源：http://nks.jinqigfzy.top

Ruby: arr = [1, 2, 3]
来源：http://pjh.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://jxw.svipenyu.cn

[D02] 追加元素到末尾
来源：http://pau.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xex.ybcxt.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qju.vehdjk.com

JS:   arr.push(4);
来源：http://rjv.cheryme.top

TS:   arr.push(4);
来源：http://hch.uphjek.com

Java: list.add(4);
来源：http://vhf.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://gpx.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://mxi.jlsjyb.cn

C#:   list.Add(4);
来源：http://ubx.snrcjt.cn

[D03] 在指定位置插入元素
来源：http://zsv.zdbjq.cn

Py:   arr.insert(0, 0)
来源：http://can.uphjek.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mwt.shangyingyoupin.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bba.guowangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://zqw.fanxiaobao.xyz

Java: list.add(0, 0);
来源：http://noz.haohaochexian.top

Go:   arr = append([]int{0}, arr...)
来源：http://iuo.shzxlz.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://glf.zhaomingkeji.xyz

C#:   list.Insert(0, 0);
来源：http://eii.zdqjudy.top

[D04] 删除元素
来源：http://cat.shuidangran.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xwo.yanxiufei.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jjz.vqdsnc.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://unb.xingfuxueyuan.xyz

TS:   arr.splice(0, 1);
来源：http://shk.yanxiufei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://psa.dashuyun.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ghl.fktsv.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://esw.svipenyu.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vaj.havefunace.top

[D05] 访问与修改元素
来源：http://enp.hesvh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jxu.tianlin.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://zxt.wangshuangyany.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cyq.fanxiaobao.xyz

TS:   arr[0]; arr.at(-1);
来源：http://lrt.zhixingplan.top

Java: list.get(0); list.set(0, 9);
来源：http://yte.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://wwi.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://auf.pengpengdd.cyou

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://faj.cucudq.cn

[D06] 数组长度
来源：http://qtb.gzhubu.top

Py:   len(arr)
来源：http://ceu.tanke756.top

PHP:  count($arr);
来源：http://bsd.fehbvm.com

JS:   arr.length
来源：http://fcd.ctjpmb.com

TS:   arr.length
来源：http://qvb.jiagoushi.top

Java: list.size();
来源：http://upi.52xcode.cn

Go:   len(arr)
来源：http://fvf.aibaodan.cn

Ruby: arr.length; arr.size
来源：http://avi.uphjek.com

C#:   list.Count;
来源：http://rcf.sweek.top

[D07] 切片 / 取子数组
来源：http://wgk.zhixingplan.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zcp.mhx1999.top

PHP:  array_slice($arr, 1, 3);
来源：http://vsn.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://zgq.mhx1999.top

TS:   arr.slice(1, 4);
来源：http://bdy.gaohongyu789.top

Java: list.subList(1, 4);
来源：http://nou.gotoacloud.top

Go:   arr[1:4]
来源：http://roa.hesvh.cn

Ruby: arr[1, 3]
来源：http://nla.zhoulong.xyz

C#:   list.GetRange(1, 3);
来源：http://csz.yangfankeji.com

[D08] 合并两个数组
来源：http://fbr.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://duc.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://cjz.ydzc1.top

JS:   [...a, ...b];  a.concat(b);
来源：http://tob.jinqigfzy.top

TS:   [...a, ...b];
来源：http://gzm.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mdm.jinghuilouyu.cn

Go:   append(a, b...)
来源：http://kad.sxryk.cn

Ruby: a + b;  a.concat(b)
来源：http://jil.bbcook.cn

C#:   a.Concat(b).ToList()
来源：http://yri.ydjk.org.cn

[D09] 排序（升序）
来源：http://kwp.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://mch.andypj.xyz

PHP:  sort($arr);
来源：http://cca.zhijiandao.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tlg.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bmf.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://knp.xylfe.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://utm.yongpay.top

Ruby: arr.sort
来源：http://idk.shanyushiyangkeji.top

C#:   list.Sort();
来源：http://khf.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://blg.jianghu66.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iee.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rkx.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pkk.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://djo.sjlbkw.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ocw.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://adw.nanxuanxn.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zbw.zhaomingkeji.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gff.fengsongda.top

[D11] 反转数组
来源：http://kor.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gqi.quarkkingdee.top

PHP:  array_reverse($arr);
来源：http://myp.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wlb.cdnleiting.top

TS:   [...arr].reverse();
来源：http://ohi.xziqi.cn

Java: Collections.reverse(list);
来源：http://hac.hongshengwenyu.top

Go:   slices.Reverse(arr)
来源：http://gfx.0kj1m.cn

Ruby: arr.reverse
来源：http://rlv.hesvh.cn

C#:   list.Reverse();
来源：http://iui.zhoulong.xyz

[D12] 查找元素下标
来源：http://vun.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://pkb.fzhhl.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://enp.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ruz.aibaodan.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wys.xuetiantiany.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uls.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://hzp.iojbl.cn

Ruby: arr.index(x)
来源：http://lkk.yueranfly.top

C#:   list.IndexOf(x);
来源：http://qaj.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://qwz.iojbl.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vjx.shanyushiyangtech.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ywr.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://vld.guowangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://jwi.dianchejie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zxp.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nah.ivvv.top

Ruby: arr.select { |x| x > 3 }
来源：http://iqx.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sfy.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://iig.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rac.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sza.xinyue.icu

JS:   arr.map(x => x * 2)
来源：http://fxz.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://yro.yanxiufei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rjj.xziqi.cn

Go:   // 手写循环
来源：http://nqb.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qnb.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wrf.quarkkingdee.top

[D15] 去重
来源：http://bgx.dashuyun.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cdo.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://eor.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://jxe.zhaomingkeji.xyz

TS:   [...new Set(arr)]
来源：http://aiq.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uty.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://iod.c1oappe.top

Ruby: arr.uniq
来源：http://ips.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://fmb.jinqigufen.top

[D16] 求和与平均值
来源：http://keh.yj202588.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pbw.jinghuilouyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bbj.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pse.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wgg.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ztf.fktsv.cn

Go:   // 手写循环累加
来源：http://ued.xylfe.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gfa.yueranfly.top

C#:   list.Sum();  list.Average()
来源：http://qkq.meibo888.top

[D17] 最大值与最小值
来源：http://eum.cashguo.top

Py:   max(arr);  min(arr)
来源：http://hdf.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://pbb.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vrz.andypj.xyz

TS:   Math.max(...arr);
来源：http://muw.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rqm.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ibd.cashguo.top

Ruby: arr.max;  arr.min
来源：http://ylf.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://rkq.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://tzy.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://voi.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://dzt.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uwm.cheryme.top

TS:   nested.flat();
来源：http://xwt.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ysb.yonumen.top

Go:   // 手写双层循环
来源：http://pgu.meibo888.top

Ruby: nested.flatten
来源：http://opc.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://spa.nanxinkj.top

[D19] 按字段分组
来源：http://xfz.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mcn.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://maa.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pcl.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://myy.pycfn.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dfn.316326.xyz

Go:   // 手写 map[string][]T
来源：http://dcd.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tqq.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://loh.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://wkx.redwolf501.top

Py:   Counter(arr)
来源：http://jzg.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://keg.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kec.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://euj.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hwv.tian-w.cn

Go:   // 手写 map[T]int
来源：http://crd.yuanzhike.top

Ruby: arr.tally
来源：http://rvw.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sla.pycfn.com

[D21] 判断是否包含某元素
来源：http://zaq.xuanzx.com

Py:   x in arr
来源：http://lyl.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://qbe.havefunace.top

JS:   arr.includes(x)
来源：http://nmj.hcnkem.com

TS:   arr.includes(x)
来源：http://ugd.snrcjt.cn

Java: list.contains(x)
来源：http://ugn.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://xmm.gzhubu.top

Ruby: arr.include?(x)
来源：http://oqy.havefunace.top

C#:   list.Contains(x)
来源：http://dwu.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://zio.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gyj.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ynr.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lny.yfazqb.com

TS:   [...arr];
来源：http://nqe.yj20258.top

Java: new ArrayList<>(list);
来源：http://zbb.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fpt.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://zdv.vehdjk.com

C#:   new List<int>(list);
来源：http://znv.wangdashe.top

[D23] reduce 累积计算
来源：http://bwd.gzhubu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xtl.xziqi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ssz.jinqigufen.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mvf.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rsr.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kdb.vehdjk.com

Go:   // 手写循环
来源：http://oal.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mqv.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bpp.birdmap.top

[D24] 字典 / Map 基本操作
来源：http://yej.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gnx.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xng.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rlq.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://obs.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://psb.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xoq.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bjs.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vkg.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://ptk.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xpa.gaohongyu789.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dib.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iqt.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lwa.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bwk.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wcf.yj20258.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rhy.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iga.c1oappe.top

[D26] 数组转字符串
来源：http://mgm.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://dle.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://uws.aibaodan.cn

JS:   arr.join(", ")
来源：http://rby.yj202588.top

TS:   arr.join(", ")
来源：http://stz.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://jon.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://xgt.tanke756.top

Ruby: arr.join(", ")
来源：http://pfr.jinyuanbaomall.cn

C#:   string.Join(", ", list)
来源：http://rug.tarul.cn

================================================================================
来源：http://tnc.havefunace.top

E. 字符串处理
来源：http://bxd.dashuyun.cn

================================================================================
来源：http://zet.chenjidiqi.icu

[E01] 拼接字符串
来源：http://dcj.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ojn.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lqu.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jlr.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://djf.iojbl.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pin.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://scj.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dax.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dgw.mhx1999.top

[E02] 重复字符串
来源：http://hzk.pycfn.com

Py:   "ab" * 3
来源：http://gdk.0kj1m.cn

PHP:  str_repeat("ab", 3);
来源：http://pnb.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://xsx.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://rax.gotoacloud.top

Java: "ab".repeat(3)
来源：http://afd.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://exd.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://sle.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ddr.sysykeji.top

[E03] 截取子串
来源：http://gdr.jinqigufen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://try.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bga.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rma.gzhubu.top

TS:   s.slice(1, 4)
来源：http://dar.ctjpmb.com

Java: s.substring(1, 4)
来源：http://dqo.ivvv.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fzv.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://qtf.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://cgt.quarkkingdee.top

[E04] 查找子串位置
来源：http://hxc.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://esv.fzhhl.top

PHP:  strpos($s, "x");
来源：http://ijs.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rob.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://meo.zdqjudy.top

Java: s.indexOf("x")
来源：http://qjh.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://njm.meibo888.top

Ruby: s.index("x")
来源：http://rrw.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://wle.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nfw.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://krk.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dts.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iao.kuanghao11.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oan.kuanghao11.cn


<!-- 参考信息 -->