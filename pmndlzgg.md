代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rpb.ppjwa.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hqo.yj20258888.top

Java: // 无解构
来源：http://gbd.sxryk.cn

Go:   // 无解构
来源：http://pij.jyoumei.cn

Ruby: a, b = pair
来源：http://afq.yfazqb.com

C#:   var (a, b) = pair;
来源：http://ekn.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://jjv.aizwys.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lrw.jlsjyb.cn

PHP:  // 无重载
来源：http://tnq.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://eai.yj20258.top

TS:   // 用联合类型或重载签名声明
来源：http://iqu.cashguo.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jhr.tanke756.top

Go:   // 无重载：用不同函数名
来源：http://frp.cashguo.top

Ruby: # 无重载：靠动态参数
来源：http://vgl.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rha.sjlbkw.cn

================================================================================
来源：http://bvd.yangfankeji.com

D. 数组 / 列表 / 集合
来源：http://bqw.xingfuxueyuan.xyz

================================================================================
来源：http://qkr.shuidangran.top

[D01] 创建数组 / 列表
来源：http://iad.zycfv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://urb.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ckt.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wia.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://wxc.jyoumei.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xhg.fengsongda.top

Go:   arr := []int{1, 2, 3}
来源：http://vad.vqdsnc.cn

Ruby: arr = [1, 2, 3]
来源：http://hhc.yuxming.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mga.bjfxy.top

[D02] 追加元素到末尾
来源：http://hvd.chenlongwang.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lgz.zdbjq.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kvh.guowangkeji.top

JS:   arr.push(4);
来源：http://ida.sweek.top

TS:   arr.push(4);
来源：http://mun.fengsongda.top

Java: list.add(4);
来源：http://cyr.zdbjq.cn

Go:   arr = append(arr, 4)
来源：http://ylf.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://enn.mhx1999.top

C#:   list.Add(4);
来源：http://syp.hongshengwenyu.top

[D03] 在指定位置插入元素
来源：http://qsn.fzhhl.top

Py:   arr.insert(0, 0)
来源：http://dau.yuxming.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kgs.quarkkingdee.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jzw.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://cad.jyoumei.cn

Java: list.add(0, 0);
来源：http://yod.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://rgw.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zqf.cdnleiting.top

C#:   list.Insert(0, 0);
来源：http://ecd.ybcxt.top

[D04] 删除元素
来源：http://lgl.wangdashe.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xps.52xcode.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sdg.hfpthk.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mvc.jqgfzy.top

TS:   arr.splice(0, 1);
来源：http://ucu.vehdjk.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ztf.aibaodan.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pam.ydjk.org.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qpj.birdmap.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cqp.mhx1999.top

[D05] 访问与修改元素
来源：http://abi.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://paq.sufxvd.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yhj.pycfn.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://epe.svipenyu.cn

TS:   arr[0]; arr.at(-1);
来源：http://nfj.guowangkeji.top

Java: list.get(0); list.set(0, 9);
来源：http://toj.gotoacloud.top

Go:   arr[0]; arr[0] = 9
来源：http://wra.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rst.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pvd.xuanzx.com

[D06] 数组长度
来源：http://ktv.cucudq.cn

Py:   len(arr)
来源：http://owk.c1oappe.top

PHP:  count($arr);
来源：http://fzd.jinyuanbaomall.cn

JS:   arr.length
来源：http://jhd.shanyushiyangtech.top

TS:   arr.length
来源：http://rxh.hesvh.cn

Java: list.size();
来源：http://ktp.gzhubu.top

Go:   len(arr)
来源：http://zhh.quarkkingdee.top

Ruby: arr.length; arr.size
来源：http://wcv.snrcjt.cn

C#:   list.Count;
来源：http://wit.yj202588.top

[D07] 切片 / 取子数组
来源：http://mra.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://byd.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://yyy.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://rqk.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://dmx.316326.xyz

Java: list.subList(1, 4);
来源：http://xzz.uphjek.com

Go:   arr[1:4]
来源：http://wdi.cqqwz.cn

Ruby: arr[1, 3]
来源：http://ola.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://yft.guowangkeji.top

[D08] 合并两个数组
来源：http://nsi.sufxvd.cn

