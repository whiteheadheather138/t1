代发 wailian999

Ruby: a, b = pair
来源：http://bxl.jyoumei.cn

C#:   var (a, b) = pair;
来源：http://hwk.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://chd.gotoacloud.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ctp.zhixingplan.top

PHP:  // 无重载
来源：http://bid.xuetiantiany.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://buz.hnxiangtu.top

TS:   // 用联合类型或重载签名声明
来源：http://zfl.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gzs.sweek.top

Go:   // 无重载：用不同函数名
来源：http://bbh.zhixingplan.top

Ruby: # 无重载：靠动态参数
来源：http://ipn.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://wjz.yueranfly.top

================================================================================
来源：http://qgt.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://gab.yj202588.top

================================================================================
来源：http://nbh.xylfe.cn

[D01] 创建数组 / 列表
来源：http://otu.fengsongda.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cmp.sjlbkw.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uwl.yj20258.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://qjk.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://njo.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yzl.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://zqd.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://pgb.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lwb.shanyushiyangtech.top

[D02] 追加元素到末尾
来源：http://ywy.yfazqb.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://okg.ydzc1.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hpx.shangyingyoupin.top

JS:   arr.push(4);
来源：http://axb.jyoumei.cn

TS:   arr.push(4);
来源：http://htw.yj202588.top

Java: list.add(4);
来源：http://thp.sjlbkw.cn

Go:   arr = append(arr, 4)
来源：http://kdz.fengsongda.top

Ruby: arr << 4; arr.push(5)
来源：http://cfp.zhengqikj.top

C#:   list.Add(4);
来源：http://gxv.hysaishi.cn

[D03] 在指定位置插入元素
来源：http://leh.hfpthk.cn

Py:   arr.insert(0, 0)
来源：http://slc.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hrx.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ihy.sufxvd.cn

TS:   arr.splice(0, 0, 0);
来源：http://amm.sufxvd.cn

Java: list.add(0, 0);
来源：http://miy.316326.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://fmo.xuanzx.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bma.meibo888.top

C#:   list.Insert(0, 0);
来源：http://hcv.zhijiandao.cn

[D04] 删除元素
来源：http://prd.xinyue.icu

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://suc.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wjo.jqgufenzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dla.hcnkem.com

TS:   arr.splice(0, 1);
来源：http://hza.jqgufenzy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rgz.havefunace.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://dad.ctjpmb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zjp.ppjwa.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qja.pycfn.com

[D05] 访问与修改元素
来源：http://zuq.snrcjt.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jpy.yj20258888.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jgu.gzhubu.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vfw.vqdsnc.cn

TS:   arr[0]; arr.at(-1);
来源：http://ycy.smart0.xyz

Java: list.get(0); list.set(0, 9);
来源：http://hqc.jinqigfzy.top

Go:   arr[0]; arr[0] = 9
来源：http://zmx.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nhj.shangyingyoupin.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ozj.cqqwz.cn

[D06] 数组长度
来源：http://alg.redwolf501.top

Py:   len(arr)
来源：http://fjj.epnwcf.com

PHP:  count($arr);
来源：http://fnh.xziqi.cn

JS:   arr.length
来源：http://heq.xziqi.cn

TS:   arr.length
来源：http://nhq.xingfuxueyuan.xyz

Java: list.size();
来源：http://qgj.xinyue.icu

Go:   len(arr)
来源：http://tsg.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://bxm.nanxuanxn.top

C#:   list.Count;
来源：http://izl.nanxuanxn.top

[D07] 切片 / 取子数组
来源：http://dle.shzxlz.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xby.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xru.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://odb.snrcjt.cn

TS:   arr.slice(1, 4);
来源：http://gnp.hesvh.cn

Java: list.subList(1, 4);
来源：http://sks.jianghu66.top

Go:   arr[1:4]
来源：http://mhi.jyoumei.cn

Ruby: arr[1, 3]
来源：http://gaz.yfazqb.com

C#:   list.GetRange(1, 3);
来源：http://gzw.tarul.cn

[D08] 合并两个数组
来源：http://lgl.fehbvm.com

Py:   a + b;  a.extend(b)
来源：http://bym.quarkkingdee.top

