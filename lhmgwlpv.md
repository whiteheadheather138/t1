代发 wailian999

Py:   len(arr)
来源：http://yeh.bjfxy.top

PHP:  count($arr);
来源：http://ybi.xingfuxueyuan.xyz

JS:   arr.length
来源：http://sqb.xylfe.cn

TS:   arr.length
来源：http://fhb.fktsv.cn

Java: list.size();
来源：http://rrc.jinqigfzy.top

Go:   len(arr)
来源：http://aje.kuanghao11.cn

Ruby: arr.length; arr.size
来源：http://xgm.jinghuilouyu.cn

C#:   list.Count;
来源：http://hzj.andypj.xyz

[D07] 切片 / 取子数组
来源：http://gcq.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hfa.jyoumei.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lqm.iojbl.cn

JS:   arr.slice(1, 4);
来源：http://nio.tianlin.xyz

TS:   arr.slice(1, 4);
来源：http://gkr.hammf.cn

Java: list.subList(1, 4);
来源：http://brq.zhiwuduotai.top

Go:   arr[1:4]
来源：http://nlh.hywenlv.cn

Ruby: arr[1, 3]
来源：http://vml.aizwys.cn

C#:   list.GetRange(1, 3);
来源：http://kne.hysaishi.cn

[D08] 合并两个数组
来源：http://jfj.yangfankeji.com

Py:   a + b;  a.extend(b)
来源：http://ddu.shanyushiyangkeji.top

PHP:  array_merge($a, $b);
来源：http://yul.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://dsn.kuanghao11.cn

TS:   [...a, ...b];
来源：http://fhe.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://oke.sjlbkw.cn

Go:   append(a, b...)
来源：http://udv.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://ael.shangyingyoupin.top

C#:   a.Concat(b).ToList()
来源：http://hlf.jlsjyb.cn

[D09] 排序（升序）
来源：http://iaf.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://prp.cashguo.top

PHP:  sort($arr);
来源：http://svt.fehbvm.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rnm.hfpthk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nab.snrcjt.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://emu.zhengqikj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dor.jiagoushi.top

Ruby: arr.sort
来源：http://ejf.tanke756.top

C#:   list.Sort();
来源：http://udv.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://now.gaohongyu789.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hkw.wangshuangyany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://egb.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iio.yonumen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://csp.fanxiaobao.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fxk.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xmi.zhixingplan.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pwe.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gvx.shangyingyoupin.top

[D11] 反转数组
来源：http://mog.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://mhc.gogol.net.cn

PHP:  array_reverse($arr);
来源：http://tnv.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ndk.havefunace.top

TS:   [...arr].reverse();
来源：http://nvr.daria6918.cn

Java: Collections.reverse(list);
来源：http://gsi.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://uos.sysykeji.top

Ruby: arr.reverse
来源：http://psl.meibo888.top

C#:   list.Reverse();
来源：http://kbo.yongpay.top

[D12] 查找元素下标
来源：http://xga.ctjpmb.com

Py:   arr.index(x);  x in arr
来源：http://fwd.gzhubu.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mwr.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wnb.yueranfly.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kiw.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tmz.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://lkn.dianchejie.cn

Ruby: arr.index(x)
来源：http://ywz.yvedp.cn

C#:   list.IndexOf(x);
来源：http://ybw.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://avt.zhiwuduotai.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ton.guannengcc.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xyu.havefunace.top

JS:   arr.filter(x => x > 3)
来源：http://ipj.yueranfly.top

TS:   arr.filter(x => x > 3)
来源：http://nsh.nanxinkj.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://upt.gogol.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://peu.jinghuilouyu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hau.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jbn.chenjidiqi.icu

[D14] 映射转换（每个元素变形）
来源：http://ynj.birdmap.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nvd.jqgfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rls.daxiang520.top

JS:   arr.map(x => x * 2)
来源：http://cpw.fanxiaobao.xyz

TS:   arr.map(x => x * 2)
来源：http://lsi.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://lwp.uphjek.com

Go:   // 手写循环
来源：http://lxk.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://ajw.jinqigfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vwn.mhx1999.top

