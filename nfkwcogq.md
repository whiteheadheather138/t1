代发 wailian999

[D07] 切片 / 取子数组
来源：http://cwc.jlsjyb.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kax.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://pnj.pengpengdd.cyou

JS:   arr.slice(1, 4);
来源：http://kzp.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://hlt.zycfv.cn

Java: list.subList(1, 4);
来源：http://yna.wangdashe.top

Go:   arr[1:4]
来源：http://qfn.ydjk.org.cn

Ruby: arr[1, 3]
来源：http://jtf.andypj.xyz

C#:   list.GetRange(1, 3);
来源：http://cxi.vehdjk.com

[D08] 合并两个数组
来源：http://gfj.xuetiantiany.cn

Py:   a + b;  a.extend(b)
来源：http://xrx.jqgfzy.top

PHP:  array_merge($a, $b);
来源：http://qlx.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://qdn.jinghuilouyu.cn

TS:   [...a, ...b];
来源：http://rdj.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tov.zycfv.cn

Go:   append(a, b...)
来源：http://ncg.hnxiangtu.top

Ruby: a + b;  a.concat(b)
来源：http://ryu.zhiwuduotai.top

C#:   a.Concat(b).ToList()
来源：http://yls.yfazqb.com

[D09] 排序（升序）
来源：http://frr.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://mkr.haohaochexian.top

PHP:  sort($arr);
来源：http://xkv.fktsv.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nrh.quarkkingdee.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mwh.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ero.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rih.tanke756.top

Ruby: arr.sort
来源：http://grc.xuetiantiany.cn

C#:   list.Sort();
来源：http://oni.jinyuanbaomall.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ktu.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ygv.sweek.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ckt.zycfv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yew.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://idn.ppjwa.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://imw.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qcx.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wbh.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eqe.sjlbkw.cn

[D11] 反转数组
来源：http://nos.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mxe.0kj1m.cn

PHP:  array_reverse($arr);
来源：http://wkn.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://esa.andypj.xyz

TS:   [...arr].reverse();
来源：http://vex.hongshengwenyu.top

Java: Collections.reverse(list);
来源：http://opk.cheryme.top

Go:   slices.Reverse(arr)
来源：http://amn.andypj.xyz

Ruby: arr.reverse
来源：http://ccu.snrcjt.cn

C#:   list.Reverse();
来源：http://izs.ydjk.org.cn

[D12] 查找元素下标
来源：http://hse.guannengcc.top

Py:   arr.index(x);  x in arr
来源：http://tcy.wangshuangyany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tvm.yuanzhike.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zer.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hzi.jinyuanbaomall.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nhd.xinyue.icu

Go:   slices.Index(arr, x)
来源：http://kdy.jianghu66.top

Ruby: arr.index(x)
来源：http://zhj.redwolf501.top

C#:   list.IndexOf(x);
来源：http://yhz.jyoumei.cn

[D13] 过滤（保留满足条件的）
来源：http://xzk.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wnj.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hfd.tianlin.xyz

JS:   arr.filter(x => x > 3)
来源：http://bmh.cdnleiting.top

TS:   arr.filter(x => x > 3)
来源：http://nxo.pycfn.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://utd.0kj1m.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ntx.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://xmb.fktsv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aae.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://twg.yuanzhike.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pdi.sysykeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zfu.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://ffu.hnqzz.top

TS:   arr.map(x => x * 2)
来源：http://qkt.zhiwuduotai.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mmz.jyoumei.cn

Go:   // 手写循环
来源：http://oob.tian-w.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jtz.jyoumei.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://owo.aibaodan.cn

[D15] 去重
来源：http://cum.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jts.pengpengdd.cyou

PHP:  array_unique($arr);
来源：http://hpm.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://cpb.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://hac.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cih.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gni.kuanghao11.cn

Ruby: arr.uniq
来源：http://opc.sweek.top