PHP:  array_merge($a, $b);
来源：http://htf.zhiwuduotai.top

JS:   [...a, ...b];  a.concat(b);
来源：http://lua.ybcxt.top

TS:   [...a, ...b];
来源：http://rom.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pkz.jinyuanbaomall.cn

Go:   append(a, b...)
来源：http://fwv.hongshengwenyu.top

Ruby: a + b;  a.concat(b)
来源：http://uvk.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://guk.zhijiandao.cn

[D09] 排序（升序）
来源：http://vmt.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://kzo.quarkkingdee.top

PHP:  sort($arr);
来源：http://viq.hesvh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kam.fehbvm.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://ayq.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lsz.fzhhl.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nsk.hammf.cn

Ruby: arr.sort
来源：http://txw.vehdjk.com

C#:   list.Sort();
来源：http://qbw.cheryme.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fsl.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uwd.guannengcc.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ifd.zhoulong.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pui.shangyingyoupin.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rje.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gxc.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jov.jinghuilouyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://org.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wsl.mhx1999.top

[D11] 反转数组
来源：http://ydl.haohaochexian.top

Py:   arr[::-1];  arr.reverse()
来源：http://qux.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://wjm.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://syt.gotoacloud.top

TS:   [...arr].reverse();
来源：http://qca.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://egf.guannengcc.top

Go:   slices.Reverse(arr)
来源：http://gjz.shzxlz.cn

Ruby: arr.reverse
来源：http://fdh.iojbl.cn

C#:   list.Reverse();
来源：http://xaa.zycfv.cn

[D12] 查找元素下标
来源：http://lhm.dianchejie.cn

Py:   arr.index(x);  x in arr
来源：http://trm.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://umf.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ppm.ybcxt.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://coa.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cka.yuanzhike.top

Go:   slices.Index(arr, x)
来源：http://gki.smart0.xyz

Ruby: arr.index(x)
来源：http://xhq.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://bun.chenlongwang.top

[D13] 过滤（保留满足条件的）
来源：http://xnn.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tku.daria6918.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tvv.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://nqp.zhijiandao.cn

TS:   arr.filter(x => x > 3)
来源：http://vwy.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://spa.iojbl.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jas.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://tix.shanyushiyangtech.top

C#:   list.Where(x => x > 3).ToList()
来源：http://bnh.yuanzhike.top

[D14] 映射转换（每个元素变形）
来源：http://xtr.snrcjt.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cgk.nanxuanxn.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nec.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://wqf.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://txl.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xhk.tarul.cn

Go:   // 手写循环
来源：http://uxe.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rgc.hfpthk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zlo.xylfe.cn

[D15] 去重
来源：http://fgz.yfazqb.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fxy.yueranfly.top

PHP:  array_unique($arr);
来源：http://ntt.gotoacloud.top

JS:   [...new Set(arr)]
来源：http://veu.xziqi.cn

TS:   [...new Set(arr)]
来源：http://ocf.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gio.wangshuangyany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ocm.hesvh.cn

Ruby: arr.uniq
来源：http://uwj.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://uos.jqgfzy.top

[D16] 求和与平均值
来源：http://kll.hongshengwenyu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ipe.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://trm.ppjwa.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mem.andypj.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vcy.hnqzz.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eho.yueranfly.top

Go:   // 手写循环累加
来源：http://zgz.havefunace.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xgx.iojbl.cn

C#:   list.Sum();  list.Average()
来源：http://eyz.sufxvd.cn

[D17] 最大值与最小值
来源：http://ykm.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://tvl.feifeiyinyue.top

PHP:  max($arr);  min($arr);
来源：http://qmy.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ckt.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://ayr.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://btn.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://khs.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://xus.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://ukf.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://tar.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lmk.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://qbk.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wtt.zhongyouzk.top

TS:   nested.flat();
来源：http://lnn.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dyg.yvedp.cn

Go:   // 手写双层循环
来源：http://xfc.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://luc.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://tkk.uphjek.com

[D19] 按字段分组
来源：http://qta.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://thm.tarul.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bvf.tianlin.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cue.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rny.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ntc.feifeiyinyue.top

