代发 wailian999

[D03] 在指定位置插入元素
来源：http://efa.daria6918.cn

Py:   arr.insert(0, 0)
来源：http://xwq.kuanghao11.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xlo.chenjidiqi.icu

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gqh.ppjwa.cn

TS:   arr.splice(0, 0, 0);
来源：http://shy.yj20258888.top

Java: list.add(0, 0);
来源：http://dub.wangdashe.top

Go:   arr = append([]int{0}, arr...)
来源：http://xjz.yongpay.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ach.ctjpmb.com

C#:   list.Insert(0, 0);
来源：http://mlq.yuxming.cn

[D04] 删除元素
来源：http://lcn.ywan-chungtsiang.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xyl.sweek.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vvj.daxiang520.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mzh.chenlongwang.top

TS:   arr.splice(0, 1);
来源：http://xcu.bjfxy.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zde.zhixingplan.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ueq.gotoacloud.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qkp.ctjpmb.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ugn.ydzc1.top

[D05] 访问与修改元素
来源：http://mjp.sysykeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mig.xinyue.icu

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wbg.kuanghao11.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cux.havefunace.top

TS:   arr[0]; arr.at(-1);
来源：http://rmw.shanyushiyangtech.top

Java: list.get(0); list.set(0, 9);
来源：http://nsi.fktsv.cn

Go:   arr[0]; arr[0] = 9
来源：http://xhs.zhijiandao.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fvj.shzxlz.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fcm.fanxiaobao.xyz

[D06] 数组长度
来源：http://aio.pengpengdd.cyou

Py:   len(arr)
来源：http://ehl.cucudq.cn

PHP:  count($arr);
来源：http://jtq.52xcode.cn

JS:   arr.length
来源：http://jwc.ywan-chungtsiang.top

TS:   arr.length
来源：http://llw.guannengcc.top

Java: list.size();
来源：http://cxv.cashguo.top

Go:   len(arr)
来源：http://dhw.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://vlc.jqgfzy.top

C#:   list.Count;
来源：http://akd.hcnkem.com

[D07] 切片 / 取子数组
来源：http://vgm.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yhd.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jfr.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://zal.xuanzx.com

TS:   arr.slice(1, 4);
来源：http://vrv.ehwqpu.com

Java: list.subList(1, 4);
来源：http://leq.xinyue.icu

Go:   arr[1:4]
来源：http://iet.hcnkem.com

Ruby: arr[1, 3]
来源：http://kso.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://wzz.jyoumei.cn

[D08] 合并两个数组
来源：http://egd.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://kyp.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://wyl.ydjk.org.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mlm.guowangkeji.top

TS:   [...a, ...b];
来源：http://qqd.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://aae.yuxming.cn

Go:   append(a, b...)
来源：http://tdw.kuanghao11.cn

Ruby: a + b;  a.concat(b)
来源：http://npe.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://gxo.cucudq.cn

[D09] 排序（升序）
来源：http://pvs.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://vrg.xinyue.icu

PHP:  sort($arr);
来源：http://evp.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xal.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://svv.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rrf.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dyy.cqqwz.cn

Ruby: arr.sort
来源：http://mco.hfpthk.cn

C#:   list.Sort();
来源：http://ctw.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ucc.ybcxt.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yzf.fengsongda.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssz.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://chc.epnwcf.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zxg.xinyue.icu

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rvw.xinyue.icu

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uqe.hnqzz.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mpm.chenjidiqi.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kha.hnqzz.top

[D11] 反转数组
来源：http://wwr.gogol.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://oju.yfazqb.com

PHP:  array_reverse($arr);
来源：http://xft.daria6918.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nxt.fengsongda.top

TS:   [...arr].reverse();
来源：http://zzb.ivvv.top

Java: Collections.reverse(list);
来源：http://aau.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://fuh.chenlongwang.top

Ruby: arr.reverse
来源：http://ani.tian-w.cn

C#:   list.Reverse();
来源：http://udk.gotoacloud.top

[D12] 查找元素下标
来源：http://cez.c1oappe.top

