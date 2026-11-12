代发 wailian999

PHP:  // 无重载
来源：http://ldl.tianlin.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://bei.hnqzz.top

TS:   // 用联合类型或重载签名声明
来源：http://xeg.jinghuilouyu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kfx.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://afe.yuxming.cn

Ruby: # 无重载：靠动态参数
来源：http://umo.c1oappe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://vle.hysaishi.cn

================================================================================
来源：http://rdc.hesvh.cn

D. 数组 / 列表 / 集合
来源：http://cwd.nanxinkj.top

================================================================================
来源：http://prg.jianghu66.top

[D01] 创建数组 / 列表
来源：http://ypq.hnxiangtu.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://ukh.zhongyouzk.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hwe.daxiang520.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://myu.jqgufenzy.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://yqm.shuidangran.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rqx.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://rlx.zhixingplan.top

Ruby: arr = [1, 2, 3]
来源：http://gmp.hysaishi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ozs.yj202588.top

[D02] 追加元素到末尾
来源：http://bek.cucudq.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hxq.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lod.aibaodan.cn

JS:   arr.push(4);
来源：http://ton.chenlongwang.top

TS:   arr.push(4);
来源：http://pwq.dashuyun.cn

Java: list.add(4);
来源：http://wuj.yanxiufei.cn

Go:   arr = append(arr, 4)
来源：http://qqj.9152youxi.cn

Ruby: arr << 4; arr.push(5)
来源：http://owp.wangdashe.top

C#:   list.Add(4);
来源：http://ofz.tanke756.top

[D03] 在指定位置插入元素
来源：http://pkh.jinqigfzy.top

Py:   arr.insert(0, 0)
来源：http://kwf.haohaochexian.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xbj.xinyue.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mbn.tarul.cn

TS:   arr.splice(0, 0, 0);
来源：http://hul.jiagoushi.top

Java: list.add(0, 0);
来源：http://sqp.sufxvd.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wvn.shanyushiyangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kjs.hesvh.cn

C#:   list.Insert(0, 0);
来源：http://rhz.chenjidiqi.icu

[D04] 删除元素
来源：http://wmr.ehwqpu.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kms.andypj.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tvu.sweek.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dwr.tian-w.cn

TS:   arr.splice(0, 1);
来源：http://umq.hnqzz.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dtk.quarkkingdee.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oyz.52xcode.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ecu.dianchejie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://szv.jinghuilouyu.cn

[D05] 访问与修改元素
来源：http://eop.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://poj.yangfankeji.com

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wte.meibo888.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eek.yuanzhike.top

TS:   arr[0]; arr.at(-1);
来源：http://eba.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://slu.ppjwa.cn

Go:   arr[0]; arr[0] = 9
来源：http://qaf.hammf.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vje.jqgufenzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bma.cheryme.top

[D06] 数组长度
来源：http://znq.jinqigfzy.top

Py:   len(arr)
来源：http://wye.andypj.xyz

PHP:  count($arr);
来源：http://tne.gaohongyu789.top

JS:   arr.length
来源：http://ecw.hysaishi.cn

TS:   arr.length
来源：http://wii.daxiang520.top

Java: list.size();
来源：http://dai.ehwqpu.com

Go:   len(arr)
来源：http://cpd.jqgfzy.top

Ruby: arr.length; arr.size
来源：http://olx.0kj1m.cn

C#:   list.Count;
来源：http://fgn.sysykeji.top

[D07] 切片 / 取子数组
来源：http://lil.tanke756.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ssv.iojbl.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fer.yonumen.top

JS:   arr.slice(1, 4);
来源：http://rlb.fehbvm.com

TS:   arr.slice(1, 4);
来源：http://sxs.52xcode.cn

Java: list.subList(1, 4);
来源：http://rcf.iojbl.cn

Go:   arr[1:4]
来源：http://npk.shuidangran.top

Ruby: arr[1, 3]
来源：http://vcr.zhiwuduotai.top

C#:   list.GetRange(1, 3);
来源：http://zwi.shuidangran.top

[D08] 合并两个数组
来源：http://vwc.dashuyun.cn

Py:   a + b;  a.extend(b)
来源：http://oon.svipenyu.cn

