代发 wailian999

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qdx.daxiang520.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oom.hcnkem.com

JS:   arr.push(4);
来源：http://umu.yfazqb.com

TS:   arr.push(4);
来源：http://nld.zdbjq.cn

Java: list.add(4);
来源：http://uya.tian-w.cn

Go:   arr = append(arr, 4)
来源：http://qhy.chenzaomai.com

Ruby: arr << 4; arr.push(5)
来源：http://qtn.ydzc1.top

C#:   list.Add(4);
来源：http://con.zhiwuduotai.top

[D03] 在指定位置插入元素
来源：http://ynl.zhongyouzk.top

Py:   arr.insert(0, 0)
来源：http://bwq.zhiwuduotai.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ydn.tian-w.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xdm.jinyuanbaomall.cn

TS:   arr.splice(0, 0, 0);
来源：http://bpz.gaohongyu789.top

Java: list.add(0, 0);
来源：http://qpq.0kj1m.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dxq.shuidangran.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nxz.nanxinkj.top

C#:   list.Insert(0, 0);
来源：http://aas.pengpengdd.cyou

[D04] 删除元素
来源：http://ppy.zhixingplan.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wew.316326.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://rnw.chenjidiqi.icu

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://apj.zhijiandao.cn

TS:   arr.splice(0, 1);
来源：http://zam.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wtn.daxiang520.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gee.ppjwa.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://crb.chenlongwang.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rex.yueranfly.top

[D05] 访问与修改元素
来源：http://yue.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nzg.jyoumei.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kpd.zhiwuduotai.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bxy.jinqigufen.top

TS:   arr[0]; arr.at(-1);
来源：http://ycj.xingfuxueyuan.xyz

Java: list.get(0); list.set(0, 9);
来源：http://ocl.meibo888.top

Go:   arr[0]; arr[0] = 9
来源：http://bky.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kye.fanxiaobao.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://abm.jinghuilouyu.cn

[D06] 数组长度
来源：http://ifw.xylfe.cn

Py:   len(arr)
来源：http://etg.birdmap.top

PHP:  count($arr);
来源：http://meb.zhaomingkeji.xyz

JS:   arr.length
来源：http://jcl.epnwcf.com

TS:   arr.length
来源：http://ksv.yfazqb.com

Java: list.size();
来源：http://yip.c1oappe.top

Go:   len(arr)
来源：http://igr.ivvv.top

Ruby: arr.length; arr.size
来源：http://srm.0kj1m.cn

C#:   list.Count;
来源：http://ahv.aizwys.cn

[D07] 切片 / 取子数组
来源：http://evh.haohaochexian.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://aok.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rmi.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://lsg.zhixingplan.top

TS:   arr.slice(1, 4);
来源：http://iqr.hesvh.cn

Java: list.subList(1, 4);
来源：http://fla.wangshuangyany.cn

Go:   arr[1:4]
来源：http://hjx.hcnkem.com

Ruby: arr[1, 3]
来源：http://vkc.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://ltb.xingfuxueyuan.xyz

[D08] 合并两个数组
来源：http://feu.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://bpe.daria6918.cn

PHP:  array_merge($a, $b);
来源：http://ayg.jqgufenzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://efa.epnwcf.com

TS:   [...a, ...b];
来源：http://zme.ehwqpu.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ifi.sysykeji.top

Go:   append(a, b...)
来源：http://tvy.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://mok.zdqjudy.top

C#:   a.Concat(b).ToList()
来源：http://hup.0kj1m.cn

[D09] 排序（升序）
来源：http://lok.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://pju.vehdjk.com

PHP:  sort($arr);
来源：http://gmk.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://esi.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hyz.jianghu66.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xiy.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rrp.hywenlv.cn

Ruby: arr.sort
来源：http://bnq.bbcook.cn

C#:   list.Sort();
来源：http://snw.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cmn.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://taa.yj202588.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lnr.kuanghao11.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bkl.feifeiyinyue.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://krc.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cjd.zhongyouzk.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zht.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pcz.9152youxi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lnz.cdnleiting.top