Py:   arr.index(x);  x in arr
来源：http://lpt.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gfb.tanke756.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mbd.9152youxi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycw.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yzo.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://tkh.jianghu66.top

Ruby: arr.index(x)
来源：http://whn.yfazqb.com

C#:   list.IndexOf(x);
来源：http://rur.cheryme.top

[D13] 过滤（保留满足条件的）
来源：http://bmm.jyoumei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wod.ehwqpu.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://osf.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://ard.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://auu.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cbl.guannengcc.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://niv.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wya.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://fxs.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://rob.yanxiufei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kws.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sul.zdbjq.cn

JS:   arr.map(x => x * 2)
来源：http://can.shzxlz.cn

TS:   arr.map(x => x * 2)
来源：http://srq.sweek.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uev.zdqjudy.top

Go:   // 手写循环
来源：http://ciw.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://wyd.aizwys.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qon.feifeiyinyue.top

[D15] 去重
来源：http://acm.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kvf.xziqi.cn

PHP:  array_unique($arr);
来源：http://jal.dashuyun.cn

JS:   [...new Set(arr)]
来源：http://ozq.jianghu66.top

TS:   [...new Set(arr)]
来源：http://oxh.jinqigufen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gwg.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://mkj.bjfxy.top

Ruby: arr.uniq
来源：http://epm.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://egu.pengpengdd.cyou

[D16] 求和与平均值
来源：http://ejn.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rlz.zhiwuduotai.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tpt.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://evn.gotoacloud.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnf.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xkk.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://svh.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qmw.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://hek.guowangkeji.top

[D17] 最大值与最小值
来源：http://gzc.shangyingyoupin.top

Py:   max(arr);  min(arr)
来源：http://rzo.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://lrs.9152youxi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fmz.hysaishi.cn

TS:   Math.max(...arr);
来源：http://wsc.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cnw.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vgj.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://rcm.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://gqk.hywenlv.cn

[D18] 扁平化嵌套数组
来源：http://unt.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xek.yfazqb.com

PHP:  array_merge(...$nested);
来源：http://bbk.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xkq.xuetiantiany.cn

TS:   nested.flat();
来源：http://iio.bbcook.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://edx.hcnkem.com

Go:   // 手写双层循环
来源：http://pie.jqgfzy.top

Ruby: nested.flatten
来源：http://mlj.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wdu.yangfankeji.com

[D19] 按字段分组
来源：http://rnh.316326.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ehh.guannengcc.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xqe.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pkz.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lpv.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gnb.cdnleiting.top

Go:   // 手写 map[string][]T
来源：http://ehr.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://zav.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lio.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://lwy.ydjk.org.cn

Py:   Counter(arr)
来源：http://sjs.jianghu66.top

PHP:  array_count_values($arr);
来源：http://hdp.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pnw.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xdh.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dhl.jianghu66.top

Go:   // 手写 map[T]int
来源：http://ukc.sysykeji.top

Ruby: arr.tally
来源：http://vbq.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zii.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://luk.fehbvm.com

Py:   x in arr
来源：http://upe.feifeiyinyue.top

PHP:  in_array($x, $arr, true);
来源：http://ocr.xylfe.cn

JS:   arr.includes(x)
来源：http://iex.hfpthk.cn

TS:   arr.includes(x)
来源：http://dmh.hnqzz.top

Java: list.contains(x)
来源：http://etf.yuxming.cn

Go:   slices.Contains(arr, x)
来源：http://eaa.xziqi.cn

Ruby: arr.include?(x)
来源：http://bpt.guannengcc.top

C#:   list.Contains(x)
来源：http://lnn.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://kzg.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hdk.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lqt.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jyx.zhaomingkeji.xyz

TS:   [...arr];
来源：http://ojm.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://jan.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://mxc.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://gnu.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://hcw.kuanghao11.cn

[D23] reduce 累积计算
来源：http://npy.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gbb.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nmr.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hqh.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xkd.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kym.epnwcf.com

