代发 wailian999

C#:   list.Insert(0, 0);
来源：http://svn.xziqi.cn

[D04] 删除元素
来源：http://iiq.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://rky.zhijiandao.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vdk.gzhubu.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zpp.jianghu66.top

TS:   arr.splice(0, 1);
来源：http://nmn.xingfuxueyuan.xyz

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://xsq.zhaomingkeji.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://atn.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uew.xuetiantiany.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bww.uphjek.com

[D05] 访问与修改元素
来源：http://iwn.fehbvm.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://nlj.guowangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ole.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zyy.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://szm.fehbvm.com

Java: list.get(0); list.set(0, 9);
来源：http://aai.jiagoushi.top

Go:   arr[0]; arr[0] = 9
来源：http://fzh.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://omz.zhengqikj.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jbs.ehwqpu.com

[D06] 数组长度
来源：http://yrr.feifeiyinyue.top

Py:   len(arr)
来源：http://lar.pengpengdd.cyou

PHP:  count($arr);
来源：http://zzm.xylfe.cn

JS:   arr.length
来源：http://tds.hammf.cn

TS:   arr.length
来源：http://gxg.mhx1999.top

Java: list.size();
来源：http://kkj.xingfuxueyuan.xyz

Go:   len(arr)
来源：http://ybr.jyoumei.cn

Ruby: arr.length; arr.size
来源：http://avh.xylfe.cn

C#:   list.Count;
来源：http://ouu.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://lcr.tarul.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gyc.bbcook.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jlc.shangyingyoupin.top

JS:   arr.slice(1, 4);
来源：http://zhx.ctjpmb.com

TS:   arr.slice(1, 4);
来源：http://xeg.gotoacloud.top

Java: list.subList(1, 4);
来源：http://olj.smart0.xyz

Go:   arr[1:4]
来源：http://drb.hysaishi.cn

Ruby: arr[1, 3]
来源：http://pwf.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://vye.wangdashe.top

[D08] 合并两个数组
来源：http://amb.shanyushiyangtech.top

Py:   a + b;  a.extend(b)
来源：http://aqe.dashuyun.cn

PHP:  array_merge($a, $b);
来源：http://cqa.zhaomingkeji.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://gla.yj202588.top

TS:   [...a, ...b];
来源：http://kvu.kuanghao11.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qhj.hysaishi.cn

Go:   append(a, b...)
来源：http://pwm.yonumen.top

Ruby: a + b;  a.concat(b)
来源：http://nmi.zhoulong.xyz

C#:   a.Concat(b).ToList()
来源：http://mmy.shangyingyoupin.top

[D09] 排序（升序）
来源：http://wnm.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://yun.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://cia.316326.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://skl.cucudq.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ywl.xingfuxueyuan.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://mmp.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yok.bjfxy.top

Ruby: arr.sort
来源：http://rcj.ivvv.top

C#:   list.Sort();
来源：http://caj.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nzt.svipenyu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tbe.yongpay.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://flu.sysykeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jhs.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://olr.nwbrower.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fre.aizwys.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cqb.pycfn.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ygr.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ohd.zycfv.cn

[D11] 反转数组
来源：http://jwg.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://lqo.zdqjudy.top

PHP:  array_reverse($arr);
来源：http://gak.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jel.tian-w.cn

TS:   [...arr].reverse();
来源：http://ccz.iojbl.cn

Java: Collections.reverse(list);
来源：http://vnf.bjfxy.top

Go:   slices.Reverse(arr)
来源：http://wgh.jyoumei.cn

Ruby: arr.reverse
来源：http://zpu.vqdsnc.cn

C#:   list.Reverse();
来源：http://gmo.zhengqikj.top

[D12] 查找元素下标
来源：http://tjr.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://qve.birdmap.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jpo.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dgy.jqgufenzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://grs.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nfe.uphjek.com

Go:   slices.Index(arr, x)
来源：http://ldb.guannengcc.top

Ruby: arr.index(x)
来源：http://xhq.cashguo.top

C#:   list.IndexOf(x);
来源：http://ikn.zdbjq.cn