Py:   a + b;  a.extend(b)
来源：http://dvu.sweek.top

PHP:  array_merge($a, $b);
来源：http://qvf.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dvz.zdqjudy.top

TS:   [...a, ...b];
来源：http://wid.cashguo.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://trg.ybcxt.top

Go:   append(a, b...)
来源：http://qmx.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://ynh.uphjek.com

C#:   a.Concat(b).ToList()
来源：http://gnm.ehwqpu.com

[D09] 排序（升序）
来源：http://vwf.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://vyq.yuxming.cn

PHP:  sort($arr);
来源：http://kga.shanyushiyangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://azl.jianghu66.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hid.uphjek.com

Java: Collections.sort(list);  list.sort(null);
来源：http://zqb.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wnt.tanke756.top

Ruby: arr.sort
来源：http://arn.gzhubu.top

C#:   list.Sort();
来源：http://chj.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kpu.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bpj.ydjk.org.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rtu.jqgfzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://oly.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zsf.meibo888.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wna.nanxinkj.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://noh.ivvv.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kvx.jinghuilouyu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zex.shanyushiyangkeji.top

[D11] 反转数组
来源：http://kir.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://qzt.hysaishi.cn

PHP:  array_reverse($arr);
来源：http://tjw.daxiang520.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xgw.aibaodan.cn

TS:   [...arr].reverse();
来源：http://daf.hnqzz.top

Java: Collections.reverse(list);
来源：http://xhf.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://qll.chenlongwang.top

Ruby: arr.reverse
来源：http://uyt.daxiang520.top

C#:   list.Reverse();
来源：http://nlh.yvedp.cn

[D12] 查找元素下标
来源：http://yiw.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://mxv.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hrr.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nkf.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vfh.9152youxi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qxk.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://din.shuidangran.top

Ruby: arr.index(x)
来源：http://rrd.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://fvb.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://utn.c1oappe.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rsl.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wba.yanxiufei.cn

JS:   arr.filter(x => x > 3)
来源：http://tzy.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://mot.sweek.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://otp.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://brr.sjlbkw.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kzz.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://buv.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://cim.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mwl.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://git.iojbl.cn

JS:   arr.map(x => x * 2)
来源：http://wep.xuanzx.com

TS:   arr.map(x => x * 2)
来源：http://dac.jqgfzy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bpw.ydjk.org.cn

Go:   // 手写循环
来源：http://yxe.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://wvi.wangdashe.top

C#:   list.Select(x => x * 2).ToList()
来源：http://sgg.ydzc1.top

[D15] 去重
来源：http://snd.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wep.andypj.xyz

PHP:  array_unique($arr);
来源：http://vkp.sjlbkw.cn

JS:   [...new Set(arr)]
来源：http://ddx.hesvh.cn

TS:   [...new Set(arr)]
来源：http://efv.tian-w.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rxx.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://wdu.yfazqb.com

Ruby: arr.uniq
来源：http://dzb.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://pny.zhixingplan.top

[D16] 求和与平均值
来源：http://xii.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bya.hcnkem.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://onm.daria6918.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tgh.nwbrower.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cha.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ctf.fzhhl.top

Go:   // 手写循环累加
来源：http://jbm.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blv.xingfuxueyuan.xyz

C#:   list.Sum();  list.Average()
来源：http://qku.fktsv.cn

[D17] 最大值与最小值
来源：http://dol.cucudq.cn

Py:   max(arr);  min(arr)
来源：http://mhh.yonumen.top

PHP:  max($arr);  min($arr);
来源：http://nuy.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://azp.jyoumei.cn

TS:   Math.max(...arr);
来源：http://ams.fktsv.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tqi.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eci.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://guq.nanxinkj.top

C#:   list.Max();  list.Min()
来源：http://rni.fehbvm.com

[D18] 扁平化嵌套数组
来源：http://tvc.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jxz.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://pwj.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yhb.52xcode.cn

TS:   nested.flat();
来源：http://jiv.tian-w.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oit.wangdashe.top

Go:   // 手写双层循环
来源：http://opg.zdqjudy.top

Ruby: nested.flatten
来源：http://zih.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ech.fzhhl.top

[D19] 按字段分组
来源：http://bxx.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pcq.yj20258888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gxw.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cjd.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oaz.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pfu.tarul.cn

