代发 wailian999

PHP:  // 无重载
来源：http://uoy.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://trk.jlsjyb.cn

TS:   // 用联合类型或重载签名声明
来源：http://poz.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jsw.jinqigfzy.top

Go:   // 无重载：用不同函数名
来源：http://ymx.ppjwa.cn

Ruby: # 无重载：靠动态参数
来源：http://wqg.xylfe.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hvc.pycfn.com

================================================================================
来源：http://rsw.hnxiangtu.top

D. 数组 / 列表 / 集合
来源：http://okc.jinghuilouyu.cn

================================================================================
来源：http://wfw.zdbjq.cn

[D01] 创建数组 / 列表
来源：http://emp.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xib.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://alu.bjfxy.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://cpy.tanke756.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ora.kuanghao11.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oaw.zhaomingkeji.xyz

Go:   arr := []int{1, 2, 3}
来源：http://pnx.tian-w.cn

Ruby: arr = [1, 2, 3]
来源：http://mxi.ydjk.org.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://umo.shzxlz.cn

[D02] 追加元素到末尾
来源：http://fmq.ppjwa.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pob.ctjpmb.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wbh.zhijiandao.cn

JS:   arr.push(4);
来源：http://hdn.snrcjt.cn

TS:   arr.push(4);
来源：http://tjo.ivvv.top

Java: list.add(4);
来源：http://aby.fehbvm.com

Go:   arr = append(arr, 4)
来源：http://rsi.zhixingplan.top

Ruby: arr << 4; arr.push(5)
来源：http://xfh.zhijiandao.cn

C#:   list.Add(4);
来源：http://abk.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://pab.hysaishi.cn

Py:   arr.insert(0, 0)
来源：http://aqg.aizwys.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tob.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bhk.chenjidiqi.icu

TS:   arr.splice(0, 0, 0);
来源：http://rbe.jinyuanbaomall.cn

Java: list.add(0, 0);
来源：http://qsp.xziqi.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nji.shangyingyoupin.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fwr.zhengqikj.top

C#:   list.Insert(0, 0);
来源：http://eug.meibo888.top

[D04] 删除元素
来源：http://ztk.chenlongwang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ipm.haohaochexian.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nzk.hongshengwenyu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zyg.jinyuanbaomall.cn

TS:   arr.splice(0, 1);
来源：http://noh.dianchejie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ert.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://aij.kuanghao11.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://anf.ydzc1.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://olu.hnxiangtu.top

[D05] 访问与修改元素
来源：http://ttb.daxiang520.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://pbz.wangdashe.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rhl.316326.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dht.ydzc1.top

TS:   arr[0]; arr.at(-1);
来源：http://qbp.shuidangran.top

Java: list.get(0); list.set(0, 9);
来源：http://thw.smart0.xyz

Go:   arr[0]; arr[0] = 9
来源：http://aof.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sdy.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://aca.ybcxt.top

[D06] 数组长度
来源：http://gmf.zdqjudy.top

Py:   len(arr)
来源：http://jbm.sysykeji.top

PHP:  count($arr);
来源：http://bht.yj202588.top

JS:   arr.length
来源：http://unr.uphjek.com

TS:   arr.length
来源：http://bip.aizwys.cn

Java: list.size();
来源：http://web.gotoacloud.top

Go:   len(arr)
来源：http://dyx.epnwcf.com

Ruby: arr.length; arr.size
来源：http://gcu.chenzaomai.com

C#:   list.Count;
来源：http://atk.vqdsnc.cn

[D07] 切片 / 取子数组
来源：http://jtb.xuanzx.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://njy.nwbrower.top

PHP:  array_slice($arr, 1, 3);
来源：http://nca.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://oco.jiagoushi.top

TS:   arr.slice(1, 4);
来源：http://hqi.zdqjudy.top

Java: list.subList(1, 4);
来源：http://toh.sysykeji.top

Go:   arr[1:4]
来源：http://ycb.zhijiandao.cn

Ruby: arr[1, 3]
来源：http://fht.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://qgb.hysaishi.cn

[D08] 合并两个数组
来源：http://ian.hywenlv.cn

Py:   a + b;  a.extend(b)
来源：http://tsn.yangfankeji.com