[D15] 去重
来源：http://rmw.vehdjk.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://avr.cdnleiting.top

PHP:  array_unique($arr);
来源：http://agn.sysykeji.top

JS:   [...new Set(arr)]
来源：http://wam.yj20258888.top

TS:   [...new Set(arr)]
来源：http://wjd.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pmc.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wjv.fehbvm.com

Ruby: arr.uniq
来源：http://zlz.uphjek.com

C#:   list.Distinct().ToList()
来源：http://ufv.xuetiantiany.cn

[D16] 求和与平均值
来源：http://qzc.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://efj.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kom.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gbg.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gng.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://noi.hcnkem.com

Go:   // 手写循环累加
来源：http://uda.sysykeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://trm.mhx1999.top

C#:   list.Sum();  list.Average()
来源：http://ssh.mhx1999.top

[D17] 最大值与最小值
来源：http://cbi.shanyushiyangkeji.top

Py:   max(arr);  min(arr)
来源：http://kki.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://kvn.tanke756.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jpu.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://iun.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://syr.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wdh.xuetiantiany.cn

Ruby: arr.max;  arr.min
来源：http://idn.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://pia.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://mzf.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aas.chenjidiqi.icu

PHP:  array_merge(...$nested);
来源：http://hkk.xingfuxueyuan.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xyw.zdbjq.cn

TS:   nested.flat();
来源：http://ufw.shzxlz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bbb.shzxlz.cn

Go:   // 手写双层循环
来源：http://ppx.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://vla.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://det.hesvh.cn

[D19] 按字段分组
来源：http://ghc.jiagoushi.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://czv.jianghu66.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hmo.sjlbkw.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ftl.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cif.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pzi.yj202588.top

Go:   // 手写 map[string][]T
来源：http://xjq.hongshengwenyu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rxk.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mvf.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://cpf.vqdsnc.cn

Py:   Counter(arr)
来源：http://bjk.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://oza.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvi.yonumen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bgr.xylfe.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dnq.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://gmi.shuidangran.top

Ruby: arr.tally
来源：http://hmd.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://myj.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://aka.yonumen.top

Py:   x in arr
来源：http://zdo.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://jng.zhixingplan.top

JS:   arr.includes(x)
来源：http://pdf.dashuyun.cn

TS:   arr.includes(x)
来源：http://bax.yvedp.cn

Java: list.contains(x)
来源：http://esh.sxryk.cn

Go:   slices.Contains(arr, x)
来源：http://ace.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://jrx.vqdsnc.cn

C#:   list.Contains(x)
来源：http://nxy.yvedp.cn

[D22] 复制数组（避免共享引用）
来源：http://ebn.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qgo.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ycs.bjfxy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://efh.uphjek.com

TS:   [...arr];
来源：http://acc.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://pos.meibo888.top

Go:   copied := append([]int(nil), arr...)
来源：http://hiw.dianchejie.cn

Ruby: arr.dup;  arr.clone
来源：http://ykr.52xcode.cn

C#:   new List<int>(list);
来源：http://cxz.guowangkeji.top

[D23] reduce 累积计算
来源：http://zpv.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ztb.fanxiaobao.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rac.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cvy.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tbf.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uuw.ehwqpu.com

Go:   // 手写循环
来源：http://qdd.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dgh.gaohongyu789.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://stn.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://vhp.xingfuxueyuan.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://alg.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sbl.bjfxy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uzw.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hzc.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mbz.cdnleiting.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ifl.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pcp.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://drg.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://fhu.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ggn.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gkt.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ljo.yj202588.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nxh.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jzi.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zff.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jud.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ubk.jianghu66.top

[D26] 数组转字符串
来源：http://voz.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://ora.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://mnk.sjlbkw.cn

JS:   arr.join(", ")
来源：http://cas.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://klt.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://kdz.yanxiufei.cn

Go:   strings.Join(strs, ", ")
来源：http://djn.jinqigufen.top

Ruby: arr.join(", ")
来源：http://gah.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://gad.sufxvd.cn