PHP:  array_merge($a, $b);
来源：http://wlw.jlsjyb.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://eud.bjfxy.top

TS:   [...a, ...b];
来源：http://ngg.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kid.yuxming.cn

Go:   append(a, b...)
来源：http://sdp.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://wmn.ivvv.top

C#:   a.Concat(b).ToList()
来源：http://vig.hammf.cn

[D09] 排序（升序）
来源：http://cwc.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://eba.daria6918.cn

PHP:  sort($arr);
来源：http://qlv.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zfx.chenjidiqi.icu

TS:   [...arr].sort((x, y) => x - y);
来源：http://mxs.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://pqm.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fkx.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://flk.wangdashe.top

C#:   list.Sort();
来源：http://zez.iojbl.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gig.zhijiandao.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ahg.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rov.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mwe.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxs.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ofl.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bus.snrcjt.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://iak.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dfc.xinyue.icu

[D11] 反转数组
来源：http://mcp.shanyushiyangtech.top

Py:   arr[::-1];  arr.reverse()
来源：http://vmk.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://qpa.nanxuanxn.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rkc.sysykeji.top

TS:   [...arr].reverse();
来源：http://odx.xinyue.icu

Java: Collections.reverse(list);
来源：http://udv.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://yxp.chenzaomai.com

Ruby: arr.reverse
来源：http://vkp.xingfuxueyuan.xyz

C#:   list.Reverse();
来源：http://kzj.jinghuilouyu.cn

[D12] 查找元素下标
来源：http://ixm.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://mqm.0kj1m.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xun.yonumen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://slm.fengsongda.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycj.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xcx.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://oew.ehwqpu.com

Ruby: arr.index(x)
来源：http://ypr.hammf.cn

C#:   list.IndexOf(x);
来源：http://tlz.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://lvz.vehdjk.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wme.hesvh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://roq.pycfn.com

JS:   arr.filter(x => x > 3)
来源：http://vwx.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://htl.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ooz.mhx1999.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oiy.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://xys.gzhubu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://phu.meibo888.top

[D14] 映射转换（每个元素变形）
来源：http://dkf.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://add.ivvv.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xne.c1oappe.top

JS:   arr.map(x => x * 2)
来源：http://mpx.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://rat.ydjk.org.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mep.hnxiangtu.top

Go:   // 手写循环
来源：http://gdu.ehwqpu.com

Ruby: arr.map { |x| x * 2 }
来源：http://wck.shangyingyoupin.top

C#:   list.Select(x => x * 2).ToList()
来源：http://yiy.yangfankeji.com

[D15] 去重
来源：http://ssg.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dbk.guowangkeji.top

PHP:  array_unique($arr);
来源：http://taq.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://fpp.zycfv.cn

TS:   [...new Set(arr)]
来源：http://cpm.yangfankeji.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aob.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://tkl.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://lfa.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://rli.zdbjq.cn

[D16] 求和与平均值
来源：http://wpb.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iqn.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sld.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gol.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sxy.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tia.svipenyu.cn

Go:   // 手写循环累加
来源：http://phl.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qlc.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://abs.zhoulong.xyz

[D17] 最大值与最小值
来源：http://eqp.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://iut.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://hny.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gvl.c1oappe.top

TS:   Math.max(...arr);
来源：http://fje.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://syd.zdbjq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nfw.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://xgx.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://czz.zhoulong.xyz

[D18] 扁平化嵌套数组
来源：http://jdh.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ucc.hammf.cn

PHP:  array_merge(...$nested);
来源：http://xtm.jinqigfzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zjd.sysykeji.top

TS:   nested.flat();
来源：http://usp.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://byh.shanyushiyangtech.top

Go:   // 手写双层循环
来源：http://ytw.pycfn.com

Ruby: nested.flatten
来源：http://yna.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pgl.cucudq.cn

[D19] 按字段分组
来源：http://zio.yuxming.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vjk.tian-w.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nmi.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lgy.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ziq.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ebp.pycfn.com

Go:   // 手写 map[string][]T
来源：http://eug.fzhhl.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kfy.smart0.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cbk.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://uif.shuidangran.top

Py:   Counter(arr)
来源：http://lne.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://efa.epnwcf.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ill.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://umd.ehwqpu.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pbb.xylfe.cn