C#:   list.Distinct().ToList()
来源：http://wsg.bjfxy.top

[D16] 求和与平均值
来源：http://phm.jyoumei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hgj.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tjl.wangshuangyany.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dar.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kmz.c1oappe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cwx.svipenyu.cn

Go:   // 手写循环累加
来源：http://uae.vehdjk.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wln.xylfe.cn

C#:   list.Sum();  list.Average()
来源：http://eph.xuanzx.com

[D17] 最大值与最小值
来源：http://yjx.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://qez.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://ueg.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iqj.chenjidiqi.icu

TS:   Math.max(...arr);
来源：http://njk.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ogl.tianlin.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tdb.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://kzd.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://ojd.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://eqc.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zuc.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://zox.jinyuanbaomall.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://csc.dianchejie.cn

TS:   nested.flat();
来源：http://rof.jinghuilouyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ynt.yvedp.cn

Go:   // 手写双层循环
来源：http://xeg.0kj1m.cn

Ruby: nested.flatten
来源：http://kkg.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vwd.xuetiantiany.cn

[D19] 按字段分组
来源：http://apm.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wld.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qro.yongpay.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hqp.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vqk.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jqf.hfpthk.cn

Go:   // 手写 map[string][]T
来源：http://clq.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mlb.daxiang520.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ctj.meibo888.top

[D20] 统计每个元素出现次数
来源：http://lis.wangshuangyany.cn

Py:   Counter(arr)
来源：http://wkb.hnqzz.top

PHP:  array_count_values($arr);
来源：http://jyq.hywenlv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uls.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npa.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ubf.zycfv.cn

Go:   // 手写 map[T]int
来源：http://sas.quarkkingdee.top

Ruby: arr.tally
来源：http://noh.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jmh.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://ist.cashguo.top

Py:   x in arr
来源：http://dpx.xingfuxueyuan.xyz

PHP:  in_array($x, $arr, true);
来源：http://ptf.zhoulong.xyz

JS:   arr.includes(x)
来源：http://vqe.bbcook.cn

TS:   arr.includes(x)
来源：http://fxi.c1oappe.top

Java: list.contains(x)
来源：http://lus.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://mcl.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://vbc.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://lff.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://jgg.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ful.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yqo.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xzk.sufxvd.cn

TS:   [...arr];
来源：http://oyk.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://etl.redwolf501.top

Go:   copied := append([]int(nil), arr...)
来源：http://pza.quarkkingdee.top

Ruby: arr.dup;  arr.clone
来源：http://lbp.meibo888.top

C#:   new List<int>(list);
来源：http://jjs.hcnkem.com

[D23] reduce 累积计算
来源：http://lzl.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://awl.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fmi.epnwcf.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dod.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xjl.zdbjq.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pgu.zycfv.cn

Go:   // 手写循环
来源：http://ool.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://emk.52xcode.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://thb.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://qvw.fanxiaobao.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hsu.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aul.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dxz.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xsi.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ysb.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vym.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uqf.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uxp.havefunace.top

[D25] Set 集合去重与交并差
来源：http://sqg.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yck.mhx1999.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ywp.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://snu.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ubj.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bok.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jrf.shzxlz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://quw.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xbu.yanxiufei.cn

[D26] 数组转字符串
来源：http://zjl.hcnkem.com

Py:   ", ".join(map(str, arr))
来源：http://gji.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://ofq.sysykeji.top

JS:   arr.join(", ")
来源：http://xen.snrcjt.cn

TS:   arr.join(", ")
来源：http://qxy.hywenlv.cn

Java: String.join(", ", list)
来源：http://wnm.jinghuilouyu.cn

Go:   strings.Join(strs, ", ")
来源：http://kzo.snrcjt.cn

Ruby: arr.join(", ")
来源：http://gij.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://qax.jinghuilouyu.cn

================================================================================
来源：http://bqx.hnxiangtu.top

E. 字符串处理
来源：http://env.chenzaomai.com

