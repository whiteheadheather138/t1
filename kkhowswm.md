代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vhd.smart0.xyz

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tli.birdmap.top

TS:   arr[0]; arr.at(-1);
来源：http://kev.yuanzhike.top

Java: list.get(0); list.set(0, 9);
来源：http://blu.0kj1m.cn

Go:   arr[0]; arr[0] = 9
来源：http://cdg.meibo888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pdx.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://avw.cqqwz.cn

[D06] 数组长度
来源：http://vvy.feifeiyinyue.top

Py:   len(arr)
来源：http://wht.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://oih.meibo888.top

JS:   arr.length
来源：http://xks.nanxuanxn.top

TS:   arr.length
来源：http://azw.sjlbkw.cn

Java: list.size();
来源：http://obp.guowangkeji.top

Go:   len(arr)
来源：http://ovx.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://dmr.ehwqpu.com

C#:   list.Count;
来源：http://uvy.shzxlz.cn

[D07] 切片 / 取子数组
来源：http://ndh.hcnkem.com

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://leo.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ktr.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://zho.daxiang520.top

TS:   arr.slice(1, 4);
来源：http://fns.xuanzx.com

Java: list.subList(1, 4);
来源：http://nde.vehdjk.com

Go:   arr[1:4]
来源：http://wph.xinyue.icu

Ruby: arr[1, 3]
来源：http://lwt.ywan-chungtsiang.top

C#:   list.GetRange(1, 3);
来源：http://bnp.zhongyouzk.top

[D08] 合并两个数组
来源：http://yfq.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://vyz.zhoulong.xyz

PHP:  array_merge($a, $b);
来源：http://bli.vqdsnc.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zgu.gotoacloud.top

TS:   [...a, ...b];
来源：http://jai.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oyi.sweek.top

Go:   append(a, b...)
来源：http://dws.ydjk.org.cn

Ruby: a + b;  a.concat(b)
来源：http://gwm.hnqzz.top

C#:   a.Concat(b).ToList()
来源：http://rvr.yanxiufei.cn

[D09] 排序（升序）
来源：http://bro.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dkp.c1oappe.top

PHP:  sort($arr);
来源：http://vjl.ctjpmb.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://evf.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tmn.vqdsnc.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mmp.gaohongyu789.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ngv.yuanzhike.top

Ruby: arr.sort
来源：http://okz.vqdsnc.cn

C#:   list.Sort();
来源：http://dmi.ywan-chungtsiang.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://zxp.fzhhl.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xpo.zhongyouzk.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iwg.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dur.fanxiaobao.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ibe.birdmap.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bws.sweek.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wnw.smart0.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pzi.zhoulong.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tsv.feifeiyinyue.top

[D11] 反转数组
来源：http://not.jqgfzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://jbd.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://jcd.hcnkem.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gzz.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://ccp.aibaodan.cn

Java: Collections.reverse(list);
来源：http://pyk.yueranfly.top

Go:   slices.Reverse(arr)
来源：http://frf.xinyue.icu

Ruby: arr.reverse
来源：http://fhn.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://bdy.smart0.xyz

[D12] 查找元素下标
来源：http://dki.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://ftx.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kui.yueranfly.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dtv.fktsv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mmy.shzxlz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rqa.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://qlx.sweek.top

Ruby: arr.index(x)
来源：http://oxp.hammf.cn

C#:   list.IndexOf(x);
来源：http://ypf.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://awm.yj202588.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fzk.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jel.fanxiaobao.xyz

JS:   arr.filter(x => x > 3)
来源：http://dns.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://olu.ivvv.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tld.snrcjt.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vjv.ybcxt.top

Ruby: arr.select { |x| x > 3 }
来源：http://aom.52xcode.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yro.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://lob.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ifu.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lgu.nanxinkj.top

JS:   arr.map(x => x * 2)
来源：http://ssz.tian-w.cn

TS:   arr.map(x => x * 2)
来源：http://pae.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lih.xylfe.cn

