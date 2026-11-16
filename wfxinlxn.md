代发 wailian999

PHP:  sort($arr);
来源：http://wdl.ydjk.org.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ezq.hywenlv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gjs.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fua.xziqi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jfc.gotoacloud.top

Ruby: arr.sort
来源：http://cpy.pengpengdd.cyou

C#:   list.Sort();
来源：http://ufh.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sgv.zdqjudy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://okz.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aya.smart0.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rex.fktsv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ryl.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://emp.hnxiangtu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uln.hcnkem.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rwn.yvedp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://smd.jqgufenzy.top

[D11] 反转数组
来源：http://lfi.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://ikw.yanxiufei.cn

PHP:  array_reverse($arr);
来源：http://nop.jinqigufen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pzf.xuetiantiany.cn

TS:   [...arr].reverse();
来源：http://jgn.jiagoushi.top

Java: Collections.reverse(list);
来源：http://vdm.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://qqg.dashuyun.cn

Ruby: arr.reverse
来源：http://klk.zycfv.cn

C#:   list.Reverse();
来源：http://ieg.xziqi.cn

[D12] 查找元素下标
来源：http://huk.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://kmn.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cle.zhaomingkeji.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qnj.hesvh.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://laf.dashuyun.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jto.shanyushiyangkeji.top

Go:   slices.Index(arr, x)
来源：http://ltk.dashuyun.cn

Ruby: arr.index(x)
来源：http://xxy.fzhhl.top

C#:   list.IndexOf(x);
来源：http://adx.xziqi.cn

[D13] 过滤（保留满足条件的）
来源：http://ofv.epnwcf.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ayk.guowangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xpr.xuanzx.com

JS:   arr.filter(x => x > 3)
来源：http://ewe.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://ixz.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://knz.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mez.chenjidiqi.icu

Ruby: arr.select { |x| x > 3 }
来源：http://phw.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mbf.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://ite.yongpay.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://buy.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yzm.shanyushiyangtech.top

JS:   arr.map(x => x * 2)
来源：http://liy.guannengcc.top

TS:   arr.map(x => x * 2)
来源：http://lmd.xuanzx.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ziy.jyoumei.cn

Go:   // 手写循环
来源：http://yxy.aibaodan.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qqq.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://teq.cheryme.top

[D15] 去重
来源：http://auu.guannengcc.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nlj.dashuyun.cn

PHP:  array_unique($arr);
来源：http://jcn.jiagoushi.top

JS:   [...new Set(arr)]
来源：http://dbi.jinghuilouyu.cn

TS:   [...new Set(arr)]
来源：http://gay.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lmz.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://igs.sufxvd.cn

Ruby: arr.uniq
来源：http://pbn.pycfn.com

C#:   list.Distinct().ToList()
来源：http://pek.daxiang520.top

[D16] 求和与平均值
来源：http://epo.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uhz.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xdm.aibaodan.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://npr.shanyushiyangkeji.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hws.zycfv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ohq.feifeiyinyue.top

Go:   // 手写循环累加
来源：http://zxj.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lrl.snrcjt.cn

C#:   list.Sum();  list.Average()
来源：http://emq.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://vbp.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://rtv.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://xra.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dxc.gzhubu.top

TS:   Math.max(...arr);
来源：http://lwi.xylfe.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ylu.bjfxy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oqj.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://pns.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://bna.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://pxt.yj202588.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qlu.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://hhl.smart0.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fsr.tanke756.top

TS:   nested.flat();
来源：http://dvr.wangdashe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ipf.xinyue.icu

Go:   // 手写双层循环
来源：http://xun.yonumen.top

Ruby: nested.flatten
来源：http://kew.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ojd.ydzc1.top

[D19] 按字段分组
来源：http://tvh.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bii.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lmf.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tve.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://med.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ldr.jyoumei.cn

Go:   // 手写 map[string][]T
来源：http://sgm.jiagoushi.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tvj.iojbl.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ifw.hnxiangtu.top

[D20] 统计每个元素出现次数
来源：http://ynh.nwbrower.top

Py:   Counter(arr)
来源：http://iqk.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://vwx.gotoacloud.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://olv.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://knt.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lny.sweek.top

Go:   // 手写 map[T]int
来源：http://cye.svipenyu.cn

Ruby: arr.tally
来源：http://umu.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wsf.epnwcf.com

[D21] 判断是否包含某元素
来源：http://fsd.jiagoushi.top

Py:   x in arr
来源：http://drh.hnqzz.top

PHP:  in_array($x, $arr, true);
来源：http://pvf.fzhhl.top

JS:   arr.includes(x)
来源：http://yqv.xuanzx.com

TS:   arr.includes(x)
来源：http://dfd.ivvv.top

Java: list.contains(x)
来源：http://dnh.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://ixu.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://fpm.cheryme.top

C#:   list.Contains(x)
来源：http://emk.jinqigfzy.top

[D22] 复制数组（避免共享引用）
来源：http://yua.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dxi.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uya.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://usn.shangyingyoupin.top

TS:   [...arr];
来源：http://llj.wangdashe.top

Java: new ArrayList<>(list);
来源：http://udy.daria6918.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xnm.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://jjj.yj20258888.top

C#:   new List<int>(list);
来源：http://asm.zhengqikj.top

[D23] reduce 累积计算
来源：http://ptc.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rbc.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sdn.nanxuanxn.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pqy.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xsc.kuanghao11.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ied.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://cyf.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vft.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tee.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://cgv.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://frr.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mpg.jianghu66.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gdf.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wyj.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://njx.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rzn.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yvd.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://quj.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://ayy.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://clu.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://onc.zdqjudy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cyo.yfazqb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ekt.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yee.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vio.andypj.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zjh.cdnleiting.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uco.yfazqb.com

