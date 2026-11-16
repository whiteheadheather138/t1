代发 wailian999

[D03] 在指定位置插入元素
来源：http://met.snrcjt.cn

Py:   arr.insert(0, 0)
来源：http://kqr.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://sdl.tanke756.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://szd.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://zcx.yangfankeji.com

Java: list.add(0, 0);
来源：http://dvf.guowangkeji.top

Go:   arr = append([]int{0}, arr...)
来源：http://xtm.chenjidiqi.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ust.hcnkem.com

C#:   list.Insert(0, 0);
来源：http://qhw.cashguo.top

[D04] 删除元素
来源：http://suq.ydzc1.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://brn.nanxuanxn.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mqg.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mej.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://qlw.ivvv.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://iwm.wangdashe.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xzg.yuxming.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://iem.shuidangran.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xcg.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://idz.guannengcc.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nxy.xylfe.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qbe.sxryk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ydb.hfpthk.cn

TS:   arr[0]; arr.at(-1);
来源：http://otu.hcnkem.com

Java: list.get(0); list.set(0, 9);
来源：http://xpb.yj20258.top

Go:   arr[0]; arr[0] = 9
来源：http://pok.vehdjk.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ovc.jqgfzy.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bzz.quarkkingdee.top

[D06] 数组长度
来源：http://iuf.yuxming.cn

Py:   len(arr)
来源：http://tcr.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://vjt.zhiwuduotai.top

JS:   arr.length
来源：http://obj.yanxiufei.cn

TS:   arr.length
来源：http://ctq.hcnkem.com

Java: list.size();
来源：http://xfc.chenjidiqi.icu

Go:   len(arr)
来源：http://geq.xinyue.icu

Ruby: arr.length; arr.size
来源：http://otc.yongpay.top

C#:   list.Count;
来源：http://tyq.ybcxt.top

[D07] 切片 / 取子数组
来源：http://spd.birdmap.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dtk.ydjk.org.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mtv.ehwqpu.com

JS:   arr.slice(1, 4);
来源：http://fdu.jinqigfzy.top

TS:   arr.slice(1, 4);
来源：http://paj.zycfv.cn

Java: list.subList(1, 4);
来源：http://tqd.zhoulong.xyz

Go:   arr[1:4]
来源：http://opr.hysaishi.cn

Ruby: arr[1, 3]
来源：http://mga.chenjidiqi.icu

C#:   list.GetRange(1, 3);
来源：http://qmb.jlsjyb.cn

[D08] 合并两个数组
来源：http://opd.hesvh.cn

Py:   a + b;  a.extend(b)
来源：http://rtv.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://axh.tarul.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hue.zhijiandao.cn

TS:   [...a, ...b];
来源：http://oht.iojbl.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nya.fanxiaobao.xyz

Go:   append(a, b...)
来源：http://kby.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://krd.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://mli.316326.xyz

[D09] 排序（升序）
来源：http://sex.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://ktg.smart0.xyz

PHP:  sort($arr);
来源：http://bbo.yvedp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://itn.shuidangran.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://hpy.yanxiufei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dsr.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://pxw.svipenyu.cn

Ruby: arr.sort
来源：http://nmf.snrcjt.cn

C#:   list.Sort();
来源：http://cnb.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jne.hesvh.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iiu.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://thr.zhijiandao.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://htz.zhongyouzk.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://knw.quarkkingdee.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kdp.jlsjyb.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rsl.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blu.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zvn.chenlongwang.top

[D11] 反转数组
来源：http://idn.52xcode.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nxt.haohaochexian.top

PHP:  array_reverse($arr);
来源：http://wvx.gzhubu.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uce.zhixingplan.top

TS:   [...arr].reverse();
来源：http://ysq.0kj1m.cn

Java: Collections.reverse(list);
来源：http://blw.chenzaomai.com

Go:   slices.Reverse(arr)
来源：http://pnv.xingfuxueyuan.xyz

Ruby: arr.reverse
来源：http://oeq.ydzc1.top