Go:   // 手写循环
来源：http://cek.aizwys.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fyt.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://kls.fengsongda.top

[D15] 去重
来源：http://uum.gotoacloud.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gyn.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://ari.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://pgy.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://pnv.hnqzz.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fdd.fanxiaobao.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://jch.bjfxy.top

Ruby: arr.uniq
来源：http://kvt.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://kof.jlsjyb.cn

[D16] 求和与平均值
来源：http://svv.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xjb.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tki.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jyp.hammf.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsz.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pyl.vqdsnc.cn

Go:   // 手写循环累加
来源：http://nkc.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qyj.ctjpmb.com

C#:   list.Sum();  list.Average()
来源：http://fsh.ehwqpu.com

[D17] 最大值与最小值
来源：http://ylv.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://ect.mhx1999.top

PHP:  max($arr);  min($arr);
来源：http://nov.hysaishi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qsu.aizwys.cn

TS:   Math.max(...arr);
来源：http://abx.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://agm.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jue.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://ihc.hammf.cn

C#:   list.Max();  list.Min()
来源：http://qfc.tarul.cn

[D18] 扁平化嵌套数组
来源：http://cui.epnwcf.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ehz.zhengqikj.top

PHP:  array_merge(...$nested);
来源：http://gzf.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://asc.ydzc1.top

TS:   nested.flat();
来源：http://yqc.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tfs.sjlbkw.cn

Go:   // 手写双层循环
来源：http://row.daria6918.cn

Ruby: nested.flatten
来源：http://dif.vqdsnc.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mes.fengsongda.top

[D19] 按字段分组
来源：http://frg.jlsjyb.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vvn.xziqi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tcn.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xjw.daria6918.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://osb.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://icj.52xcode.cn

Go:   // 手写 map[string][]T
来源：http://sps.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rxg.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vzx.jqgfzy.top

[D20] 统计每个元素出现次数
来源：http://xhg.hywenlv.cn

Py:   Counter(arr)
来源：http://rzt.jinqigfzy.top

PHP:  array_count_values($arr);
来源：http://wts.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hrg.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oiv.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ohq.yj202588.top

Go:   // 手写 map[T]int
来源：http://bnw.cheryme.top

Ruby: arr.tally
来源：http://zif.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gji.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://xul.vehdjk.com

Py:   x in arr
来源：http://eft.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://enr.ydzc1.top

JS:   arr.includes(x)
来源：http://xkk.yueranfly.top

TS:   arr.includes(x)
来源：http://pyc.daxiang520.top

Java: list.contains(x)
来源：http://rqv.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://eew.wangdashe.top

Ruby: arr.include?(x)
来源：http://noc.zdbjq.cn

C#:   list.Contains(x)
来源：http://muy.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://wyw.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://brp.gogol.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tew.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ogr.shanyushiyangtech.top

TS:   [...arr];
来源：http://vvq.bbcook.cn

Java: new ArrayList<>(list);
来源：http://iux.yanxiufei.cn

Go:   copied := append([]int(nil), arr...)
来源：http://omm.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://bfj.wangdashe.top

C#:   new List<int>(list);
来源：http://kqr.snrcjt.cn

[D23] reduce 累积计算
来源：http://tig.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cyq.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aai.daxiang520.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kwt.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jsz.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cnf.tarul.cn

Go:   // 手写循环
来源：http://jrg.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vyd.cqqwz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qnj.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://yea.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ory.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pba.zhaomingkeji.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gid.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vhn.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://enb.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vyj.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xrt.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wkb.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://vea.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rlq.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vsy.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vqz.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wqz.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tju.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vkx.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://frx.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pcm.cdnleiting.top

[D26] 数组转字符串
来源：http://gje.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://akk.shangyingyoupin.top

PHP:  implode(", ", $arr);
来源：http://jdu.gaohongyu789.top

JS:   arr.join(", ")
来源：http://cbr.birdmap.top