[D13] 过滤（保留满足条件的）
来源：http://agc.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mvq.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tuu.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://wrf.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://xar.guannengcc.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lno.wangshuangyany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://njb.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://sai.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://llz.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://dft.fehbvm.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kth.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dnh.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://kxq.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://ftw.jlsjyb.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ceb.smart0.xyz

Go:   // 手写循环
来源：http://gqw.ydzc1.top

Ruby: arr.map { |x| x * 2 }
来源：http://dly.sweek.top

C#:   list.Select(x => x * 2).ToList()
来源：http://uvq.redwolf501.top

[D15] 去重
来源：http://juf.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zun.svipenyu.cn

PHP:  array_unique($arr);
来源：http://msa.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://frd.hywenlv.cn

TS:   [...new Set(arr)]
来源：http://mqw.ywan-chungtsiang.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://csh.yj202588.top

Go:   // 用 map[T]struct{} 手写
来源：http://kgk.316326.xyz

Ruby: arr.uniq
来源：http://bat.andypj.xyz

C#:   list.Distinct().ToList()
来源：http://hzl.zhongyouzk.top

[D16] 求和与平均值
来源：http://gqv.uphjek.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kvx.hfpthk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lvh.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jxj.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwr.daxiang520.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xqz.yvedp.cn

Go:   // 手写循环累加
来源：http://izt.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tcx.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://drk.daria6918.cn

[D17] 最大值与最小值
来源：http://gts.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://gjr.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://tbw.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dud.mhx1999.top

TS:   Math.max(...arr);
来源：http://nzm.hfpthk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nsh.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://atn.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://xiw.birdmap.top

C#:   list.Max();  list.Min()
来源：http://gxk.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://rau.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qvf.zhaomingkeji.xyz

PHP:  array_merge(...$nested);
来源：http://lpw.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kbo.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://qut.cheryme.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lxx.hammf.cn

Go:   // 手写双层循环
来源：http://vfz.xuetiantiany.cn

Ruby: nested.flatten
来源：http://evf.cheryme.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jdt.cqqwz.cn

[D19] 按字段分组
来源：http://rvx.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sxz.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://arq.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mtt.hammf.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kyh.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zha.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://cbi.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zfv.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jvu.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://ycc.ydjk.org.cn

Py:   Counter(arr)
来源：http://eng.yfazqb.com

PHP:  array_count_values($arr);
来源：http://ipb.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhi.sweek.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yok.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fdg.sysykeji.top

Go:   // 手写 map[T]int
来源：http://cjx.yongpay.top

Ruby: arr.tally
来源：http://fgx.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hid.xinyue.icu

[D21] 判断是否包含某元素
来源：http://uao.c1oappe.top

Py:   x in arr
来源：http://kjr.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://ejs.dianchejie.cn

JS:   arr.includes(x)
来源：http://cxi.yonumen.top

TS:   arr.includes(x)
来源：http://nls.yongpay.top

Java: list.contains(x)
来源：http://ner.gogol.net.cn

Go:   slices.Contains(arr, x)
来源：http://jib.sxryk.cn

Ruby: arr.include?(x)
来源：http://hgq.yj202588.top

C#:   list.Contains(x)
来源：http://gyg.daxiang520.top

[D22] 复制数组（避免共享引用）
来源：http://isq.aibaodan.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lwp.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vpj.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gpf.meibo888.top

TS:   [...arr];
来源：http://ayy.tanke756.top

Java: new ArrayList<>(list);
来源：http://fol.wangdashe.top

Go:   copied := append([]int(nil), arr...)
来源：http://fwr.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://lla.smart0.xyz

C#:   new List<int>(list);
来源：http://awe.tanke756.top

[D23] reduce 累积计算
来源：http://dnw.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fmy.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wuy.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvk.chenlongwang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nko.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cfq.yuanzhike.top

Go:   // 手写循环
来源：http://gbx.svipenyu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pre.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://loz.zhoulong.xyz