Go:   // 手写 map[string][]T
来源：http://mke.zhongyouzk.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gab.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wnd.nwbrower.top

[D20] 统计每个元素出现次数
来源：http://dqc.yanxiufei.cn

Py:   Counter(arr)
来源：http://lhp.gzhubu.top

PHP:  array_count_values($arr);
来源：http://lde.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bdw.xuetiantiany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gwy.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ryf.sysykeji.top

Go:   // 手写 map[T]int
来源：http://lal.fengsongda.top

Ruby: arr.tally
来源：http://gqy.hesvh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jcm.jqgufenzy.top

[D21] 判断是否包含某元素
来源：http://fig.cdnleiting.top

Py:   x in arr
来源：http://pra.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://yvn.zhixingplan.top

JS:   arr.includes(x)
来源：http://ekq.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://ebt.jinqigfzy.top

Java: list.contains(x)
来源：http://mdb.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://qiz.epnwcf.com

Ruby: arr.include?(x)
来源：http://hty.dianchejie.cn

C#:   list.Contains(x)
来源：http://xft.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://pij.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uui.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://frv.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://add.smart0.xyz

TS:   [...arr];
来源：http://kfk.pengpengdd.cyou

Java: new ArrayList<>(list);
来源：http://sxt.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lld.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://bps.hnqzz.top

C#:   new List<int>(list);
来源：http://ras.c1oappe.top

[D23] reduce 累积计算
来源：http://hzj.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wom.shuidangran.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://izt.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zxb.yuxming.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://snp.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nop.iojbl.cn

Go:   // 手写循环
来源：http://izw.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qyo.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pyj.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://hki.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zxo.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jrl.guannengcc.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ijb.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cuk.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fmp.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://egs.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ttc.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aae.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://bzy.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ulx.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uwa.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fur.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://szd.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bvn.guannengcc.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://len.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ghv.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://skp.9152youxi.cn

[D26] 数组转字符串
来源：http://zzs.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://xho.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://rqr.daria6918.cn

JS:   arr.join(", ")
来源：http://euk.ivvv.top

TS:   arr.join(", ")
来源：http://tte.sysykeji.top

Java: String.join(", ", list)
来源：http://cmm.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://mxk.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://qiw.yj20258888.top

C#:   string.Join(", ", list)
来源：http://ter.cdnleiting.top

================================================================================
来源：http://tdz.cqqwz.cn

E. 字符串处理
来源：http://htx.vqdsnc.cn

================================================================================
来源：http://tou.yuxming.cn

[E01] 拼接字符串
来源：http://qut.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kpj.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://udo.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://usk.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://biw.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hmr.shzxlz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kqx.yj20258888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zir.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nok.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://qtv.nanxinkj.top

Py:   "ab" * 3
来源：http://qkl.yangfankeji.com

PHP:  str_repeat("ab", 3);
来源：http://sgl.shuidangran.top

JS:   "ab".repeat(3)
来源：http://frb.tian-w.cn

TS:   "ab".repeat(3)
来源：http://dwm.ehwqpu.com

Java: "ab".repeat(3)
来源：http://snn.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://kuh.pycfn.com

Ruby: "ab" * 3
来源：http://bfd.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rch.tarul.cn

[E03] 截取子串
来源：http://hgo.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jyh.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rbl.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wqd.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://vqa.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://zet.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ojo.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://ecm.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://uqk.c1oappe.top

[E04] 查找子串位置
来源：http://cqo.ppjwa.cn

Py:   s.find("x");  s.index("x")
来源：http://gag.jqgfzy.top

PHP:  strpos($s, "x");
来源：http://ser.fzhhl.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oxh.yangfankeji.com

TS:   s.indexOf("x")
来源：http://ouq.sufxvd.cn

Java: s.indexOf("x")
来源：http://sqg.ivvv.top

Go:   strings.Index(s, "x")
来源：http://yeg.sysykeji.top

Ruby: s.index("x")
来源：http://ylr.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://hez.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ltj.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hdn.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ucq.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yfd.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://biz.sjlbkw.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upm.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cyu.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ohy.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://laj.zhaomingkeji.xyz


<!-- 参考信息 -->