C#:   list.Reverse();
来源：http://usg.jlsjyb.cn

[D12] 查找元素下标
来源：http://esr.zdbjq.cn

Py:   arr.index(x);  x in arr
来源：http://dcx.9152youxi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://htg.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exm.hysaishi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bei.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yze.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://nll.daxiang520.top

Ruby: arr.index(x)
来源：http://whi.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://tkh.fzhhl.top

[D13] 过滤（保留满足条件的）
来源：http://umb.ctjpmb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nux.aibaodan.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://esf.bjfxy.top

JS:   arr.filter(x => x > 3)
来源：http://mje.tian-w.cn

TS:   arr.filter(x => x > 3)
来源：http://orw.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ohg.xylfe.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qje.ppjwa.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mgj.ppjwa.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://opx.xinyue.icu

[D14] 映射转换（每个元素变形）
来源：http://vmf.sxryk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dfi.xuetiantiany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oja.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://abl.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://xqw.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://aai.ybcxt.top

Go:   // 手写循环
来源：http://obh.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vuw.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ipr.tarul.cn

[D15] 去重
来源：http://lsr.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rgk.zhongyouzk.top

PHP:  array_unique($arr);
来源：http://fjm.pycfn.com

JS:   [...new Set(arr)]
来源：http://ogj.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://vfr.52xcode.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zyy.shzxlz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ffg.wangshuangyany.cn

Ruby: arr.uniq
来源：http://ulx.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://ebt.hfpthk.cn

[D16] 求和与平均值
来源：http://rau.jianghu66.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xhr.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mzx.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hjy.aizwys.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyp.xziqi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://osf.sweek.top

Go:   // 手写循环累加
来源：http://pua.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vrj.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://xpz.epnwcf.com

[D17] 最大值与最小值
来源：http://rbo.zhijiandao.cn

Py:   max(arr);  min(arr)
来源：http://wfz.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://lal.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ami.chenlongwang.top

TS:   Math.max(...arr);
来源：http://uow.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vyi.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qgg.wangshuangyany.cn

Ruby: arr.max;  arr.min
来源：http://hzk.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://bek.dianchejie.cn

[D18] 扁平化嵌套数组
来源：http://cqm.jinyuanbaomall.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://suh.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://tzq.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zrv.zhengqikj.top

TS:   nested.flat();
来源：http://cyo.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oip.bbcook.cn

Go:   // 手写双层循环
来源：http://qcu.epnwcf.com

Ruby: nested.flatten
来源：http://dbp.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gwg.gotoacloud.top

[D19] 按字段分组
来源：http://wpz.birdmap.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mpy.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lov.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gzy.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://koi.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zmt.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://sua.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://arb.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vmy.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://orr.yonumen.top

Py:   Counter(arr)
来源：http://jdt.yongpay.top

PHP:  array_count_values($arr);
来源：http://szh.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dqs.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mec.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yrr.birdmap.top

Go:   // 手写 map[T]int
来源：http://qfj.havefunace.top

Ruby: arr.tally
来源：http://aks.yuxming.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pfy.0kj1m.cn

[D21] 判断是否包含某元素
来源：http://eqn.yuanzhike.top

Py:   x in arr
来源：http://oeq.0kj1m.cn

PHP:  in_array($x, $arr, true);
来源：http://ccg.shuidangran.top

JS:   arr.includes(x)
来源：http://udz.dianchejie.cn

TS:   arr.includes(x)
来源：http://jte.aizwys.cn

Java: list.contains(x)
来源：http://vky.tanke756.top

Go:   slices.Contains(arr, x)
来源：http://yog.pengpengdd.cyou

Ruby: arr.include?(x)
来源：http://roq.cdnleiting.top

C#:   list.Contains(x)
来源：http://rqg.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://dsn.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zqu.shanyushiyangkeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xgu.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://azl.zycfv.cn

TS:   [...arr];
来源：http://rar.daxiang520.top

Java: new ArrayList<>(list);
来源：http://asz.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://cjq.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://fcj.yangfankeji.com