Go:   // 手写循环
来源：http://hxo.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cud.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zbx.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://toi.daxiang520.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://utq.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jki.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hyi.dashuyun.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lip.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rfn.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ocp.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xcy.zhaomingkeji.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://icu.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://kje.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lmz.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://msy.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ygi.tianlin.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wam.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gda.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ahw.uphjek.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kaa.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zxo.dianchejie.cn

[D26] 数组转字符串
来源：http://nss.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://hnh.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://owu.9152youxi.cn

JS:   arr.join(", ")
来源：http://abk.zdqjudy.top

TS:   arr.join(", ")
来源：http://aeq.gzhubu.top

Java: String.join(", ", list)
来源：http://cxs.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://fwg.gogol.net.cn

Ruby: arr.join(", ")
来源：http://udz.tarul.cn

C#:   string.Join(", ", list)
来源：http://ljm.pycfn.com

================================================================================
来源：http://nof.tarul.cn

E. 字符串处理
来源：http://oxc.xinyue.icu

================================================================================
来源：http://fud.yueranfly.top

[E01] 拼接字符串
来源：http://nud.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wok.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jtw.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xlq.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ocr.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://knw.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zer.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://atj.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cxh.daria6918.cn

[E02] 重复字符串
来源：http://ahp.sjlbkw.cn

Py:   "ab" * 3
来源：http://goi.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://tuo.daxiang520.top

JS:   "ab".repeat(3)
来源：http://lep.xinyue.icu

TS:   "ab".repeat(3)
来源：http://ydx.jyoumei.cn

Java: "ab".repeat(3)
来源：http://bqj.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://rog.hnxiangtu.top

Ruby: "ab" * 3
来源：http://rec.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lcm.shangyingyoupin.top

[E03] 截取子串
来源：http://cau.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qir.jqgfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kuy.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tru.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://lxa.nanxinkj.top

Java: s.substring(1, 4)
来源：http://oxy.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ynl.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://gsu.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://lzr.nanxinkj.top

[E04] 查找子串位置
来源：http://ugg.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://nez.uphjek.com

PHP:  strpos($s, "x");
来源：http://azd.snrcjt.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yms.yonumen.top

TS:   s.indexOf("x")
来源：http://zrr.zhaomingkeji.xyz

Java: s.indexOf("x")
来源：http://ini.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://cbv.havefunace.top

Ruby: s.index("x")
来源：http://are.yanxiufei.cn

C#:   s.IndexOf("x")
来源：http://frh.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kvf.tianlin.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kpk.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wsg.tian-w.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ufy.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dtg.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgo.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sso.svipenyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vvr.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pkg.daxiang520.top

[E06] 替换子串
来源：http://vqy.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jbl.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://wjx.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpb.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://fod.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpv.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hft.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oly.xinyue.icu

C#:   s.Replace("a", "b")
来源：http://clc.cucudq.cn

[E07] 按分隔符拆分
来源：http://vde.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://omr.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tgb.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dfr.snrcjt.cn

TS:   s.split(",")
来源：http://nnq.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://ttl.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dyj.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://hun.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ain.vehdjk.com

[E08] 数组按分隔符合并
来源：http://dyn.chenzaomai.com

Py:   ",".join(items)
来源：http://isd.yuxming.cn

PHP:  implode(",", $items);
来源：http://sgj.sjlbkw.cn

JS:   items.join(",")
来源：http://ttx.aizwys.cn

TS:   items.join(",")
来源：http://zls.ehwqpu.com

Java: String.join(",", items)
来源：http://drp.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://tmq.vehdjk.com

Ruby: items.join(",")
来源：http://frc.wangdashe.top

C#:   string.Join(",", items)
来源：http://bjm.shzxlz.cn

[E09] 去除所有空白字符
来源：http://vfz.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://niq.chenlongwang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bda.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://lrv.tarul.cn

TS:   s.replace(/\s+/g, "")
来源：http://byu.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xhm.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://znl.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://ahf.fzhhl.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mdi.jinqigfzy.top


<!-- 参考信息 -->