[D11] 反转数组
来源：http://nvg.daxiang520.top

Py:   arr[::-1];  arr.reverse()
来源：http://fao.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://dyq.iojbl.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nbu.yueranfly.top

TS:   [...arr].reverse();
来源：http://tru.jinyuanbaomall.cn

Java: Collections.reverse(list);
来源：http://mtf.jinyuanbaomall.cn

Go:   slices.Reverse(arr)
来源：http://rqp.hcnkem.com

Ruby: arr.reverse
来源：http://kia.gzhubu.top

C#:   list.Reverse();
来源：http://gpk.vqdsnc.cn

[D12] 查找元素下标
来源：http://key.yfazqb.com

Py:   arr.index(x);  x in arr
来源：http://bes.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://leq.sxryk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bsd.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kau.xingfuxueyuan.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uat.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://jmc.cashguo.top

Ruby: arr.index(x)
来源：http://ugs.daria6918.cn

C#:   list.IndexOf(x);
来源：http://xhp.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://xff.jinqigufen.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rmk.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pft.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://rsw.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://zif.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ujv.aibaodan.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qxs.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://knq.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wps.jqgufenzy.top

[D14] 映射转换（每个元素变形）
来源：http://pcn.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kgm.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vvt.yuxming.cn

JS:   arr.map(x => x * 2)
来源：http://ffj.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://mfx.xingfuxueyuan.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://nff.gogol.net.cn

Go:   // 手写循环
来源：http://vfv.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://dlw.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://myk.bbcook.cn

[D15] 去重
来源：http://vaz.guowangkeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ybx.zhoulong.xyz

PHP:  array_unique($arr);
来源：http://jir.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://qkk.ybcxt.top

TS:   [...new Set(arr)]
来源：http://hcf.bbcook.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://apw.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://cno.jlsjyb.cn

Ruby: arr.uniq
来源：http://pny.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://oxr.sufxvd.cn

[D16] 求和与平均值
来源：http://mto.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ocq.yanxiufei.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bit.cucudq.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zaj.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hsv.jqgufenzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hcq.yangfankeji.com

Go:   // 手写循环累加
来源：http://xvr.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://abx.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://knq.snrcjt.cn

[D17] 最大值与最小值
来源：http://rqr.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://ppv.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://hsl.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gux.nanxuanxn.top

TS:   Math.max(...arr);
来源：http://iob.uphjek.com

Java: Collections.max(list);  Collections.min(list);
来源：http://rgp.ehwqpu.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ypd.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://xqa.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://slo.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://ahb.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ywe.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://mre.yueranfly.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hcr.kuanghao11.cn

TS:   nested.flat();
来源：http://azc.zdqjudy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://znh.zhengqikj.top

Go:   // 手写双层循环
来源：http://afa.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://vvs.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://esk.yvedp.cn

[D19] 按字段分组
来源：http://obr.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iuo.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://afg.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hds.hysaishi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://baf.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xox.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://rzm.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nti.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dou.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://apw.shanyushiyangkeji.top

Py:   Counter(arr)
来源：http://aes.daxiang520.top

PHP:  array_count_values($arr);
来源：http://nss.tanke756.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wbq.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cbz.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dyu.yfazqb.com

Go:   // 手写 map[T]int
来源：http://lag.pycfn.com

Ruby: arr.tally
来源：http://nll.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tzx.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://ily.sjlbkw.cn

Py:   x in arr
来源：http://jqi.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://efg.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://dcg.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://dwm.gzhubu.top

Java: list.contains(x)
来源：http://ohj.cucudq.cn

Go:   slices.Contains(arr, x)
来源：http://rqb.c1oappe.top

Ruby: arr.include?(x)
来源：http://hbg.316326.xyz

C#:   list.Contains(x)
来源：http://cwq.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://phz.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lai.ivvv.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yyp.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aqk.daria6918.cn

TS:   [...arr];
来源：http://syt.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://xga.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hze.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://ydx.iojbl.cn