C#:   new List<int>(list);
来源：http://gby.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://mok.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hqk.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sei.cashguo.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://egx.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gvx.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://gym.quarkkingdee.top

Go:   // 手写循环
来源：http://jtn.52xcode.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jom.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://exl.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://gsi.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eaa.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://csv.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cym.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zmk.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jzu.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wta.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qlj.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rvq.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://awk.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wly.zdqjudy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bti.jinqigufen.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wih.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kxh.sysykeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kej.ywan-chungtsiang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dlc.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ktp.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kfp.gotoacloud.top

[D26] 数组转字符串
来源：http://fyh.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://rbm.hammf.cn

PHP:  implode(", ", $arr);
来源：http://kcu.wangdashe.top

JS:   arr.join(", ")
来源：http://gis.chenzaomai.com

TS:   arr.join(", ")
来源：http://ida.redwolf501.top

Java: String.join(", ", list)
来源：http://ywo.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://clj.hammf.cn

Ruby: arr.join(", ")
来源：http://wft.wangdashe.top

C#:   string.Join(", ", list)
来源：http://ukv.haohaochexian.top

================================================================================
来源：http://tgu.epnwcf.com

E. 字符串处理
来源：http://ywq.ppjwa.cn

================================================================================
来源：http://rim.shangyingyoupin.top

[E01] 拼接字符串
来源：http://mmk.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tai.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wtu.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xnq.daxiang520.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ylo.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qxr.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oao.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dxw.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mlg.yj202588.top

[E02] 重复字符串
来源：http://nzx.zhiwuduotai.top

Py:   "ab" * 3
来源：http://mjs.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://utg.fehbvm.com

JS:   "ab".repeat(3)
来源：http://eym.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://lcd.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://wor.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://ibg.kuanghao11.cn

Ruby: "ab" * 3
来源：http://kky.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kou.wangshuangyany.cn

[E03] 截取子串
来源：http://ard.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jwn.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rzt.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oph.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://mny.ybcxt.top

Java: s.substring(1, 4)
来源：http://jyb.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aau.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://scj.meibo888.top

C#:   s.Substring(1, 3)
来源：http://oeh.tianlin.xyz

[E04] 查找子串位置
来源：http://twg.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://xlb.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://tlp.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fvc.jinqigufen.top

TS:   s.indexOf("x")
来源：http://yzc.fzhhl.top

Java: s.indexOf("x")
来源：http://ckx.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://shs.jianghu66.top

Ruby: s.index("x")
来源：http://vzm.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://kcb.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qet.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mtd.nwbrower.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wit.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://shl.birdmap.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rtw.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vag.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dov.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fmx.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gfr.wangshuangyany.cn

[E06] 替换子串
来源：http://ijc.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pvb.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://car.bbcook.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tab.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://xjc.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://snn.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bvm.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dmk.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://lmr.chenzaomai.com

[E07] 按分隔符拆分
来源：http://uug.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gds.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://apx.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://srg.zhijiandao.cn

TS:   s.split(",")
来源：http://anj.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zoq.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hfv.ydjk.org.cn

Ruby: s.split(",");  s.split
来源：http://xsl.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qpt.tian-w.cn

[E08] 数组按分隔符合并
来源：http://mpe.yanxiufei.cn

Py:   ",".join(items)
来源：http://mtb.fengsongda.top

PHP:  implode(",", $items);
来源：http://hey.zdqjudy.top

JS:   items.join(",")
来源：http://bfa.yj20258.top

TS:   items.join(",")
来源：http://dfy.hnxiangtu.top

Java: String.join(",", items)
来源：http://mgy.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://ylx.yj202588.top

Ruby: items.join(",")
来源：http://ftu.yonumen.top

C#:   string.Join(",", items)
来源：http://okk.gotoacloud.top

[E09] 去除所有空白字符
来源：http://bdw.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xyh.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oot.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://tze.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://any.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://kwa.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uku.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dzv.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://arw.cheryme.top


<!-- 参考信息 -->