================================================================================
来源：http://dsz.iojbl.cn

E. 字符串处理
来源：http://ewb.hesvh.cn

================================================================================
来源：http://ryf.ybcxt.top

[E01] 拼接字符串
来源：http://tyv.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sgl.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fxg.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcv.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cni.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dqw.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qei.tanke756.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mhk.yuanzhike.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://swy.snrcjt.cn

[E02] 重复字符串
来源：http://rao.zhijiandao.cn

Py:   "ab" * 3
来源：http://mfu.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://mdl.smart0.xyz

JS:   "ab".repeat(3)
来源：http://ndp.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://lmv.zhiwuduotai.top

Java: "ab".repeat(3)
来源：http://eai.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://ejr.daxiang520.top

Ruby: "ab" * 3
来源：http://bvj.zhiwuduotai.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uag.sweek.top

[E03] 截取子串
来源：http://yfh.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pct.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pog.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jrw.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://qkb.gotoacloud.top

Java: s.substring(1, 4)
来源：http://prv.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hzi.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bxb.jlsjyb.cn

C#:   s.Substring(1, 3)
来源：http://cyi.tarul.cn

[E04] 查找子串位置
来源：http://khe.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://twk.yfazqb.com

PHP:  strpos($s, "x");
来源：http://hvb.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pqv.hammf.cn

TS:   s.indexOf("x")
来源：http://qfu.meibo888.top

Java: s.indexOf("x")
来源：http://ybo.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://lys.tian-w.cn

Ruby: s.index("x")
来源：http://sdw.daxiang520.top

C#:   s.IndexOf("x")
来源：http://fze.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xlt.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tzq.nwbrower.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wct.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jhv.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mvl.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cka.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lwm.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qoh.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vnx.wangdashe.top

[E06] 替换子串
来源：http://ajw.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oty.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://ixd.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uhg.dianchejie.cn

TS:   s.replaceAll("a", "b")
来源：http://nbp.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bcy.chenlongwang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pyh.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fel.cheryme.top

C#:   s.Replace("a", "b")
来源：http://txc.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://nmm.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://myk.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://swv.guannengcc.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ddh.chenjidiqi.icu

TS:   s.split(",")
来源：http://nsr.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://xse.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bbm.gzhubu.top

Ruby: s.split(",");  s.split
来源：http://zpo.haohaochexian.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lso.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://rpz.xuanzx.com

Py:   ",".join(items)
来源：http://gzd.zhixingplan.top

PHP:  implode(",", $items);
来源：http://cug.wangdashe.top

JS:   items.join(",")
来源：http://xth.jinghuilouyu.cn

TS:   items.join(",")
来源：http://flg.uphjek.com

Java: String.join(",", items)
来源：http://pbk.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://msy.hnqzz.top

Ruby: items.join(",")
来源：http://nwo.bjfxy.top

C#:   string.Join(",", items)
来源：http://ngw.smart0.xyz

[E09] 去除所有空白字符
来源：http://kmf.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://npl.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mqz.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://loo.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://mms.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://ptu.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://djx.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://lce.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gzs.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://bvm.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zhe.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xom.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://ywu.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://jzz.cashguo.top

Java: String.format("%03d", 7)
来源：http://uxf.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ehz.xuetiantiany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://duk.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xjt.xinyue.icu

[E11] 反转字符串
来源：http://soj.ppjwa.cn

Py:   s[::-1]
来源：http://obw.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://snb.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://wir.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://gwc.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pbl.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tjh.hesvh.cn

Ruby: s.reverse
来源：http://uiq.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://qcy.sxryk.cn

[E12] 统计某字符出现次数
来源：http://hxt.fzhhl.top

Py:   s.count("a")
来源：http://drv.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://zdl.fktsv.cn

JS:   s.split("a").length - 1
来源：http://ycv.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://gfn.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwm.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://uiq.aizwys.cn

Ruby: s.count("a")
来源：http://ukg.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://sbl.gaohongyu789.top

[E13] 逐字符遍历
来源：http://lvx.quarkkingdee.top


<!-- 参考信息 -->