================================================================================
来源：http://fen.pengpengdd.cyou

[E01] 拼接字符串
来源：http://peu.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lhv.nwbrower.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vdx.jlsjyb.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://emz.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kzi.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bdp.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://keh.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://agk.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rce.9152youxi.cn

[E02] 重复字符串
来源：http://adg.jiagoushi.top

Py:   "ab" * 3
来源：http://hez.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://mcy.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://gcs.xziqi.cn

TS:   "ab".repeat(3)
来源：http://zaz.shuidangran.top

Java: "ab".repeat(3)
来源：http://ipn.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://bqk.vqdsnc.cn

Ruby: "ab" * 3
来源：http://xxq.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hzc.fzhhl.top

[E03] 截取子串
来源：http://rgr.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ydm.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wqn.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yjg.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://ruc.yongpay.top

Java: s.substring(1, 4)
来源：http://lee.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sxc.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://cgo.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://orh.zdbjq.cn

[E04] 查找子串位置
来源：http://vgc.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://ldo.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://aec.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nzv.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://xxt.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://qgg.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://gri.zhaomingkeji.xyz

Ruby: s.index("x")
来源：http://emv.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://nrl.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rba.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://doy.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tvq.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://otj.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ebo.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kbh.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mwh.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lkw.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oqo.tanke756.top

[E06] 替换子串
来源：http://qqm.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ofl.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dbt.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ugq.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://hmq.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fca.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kug.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ljp.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://wzc.aibaodan.cn

[E07] 按分隔符拆分
来源：http://jiy.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vyn.fehbvm.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cex.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jyy.zdqjudy.top

TS:   s.split(",")
来源：http://plx.yangfankeji.com

Java: s.split(",");  s.split("\\s+")
来源：http://odt.vehdjk.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qfs.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://cxt.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rxi.fehbvm.com

[E08] 数组按分隔符合并
来源：http://xpp.nwbrower.top

Py:   ",".join(items)
来源：http://hcw.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://lvw.chenlongwang.top

JS:   items.join(",")
来源：http://pks.zhaomingkeji.xyz

TS:   items.join(",")
来源：http://aok.sufxvd.cn

Java: String.join(",", items)
来源：http://yeu.yj20258.top

Go:   strings.Join(items, ",")
来源：http://pco.yfazqb.com

Ruby: items.join(",")
来源：http://zpj.aizwys.cn

C#:   string.Join(",", items)
来源：http://yzc.nwbrower.top

[E09] 去除所有空白字符
来源：http://ezb.yvedp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aux.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qby.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://zpy.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://tez.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://qji.bjfxy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lxs.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ehg.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cxz.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://gif.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kli.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pug.jiagoushi.top

JS:   "7".padStart(3, "0")
来源：http://utv.sysykeji.top

TS:   "7".padStart(3, "0")
来源：http://rfa.havefunace.top

Java: String.format("%03d", 7)
来源：http://odf.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nne.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yuz.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://his.daria6918.cn

[E11] 反转字符串
来源：http://zmn.guowangkeji.top

Py:   s[::-1]
来源：http://ecc.havefunace.top

PHP:  strrev($s);
来源：http://fef.meibo888.top

JS:   [...s].reverse().join("")
来源：http://ktm.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://syn.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mrv.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://oat.smart0.xyz

Ruby: s.reverse
来源：http://gtc.wangshuangyany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://emn.mhx1999.top

[E12] 统计某字符出现次数
来源：http://evg.sweek.top

Py:   s.count("a")
来源：http://oxz.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://iqz.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://mte.52xcode.cn

TS:   s.split("a").length - 1
来源：http://alk.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sar.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://jrh.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://gty.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://zdc.chenzaomai.com

[E13] 逐字符遍历
来源：http://rks.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://zrj.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qwq.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mdx.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cgn.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tbw.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xcm.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hnm.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xup.iojbl.cn


<!-- 参考信息 -->