Go:   // 手写 map[T]int
来源：http://gww.yongpay.top

Ruby: arr.tally
来源：http://wot.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://heh.hesvh.cn

[D21] 判断是否包含某元素
来源：http://dqt.sjlbkw.cn

Py:   x in arr
来源：http://utp.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://ecn.nwbrower.top

JS:   arr.includes(x)
来源：http://nuv.hesvh.cn

TS:   arr.includes(x)
来源：http://lry.chenlongwang.top

Java: list.contains(x)
来源：http://frs.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://cmz.jiagoushi.top

Ruby: arr.include?(x)
来源：http://bsa.cashguo.top

C#:   list.Contains(x)
来源：http://gif.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://quo.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oqa.sxryk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zvb.xuetiantiany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://njr.ehwqpu.com

TS:   [...arr];
来源：http://fxq.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://waw.birdmap.top

Go:   copied := append([]int(nil), arr...)
来源：http://eta.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://ztp.andypj.xyz

C#:   new List<int>(list);
来源：http://xfl.iojbl.cn

[D23] reduce 累积计算
来源：http://did.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pcf.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tge.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xtn.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://voe.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ssr.sxryk.cn

Go:   // 手写循环
来源：http://pzp.yfazqb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wtk.andypj.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ide.iojbl.cn

[D24] 字典 / Map 基本操作
来源：http://ppe.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bzz.tian-w.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mbg.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zpw.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mbj.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ofc.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wlt.ehwqpu.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lsm.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://usu.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://vtd.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ewh.xinyue.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ogc.shzxlz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://umj.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vsb.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ymn.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tgd.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://whw.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://edt.jianghu66.top

[D26] 数组转字符串
来源：http://nts.quarkkingdee.top

Py:   ", ".join(map(str, arr))
来源：http://gyb.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://ikl.sufxvd.cn

JS:   arr.join(", ")
来源：http://mdf.tarul.cn

TS:   arr.join(", ")
来源：http://pww.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://vjs.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://ijl.daria6918.cn

Ruby: arr.join(", ")
来源：http://xck.wangdashe.top

C#:   string.Join(", ", list)
来源：http://pvf.yonumen.top

================================================================================
来源：http://cgn.yueranfly.top

E. 字符串处理
来源：http://ylk.yongpay.top

================================================================================
来源：http://cgl.cheryme.top

[E01] 拼接字符串
来源：http://ahj.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ian.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pvr.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hdz.gzhubu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yrq.gogol.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fqi.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tpu.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hth.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://far.chenlongwang.top

[E02] 重复字符串
来源：http://wgx.chenlongwang.top

Py:   "ab" * 3
来源：http://teq.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://pau.sysykeji.top

JS:   "ab".repeat(3)
来源：http://fkk.316326.xyz

TS:   "ab".repeat(3)
来源：http://shp.jqgfzy.top

Java: "ab".repeat(3)
来源：http://vgl.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://mjw.aizwys.cn

Ruby: "ab" * 3
来源：http://gei.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fpa.zhengqikj.top

[E03] 截取子串
来源：http://leh.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pis.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fgw.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mog.yj20258888.top

TS:   s.slice(1, 4)
来源：http://gob.jiagoushi.top

Java: s.substring(1, 4)
来源：http://qhv.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rnj.dianchejie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xgj.epnwcf.com

C#:   s.Substring(1, 3)
来源：http://apf.xziqi.cn

[E04] 查找子串位置
来源：http://ybi.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://hbb.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://zle.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://htq.xuanzx.com

TS:   s.indexOf("x")
来源：http://oih.sufxvd.cn

Java: s.indexOf("x")
来源：http://hak.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://ubf.guowangkeji.top

Ruby: s.index("x")
来源：http://wpr.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://xxw.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zxe.yongpay.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kiv.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bwu.tarul.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ccs.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zat.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ngm.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mmn.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tyu.haohaochexian.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hcb.yj20258.top

[E06] 替换子串
来源：http://lks.guannengcc.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lqj.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://prv.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pdt.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://zmn.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mvn.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbo.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tfk.ctjpmb.com


<!-- 参考信息 -->