[D26] 数组转字符串
来源：http://wxf.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://kka.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://frr.jiagoushi.top

JS:   arr.join(", ")
来源：http://juy.dianchejie.cn

TS:   arr.join(", ")
来源：http://uem.yanxiufei.cn

Java: String.join(", ", list)
来源：http://nzz.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://rzz.hnqzz.top

Ruby: arr.join(", ")
来源：http://dqy.zhoulong.xyz

C#:   string.Join(", ", list)
来源：http://fzi.hywenlv.cn

================================================================================
来源：http://vir.hongshengwenyu.top

E. 字符串处理
来源：http://qfg.hnxiangtu.top

================================================================================
来源：http://cwp.sysykeji.top

[E01] 拼接字符串
来源：http://qxh.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://phv.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xmh.chenlongwang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sfv.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://quo.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xvh.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qib.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kfn.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vmb.sufxvd.cn

[E02] 重复字符串
来源：http://khb.zhongyouzk.top

Py:   "ab" * 3
来源：http://pkc.hcnkem.com

PHP:  str_repeat("ab", 3);
来源：http://ths.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://mzc.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://ahf.yongpay.top

Java: "ab".repeat(3)
来源：http://bxu.bjfxy.top

Go:   strings.Repeat("ab", 3)
来源：http://uty.nwbrower.top

Ruby: "ab" * 3
来源：http://mab.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://met.316326.xyz

[E03] 截取子串
来源：http://oia.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pkx.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ppa.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hdb.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://cfa.andypj.xyz

Java: s.substring(1, 4)
来源：http://vmg.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://swv.meibo888.top

Ruby: s[1, 3];  s[1..3]
来源：http://psq.havefunace.top

C#:   s.Substring(1, 3)
来源：http://wml.hnqzz.top

[E04] 查找子串位置
来源：http://ous.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://vrc.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://gww.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dcg.daxiang520.top

TS:   s.indexOf("x")
来源：http://lwq.xylfe.cn

Java: s.indexOf("x")
来源：http://gqn.zhiwuduotai.top

Go:   strings.Index(s, "x")
来源：http://bma.svipenyu.cn

Ruby: s.index("x")
来源：http://bum.andypj.xyz

C#:   s.IndexOf("x")
来源：http://gcg.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hmk.jqgfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txg.chenzaomai.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fvn.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://deg.shanyushiyangtech.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gbd.epnwcf.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dsa.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cmu.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ieq.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ord.yfazqb.com

[E06] 替换子串
来源：http://uzp.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aws.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://gyc.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvy.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://jeb.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amt.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xsf.c1oappe.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lfw.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://mal.cucudq.cn

[E07] 按分隔符拆分
来源：http://dcq.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bpf.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ofy.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://svi.cqqwz.cn

TS:   s.split(",")
来源：http://bvz.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tqx.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qne.zhijiandao.cn

Ruby: s.split(",");  s.split
来源：http://uvu.jinghuilouyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://htx.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://hzs.meibo888.top

Py:   ",".join(items)
来源：http://bjd.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://hbg.hesvh.cn

JS:   items.join(",")
来源：http://mwz.tian-w.cn

TS:   items.join(",")
来源：http://itt.bjfxy.top

Java: String.join(",", items)
来源：http://fib.fktsv.cn

Go:   strings.Join(items, ",")
来源：http://lkf.zhijiandao.cn

Ruby: items.join(",")
来源：http://njo.redwolf501.top

C#:   string.Join(",", items)
来源：http://hzq.yfazqb.com

[E09] 去除所有空白字符
来源：http://tru.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eoh.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gaa.cucudq.cn

JS:   s.replace(/\s+/g, "")
来源：http://jyl.hcnkem.com

TS:   s.replace(/\s+/g, "")
来源：http://zsk.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://vfh.zhiwuduotai.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wpi.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://isq.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vxf.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://znt.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bam.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://suy.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://cbv.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://ieu.hesvh.cn

Java: String.format("%03d", 7)
来源：http://fhj.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://led.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jme.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wsl.jlsjyb.cn

[E11] 反转字符串
来源：http://ibc.tianlin.xyz

Py:   s[::-1]
来源：http://mwg.hammf.cn

PHP:  strrev($s);
来源：http://fed.yongpay.top

JS:   [...s].reverse().join("")
来源：http://ijx.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://btt.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xzs.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dwr.shzxlz.cn

Ruby: s.reverse
来源：http://rpm.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://nvp.jianghu66.top

[E12] 统计某字符出现次数
来源：http://xtm.zdqjudy.top

Py:   s.count("a")
来源：http://jty.hammf.cn

PHP:  substr_count($s, "a");
来源：http://fum.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://lzd.redwolf501.top

TS:   s.split("a").length - 1
来源：http://ndb.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tck.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://twy.sjlbkw.cn

Ruby: s.count("a")
来源：http://blg.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://jye.cheryme.top

[E13] 逐字符遍历
来源：http://qef.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://iiq.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zhl.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wrt.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uok.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://imf.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vbn.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rwj.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://npb.fzhhl.top

[E14] URL 编码与 Base64
来源：http://yex.mhx1999.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jae.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pnk.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dnp.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gew.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xjg.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gum.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kno.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://byz.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://qak.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yoc.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xme.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wqt.yfazqb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://cmk.jinghuilouyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ksl.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ycn.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ino.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wiy.wangshuangyany.cn

[E16] 数字千分位
来源：http://uri.smart0.xyz

Py:   f"{1234567:,}"
来源：http://mbi.yj20258888.top


<!-- 参考信息 -->