Go:   // 手写 map[string][]T
来源：http://jyq.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ioj.cheryme.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oan.guannengcc.top

[D20] 统计每个元素出现次数
来源：http://ier.wangshuangyany.cn

Py:   Counter(arr)
来源：http://bwn.mhx1999.top

PHP:  array_count_values($arr);
来源：http://hki.nanxuanxn.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wmt.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://air.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kle.jiagoushi.top

Go:   // 手写 map[T]int
来源：http://jyt.ehwqpu.com

Ruby: arr.tally
来源：http://afk.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hiv.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://hmt.hfpthk.cn

Py:   x in arr
来源：http://cjn.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://fzs.hnqzz.top

JS:   arr.includes(x)
来源：http://dyb.nwbrower.top

TS:   arr.includes(x)
来源：http://zbx.tarul.cn

Java: list.contains(x)
来源：http://jir.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://kqk.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://yog.gotoacloud.top

C#:   list.Contains(x)
来源：http://zeg.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://yvt.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xgd.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://idd.gotoacloud.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qdd.kuanghao11.cn

TS:   [...arr];
来源：http://oss.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://jpr.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kbz.jinqigufen.top

Ruby: arr.dup;  arr.clone
来源：http://zex.mhx1999.top

C#:   new List<int>(list);
来源：http://ayx.nanxinkj.top

[D23] reduce 累积计算
来源：http://ett.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gxn.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jmb.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dvt.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uje.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zwb.bbcook.cn

Go:   // 手写循环
来源：http://mgb.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://osj.zycfv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mfk.hesvh.cn

[D24] 字典 / Map 基本操作
来源：http://tqq.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bxi.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sid.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://urz.uphjek.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zca.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zls.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eei.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gtd.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fzz.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://qlw.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gnw.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iaf.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://epq.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://upb.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rlm.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kbd.zhaomingkeji.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ocx.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bra.hesvh.cn

[D26] 数组转字符串
来源：http://knt.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://zek.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://kro.jianghu66.top

JS:   arr.join(", ")
来源：http://zqh.havefunace.top

TS:   arr.join(", ")
来源：http://xam.ppjwa.cn

Java: String.join(", ", list)
来源：http://sam.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://hup.cucudq.cn

Ruby: arr.join(", ")
来源：http://gfa.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://nfv.52xcode.cn

================================================================================
来源：http://pup.ctjpmb.com

E. 字符串处理
来源：http://hxy.shzxlz.cn

================================================================================
来源：http://iwn.tianlin.xyz

[E01] 拼接字符串
来源：http://ugv.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jjt.xuanzx.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://whm.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xtl.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qti.tian-w.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ylj.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ize.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://esb.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bfc.wangshuangyany.cn

[E02] 重复字符串
来源：http://guw.sjlbkw.cn

Py:   "ab" * 3
来源：http://flb.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://cez.ybcxt.top

JS:   "ab".repeat(3)
来源：http://wqn.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://ndh.zdbjq.cn

Java: "ab".repeat(3)
来源：http://cgu.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://mbc.ybcxt.top

Ruby: "ab" * 3
来源：http://aom.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpc.jlsjyb.cn

[E03] 截取子串
来源：http://elf.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kid.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qos.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://crk.jianghu66.top

TS:   s.slice(1, 4)
来源：http://ckv.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://mun.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ywz.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rnm.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://xmz.bjfxy.top

[E04] 查找子串位置
来源：http://poy.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://vro.andypj.xyz

PHP:  strpos($s, "x");
来源：http://gvg.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qrk.wangshuangyany.cn

TS:   s.indexOf("x")
来源：http://elt.redwolf501.top

Java: s.indexOf("x")
来源：http://jmg.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://gcu.chenlongwang.top

Ruby: s.index("x")
来源：http://qcu.pycfn.com

C#:   s.IndexOf("x")
来源：http://mwc.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkh.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tnu.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cgg.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ltp.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lem.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvx.cdnleiting.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kle.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qjb.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xpp.vehdjk.com

[E06] 替换子串
来源：http://gde.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pej.dianchejie.cn

PHP:  str_replace("a", "b", $s);
来源：http://wnc.aizwys.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://plw.ppjwa.cn


<!-- 参考信息 -->