PHP:  array_merge($a, $b);
来源：http://wgn.yfazqb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://phz.daria6918.cn

TS:   [...a, ...b];
来源：http://mqw.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tef.zhixingplan.top

Go:   append(a, b...)
来源：http://wnf.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://gqa.havefunace.top

C#:   a.Concat(b).ToList()
来源：http://ehp.jinqigufen.top

[D09] 排序（升序）
来源：http://ryd.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://tyf.xziqi.cn

PHP:  sort($arr);
来源：http://qrg.haohaochexian.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yea.meibo888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qer.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oet.sysykeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bji.bjfxy.top

Ruby: arr.sort
来源：http://hyg.316326.xyz

C#:   list.Sort();
来源：http://uxz.zhaomingkeji.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://zmz.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fnl.xuanzx.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fts.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kjh.yongpay.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lsl.52xcode.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uzx.epnwcf.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://knd.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ixn.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pzl.hnxiangtu.top

[D11] 反转数组
来源：http://aee.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vvh.hesvh.cn

PHP:  array_reverse($arr);
来源：http://cec.jiagoushi.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bhr.yangfankeji.com

TS:   [...arr].reverse();
来源：http://tkj.nanxinkj.top

Java: Collections.reverse(list);
来源：http://jxd.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://sdv.gogol.net.cn

Ruby: arr.reverse
来源：http://ahs.zhongyouzk.top

C#:   list.Reverse();
来源：http://jim.birdmap.top

[D12] 查找元素下标
来源：http://yfd.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://seu.epnwcf.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cpl.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://anh.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lcj.chenjidiqi.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tid.gaohongyu789.top

Go:   slices.Index(arr, x)
来源：http://qse.pycfn.com

Ruby: arr.index(x)
来源：http://ycy.iojbl.cn

C#:   list.IndexOf(x);
来源：http://prh.shzxlz.cn

[D13] 过滤（保留满足条件的）
来源：http://ntx.yonumen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wuo.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kxl.c1oappe.top

JS:   arr.filter(x => x > 3)
来源：http://kug.cqqwz.cn

TS:   arr.filter(x => x > 3)
来源：http://sen.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ufe.tian-w.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yvs.kuanghao11.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yvh.nanxuanxn.top

C#:   list.Where(x => x > 3).ToList()
来源：http://rzg.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://egt.bbcook.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vbf.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rmg.yuanzhike.top

JS:   arr.map(x => x * 2)
来源：http://xgb.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://hdq.yj20258888.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bnl.c1oappe.top

Go:   // 手写循环
来源：http://bjq.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://auz.dashuyun.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jss.quarkkingdee.top

[D15] 去重
来源：http://lam.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mwd.cucudq.cn

PHP:  array_unique($arr);
来源：http://jbx.xylfe.cn

JS:   [...new Set(arr)]
来源：http://ffn.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://dqd.yj20258888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hxs.dianchejie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uco.jianghu66.top

Ruby: arr.uniq
来源：http://aqw.hnxiangtu.top

C#:   list.Distinct().ToList()
来源：http://cup.ydzc1.top

[D16] 求和与平均值
来源：http://tsb.zhijiandao.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xqn.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mmq.hesvh.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vgp.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ukf.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xwi.0kj1m.cn

Go:   // 手写循环累加
来源：http://trm.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ysv.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://gzr.cheryme.top

[D17] 最大值与最小值
来源：http://eoq.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://rpw.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://jcq.zycfv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dla.hammf.cn

TS:   Math.max(...arr);
来源：http://sde.chenzaomai.com

Java: Collections.max(list);  Collections.min(list);
来源：http://feh.chenzaomai.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yrs.iojbl.cn

Ruby: arr.max;  arr.min
来源：http://wkn.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://shn.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://hre.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bjs.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://ulx.snrcjt.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vme.zhixingplan.top

TS:   nested.flat();
来源：http://oan.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lxv.ehwqpu.com

Go:   // 手写双层循环
来源：http://nwa.yj202588.top

Ruby: nested.flatten
来源：http://tnv.sjlbkw.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dsf.xylfe.cn

[D19] 按字段分组
来源：http://hzn.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rem.0kj1m.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://owl.yangfankeji.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://olc.zycfv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vdk.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://myv.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://lfg.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mhu.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rio.sxryk.cn