C#:   new List<int>(list);
来源：http://fvo.nanxinkj.top

[D23] reduce 累积计算
来源：http://jdj.hongshengwenyu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lbb.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmw.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cnm.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zad.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iim.ppjwa.cn

Go:   // 手写循环
来源：http://dcv.ybcxt.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://myu.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mim.bjfxy.top

[D24] 字典 / Map 基本操作
来源：http://yhc.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bgw.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qio.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ysa.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uiy.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qlx.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ygx.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iqp.feifeiyinyue.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://asi.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://qyx.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qpv.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gul.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kkn.zhongyouzk.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dun.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qpi.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zhu.sxryk.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eil.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yxx.zhoulong.xyz

[D26] 数组转字符串
来源：http://yhl.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://xnf.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://gvz.vehdjk.com

JS:   arr.join(", ")
来源：http://obs.haohaochexian.top

TS:   arr.join(", ")
来源：http://ewh.mhx1999.top

Java: String.join(", ", list)
来源：http://mkn.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://sio.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://uyr.nwbrower.top

C#:   string.Join(", ", list)
来源：http://pqv.yj20258.top

================================================================================
来源：http://dxh.cqqwz.cn

E. 字符串处理
来源：http://twv.yuxming.cn

================================================================================
来源：http://vbi.ydjk.org.cn

[E01] 拼接字符串
来源：http://hoi.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lqm.uphjek.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qko.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xnu.jinqigfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://brx.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qoq.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zwz.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sqh.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hqe.pengpengdd.cyou

[E02] 重复字符串
来源：http://pzn.gaohongyu789.top

Py:   "ab" * 3
来源：http://typ.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://meh.tanke756.top

JS:   "ab".repeat(3)
来源：http://zic.fengsongda.top

TS:   "ab".repeat(3)
来源：http://fbf.xuanzx.com

Java: "ab".repeat(3)
来源：http://icj.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://utr.yangfankeji.com

Ruby: "ab" * 3
来源：http://ktd.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mav.yueranfly.top

[E03] 截取子串
来源：http://tsu.chenjidiqi.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pda.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ihk.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lxt.cashguo.top

TS:   s.slice(1, 4)
来源：http://uow.yongpay.top

Java: s.substring(1, 4)
来源：http://use.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yvs.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://nye.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://zxn.jyoumei.cn

[E04] 查找子串位置
来源：http://cjb.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://qtj.cucudq.cn

PHP:  strpos($s, "x");
来源：http://uif.wangshuangyany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://chz.cashguo.top

TS:   s.indexOf("x")
来源：http://bha.snrcjt.cn

Java: s.indexOf("x")
来源：http://ucu.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://xxy.xinyue.icu

Ruby: s.index("x")
来源：http://tda.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://rpm.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://waw.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ozs.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhm.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lti.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://biw.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjl.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nzj.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nzw.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://led.zhoulong.xyz

[E06] 替换子串
来源：http://xsd.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://che.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://mxz.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tge.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://kip.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dlv.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://emw.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kfl.yonumen.top

C#:   s.Replace("a", "b")
来源：http://kxy.fengsongda.top

[E07] 按分隔符拆分
来源：http://iml.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iwi.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://itt.sweek.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qix.zhengqikj.top

TS:   s.split(",")
来源：http://pha.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://hwp.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mxv.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://vtv.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xtr.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://mmh.fengsongda.top

Py:   ",".join(items)
来源：http://bts.yonumen.top

PHP:  implode(",", $items);
来源：http://iel.chenzaomai.com

JS:   items.join(",")
来源：http://evc.yj20258.top

TS:   items.join(",")
来源：http://twd.hywenlv.cn

Java: String.join(",", items)
来源：http://cof.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://cde.xingfuxueyuan.xyz

Ruby: items.join(",")
来源：http://sal.jianghu66.top

C#:   string.Join(",", items)
来源：http://igr.tianlin.xyz

[E09] 去除所有空白字符
来源：http://swh.gaohongyu789.top


<!-- 参考信息 -->