[D24] 字典 / Map 基本操作
来源：http://lfb.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vwa.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fwu.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oin.yvedp.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://axv.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yqb.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://syb.bbcook.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vzx.yueranfly.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ypk.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://uqh.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mfu.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kph.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lll.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yqd.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fgd.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rhv.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lti.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jkv.quarkkingdee.top

[D26] 数组转字符串
来源：http://iwf.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://yza.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://suq.pycfn.com

JS:   arr.join(", ")
来源：http://kqs.redwolf501.top

TS:   arr.join(", ")
来源：http://isr.xingfuxueyuan.xyz

Java: String.join(", ", list)
来源：http://vve.redwolf501.top

Go:   strings.Join(strs, ", ")
来源：http://yyz.shuidangran.top

Ruby: arr.join(", ")
来源：http://aen.yangfankeji.com

C#:   string.Join(", ", list)
来源：http://xtc.daxiang520.top

================================================================================
来源：http://ooa.yuanzhike.top

E. 字符串处理
来源：http://bdr.xylfe.cn

================================================================================
来源：http://lhh.xylfe.cn

[E01] 拼接字符串
来源：http://nth.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ubn.jinqigfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://abt.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hsx.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://asd.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hvz.pengpengdd.cyou

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://soy.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yjv.yfazqb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fgf.pengpengdd.cyou

[E02] 重复字符串
来源：http://rqg.sysykeji.top

Py:   "ab" * 3
来源：http://lnk.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://rhq.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://xjb.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://dqx.bbcook.cn

Java: "ab".repeat(3)
来源：http://swc.ywan-chungtsiang.top

Go:   strings.Repeat("ab", 3)
来源：http://nua.dianchejie.cn

Ruby: "ab" * 3
来源：http://pmx.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yij.52xcode.cn

[E03] 截取子串
来源：http://ztj.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hse.shanyushiyangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mia.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zxe.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://mhx.fehbvm.com

Java: s.substring(1, 4)
来源：http://hho.ydjk.org.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kvr.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://auo.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://ngu.gogol.net.cn

[E04] 查找子串位置
来源：http://kho.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://xtm.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://dvf.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://duu.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://hre.yanxiufei.cn

Java: s.indexOf("x")
来源：http://uud.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://wxp.zhoulong.xyz

Ruby: s.index("x")
来源：http://qwc.aibaodan.cn

C#:   s.IndexOf("x")
来源：http://myn.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yge.dianchejie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dap.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://snx.pengpengdd.cyou

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyv.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://htl.hysaishi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://okj.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://oke.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://odk.hywenlv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lkf.xinyue.icu

[E06] 替换子串
来源：http://sxh.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lwi.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://zla.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ksm.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://rwp.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kgs.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://caf.shuidangran.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://woi.tanke756.top

C#:   s.Replace("a", "b")
来源：http://pxf.ybcxt.top

[E07] 按分隔符拆分
来源：http://uce.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ruv.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://olj.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dcc.yonumen.top

TS:   s.split(",")
来源：http://bds.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://acr.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cnp.wangshuangyany.cn

Ruby: s.split(",");  s.split
来源：http://ouc.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rax.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://lei.zhoulong.xyz

Py:   ",".join(items)
来源：http://sgj.52xcode.cn

PHP:  implode(",", $items);
来源：http://prl.quarkkingdee.top

JS:   items.join(",")
来源：http://uee.zdqjudy.top

TS:   items.join(",")
来源：http://bcm.jqgfzy.top

Java: String.join(",", items)
来源：http://sqy.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://abe.sweek.top

Ruby: items.join(",")
来源：http://qnp.guowangkeji.top

C#:   string.Join(",", items)
来源：http://qfa.316326.xyz

[E09] 去除所有空白字符
来源：http://tvn.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vii.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ast.chenzaomai.com

JS:   s.replace(/\s+/g, "")
来源：http://ccy.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://hlu.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://xwd.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mee.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://cok.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cxl.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://bka.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aln.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mfj.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://hnh.zhongyouzk.top

TS:   "7".padStart(3, "0")
来源：http://klo.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://ylr.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sis.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lel.uphjek.com


<!-- 参考信息 -->