[D20] 统计每个元素出现次数
来源：http://tfz.jinqigfzy.top

Py:   Counter(arr)
来源：http://hfc.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://eas.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vli.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qrk.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yxw.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://izc.meibo888.top

Ruby: arr.tally
来源：http://cmg.svipenyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vuf.zycfv.cn

[D21] 判断是否包含某元素
来源：http://hqj.sjlbkw.cn

Py:   x in arr
来源：http://lqf.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://iss.nwbrower.top

JS:   arr.includes(x)
来源：http://htz.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://wmt.havefunace.top

Java: list.contains(x)
来源：http://gjh.hammf.cn

Go:   slices.Contains(arr, x)
来源：http://sqi.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://tud.ehwqpu.com

C#:   list.Contains(x)
来源：http://uvx.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://mus.feifeiyinyue.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yve.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dzf.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mef.yj20258888.top

TS:   [...arr];
来源：http://vco.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://dah.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://fcj.yuxming.cn

Ruby: arr.dup;  arr.clone
来源：http://qvc.yj20258.top

C#:   new List<int>(list);
来源：http://lbq.vehdjk.com

[D23] reduce 累积计算
来源：http://yzc.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ked.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rwb.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oll.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hfi.zhijiandao.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://usa.jinqigufen.top

Go:   // 手写循环
来源：http://xki.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qjk.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ayq.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://lxa.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ioy.ctjpmb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yfk.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hzs.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jzv.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ftd.wangshuangyany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jsn.aizwys.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rca.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qeb.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://quq.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zqm.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rdo.cdnleiting.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ssz.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbm.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dsa.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vje.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iza.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xsh.sysykeji.top

[D26] 数组转字符串
来源：http://thc.gogol.net.cn

Py:   ", ".join(map(str, arr))
来源：http://thh.jqgfzy.top

PHP:  implode(", ", $arr);
来源：http://zpd.9152youxi.cn

JS:   arr.join(", ")
来源：http://ygi.bjfxy.top

TS:   arr.join(", ")
来源：http://usu.bbcook.cn

Java: String.join(", ", list)
来源：http://lrs.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://wyh.ctjpmb.com

Ruby: arr.join(", ")
来源：http://jfd.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://mbh.chenjidiqi.icu

================================================================================
来源：http://ako.zhoulong.xyz

E. 字符串处理
来源：http://dsd.c1oappe.top

================================================================================
来源：http://nwo.zdbjq.cn

[E01] 拼接字符串
来源：http://rmx.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ora.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qtx.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dvk.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtj.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://afu.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qys.gotoacloud.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vth.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gwu.yueranfly.top

[E02] 重复字符串
来源：http://osa.aizwys.cn

Py:   "ab" * 3
来源：http://wtj.nwbrower.top

PHP:  str_repeat("ab", 3);
来源：http://dtu.yueranfly.top

JS:   "ab".repeat(3)
来源：http://rke.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://krm.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://vix.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://owm.zdbjq.cn

Ruby: "ab" * 3
来源：http://jvl.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dxx.andypj.xyz

[E03] 截取子串
来源：http://gho.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xfw.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ahw.wangdashe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hvs.yuanzhike.top

TS:   s.slice(1, 4)
来源：http://gqb.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://alj.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kwb.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dvr.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://bcw.zhengqikj.top

[E04] 查找子串位置
来源：http://gxk.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://efo.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://vnr.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pgp.wangdashe.top

TS:   s.indexOf("x")
来源：http://fiy.jqgufenzy.top

Java: s.indexOf("x")
来源：http://vwn.birdmap.top

Go:   strings.Index(s, "x")
来源：http://hxb.nwbrower.top

Ruby: s.index("x")
来源：http://ilt.daria6918.cn

C#:   s.IndexOf("x")
来源：http://ldi.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wkp.xingfuxueyuan.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cxp.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xbi.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zsb.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jgd.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ixr.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cws.fktsv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://feg.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hvc.jyoumei.cn

[E06] 替换子串
来源：http://egk.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lne.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://xmr.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://teg.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://cew.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sdo.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xqh.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ykf.havefunace.top


<!-- 参考信息 -->