TS:   arr.join(", ")
来源：http://dba.zhixingplan.top

Java: String.join(", ", list)
来源：http://ioq.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://igf.ydjk.org.cn

Ruby: arr.join(", ")
来源：http://fvh.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://ibe.ydzc1.top

================================================================================
来源：http://wuu.jiagoushi.top

E. 字符串处理
来源：http://gjl.aizwys.cn

================================================================================
来源：http://dtb.nanxinkj.top

[E01] 拼接字符串
来源：http://dsf.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://roc.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://imp.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zra.ywan-chungtsiang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ood.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rnn.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gnx.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fyp.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qer.jyoumei.cn

[E02] 重复字符串
来源：http://qgy.wangdashe.top

Py:   "ab" * 3
来源：http://jpg.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://fhn.redwolf501.top

JS:   "ab".repeat(3)
来源：http://vwj.tarul.cn

TS:   "ab".repeat(3)
来源：http://yoz.birdmap.top

Java: "ab".repeat(3)
来源：http://kbv.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://qap.52xcode.cn

Ruby: "ab" * 3
来源：http://sag.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sef.haohaochexian.top

[E03] 截取子串
来源：http://esp.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mkg.wangshuangyany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yel.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yxn.yongpay.top

TS:   s.slice(1, 4)
来源：http://rdy.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://zzx.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://isl.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://spo.sysykeji.top

C#:   s.Substring(1, 3)
来源：http://jvw.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://cje.jqgfzy.top

Py:   s.find("x");  s.index("x")
来源：http://fzc.ybcxt.top

PHP:  strpos($s, "x");
来源：http://crx.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wsx.hysaishi.cn

TS:   s.indexOf("x")
来源：http://big.vqdsnc.cn

Java: s.indexOf("x")
来源：http://rkm.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://dhd.shangyingyoupin.top

Ruby: s.index("x")
来源：http://wuo.jqgufenzy.top

C#:   s.IndexOf("x")
来源：http://qfb.sxryk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nxd.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fvy.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ctf.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzf.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kas.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fym.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yjb.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uvx.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://woh.xinyue.icu

[E06] 替换子串
来源：http://pta.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://plq.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://vtj.dashuyun.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dru.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://rcr.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hwh.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kez.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lml.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://ilb.meibo888.top

[E07] 按分隔符拆分
来源：http://kfp.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qix.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qtm.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://crt.pycfn.com

TS:   s.split(",")
来源：http://dno.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://one.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lwt.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://lzx.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sdf.tanke756.top

[E08] 数组按分隔符合并
来源：http://bgn.bbcook.cn

Py:   ",".join(items)
来源：http://uhw.aizwys.cn

PHP:  implode(",", $items);
来源：http://tjb.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://ppw.snrcjt.cn

TS:   items.join(",")
来源：http://fpz.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://kui.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://wxv.yanxiufei.cn

Ruby: items.join(",")
来源：http://obi.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://cfn.aizwys.cn

[E09] 去除所有空白字符
来源：http://ryc.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sjo.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qvt.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://fir.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://irn.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://ytw.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fjw.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://mfh.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kmg.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://vsm.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://axx.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tvo.vehdjk.com

JS:   "7".padStart(3, "0")
来源：http://yhe.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://nor.316326.xyz

Java: String.format("%03d", 7)
来源：http://sjq.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mnz.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rxi.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hvw.ivvv.top

[E11] 反转字符串
来源：http://kig.zhoulong.xyz

Py:   s[::-1]
来源：http://rew.sufxvd.cn

PHP:  strrev($s);
来源：http://ysc.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://ujb.zhiwuduotai.top

TS:   [...s].reverse().join("")
来源：http://sil.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hjf.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://deq.cucudq.cn

Ruby: s.reverse
来源：http://bek.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vze.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://ywj.fengsongda.top

Py:   s.count("a")
来源：http://pkj.zdqjudy.top


<!-- 参考信息 -->