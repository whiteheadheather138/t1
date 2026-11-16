代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pqu.fzhhl.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmh.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://krz.bbcook.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uta.feifeiyinyue.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pci.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bep.yj202588.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tnj.zhongyouzk.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://reg.hammf.cn

[D11] 反转数组
来源：http://rdp.hnxiangtu.top

Py:   arr[::-1];  arr.reverse()
来源：http://tmr.mhx1999.top

PHP:  array_reverse($arr);
来源：http://jrj.nanxinkj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rsq.nwbrower.top

TS:   [...arr].reverse();
来源：http://cpk.dianchejie.cn

Java: Collections.reverse(list);
来源：http://jvc.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://mva.zhengqikj.top

Ruby: arr.reverse
来源：http://xdr.jqgufenzy.top

C#:   list.Reverse();
来源：http://frd.chenzaomai.com

[D12] 查找元素下标
来源：http://ixu.epnwcf.com

Py:   arr.index(x);  x in arr
来源：http://cjj.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rzd.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mol.vqdsnc.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bia.zhaomingkeji.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://irw.nanxinkj.top

Go:   slices.Index(arr, x)
来源：http://xyu.havefunace.top

Ruby: arr.index(x)
来源：http://jni.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://mmj.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://yte.fanxiaobao.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ngj.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ayg.yuxming.cn

JS:   arr.filter(x => x > 3)
来源：http://flx.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://tbh.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://peh.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wcf.aibaodan.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hnu.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://wff.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://wpc.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://smg.yj20258.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://quf.fengsongda.top

JS:   arr.map(x => x * 2)
来源：http://die.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://inw.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ljp.ydzc1.top

Go:   // 手写循环
来源：http://eck.yonumen.top

Ruby: arr.map { |x| x * 2 }
来源：http://dpy.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://pfq.jinghuilouyu.cn

[D15] 去重
来源：http://ebo.yj20258.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wxf.aibaodan.cn

PHP:  array_unique($arr);
来源：http://hmw.svipenyu.cn

JS:   [...new Set(arr)]
来源：http://qdv.haohaochexian.top

TS:   [...new Set(arr)]
来源：http://vfb.ctjpmb.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ldl.zhengqikj.top

Go:   // 用 map[T]struct{} 手写
来源：http://lvm.ivvv.top

Ruby: arr.uniq
来源：http://mpu.zhixingplan.top

C#:   list.Distinct().ToList()
来源：http://kfh.gzhubu.top

[D16] 求和与平均值
来源：http://tvq.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aro.tian-w.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dgb.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sem.jianghu66.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ddh.xuetiantiany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://oiu.sufxvd.cn

Go:   // 手写循环累加
来源：http://eyi.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wgi.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://vcw.snrcjt.cn

[D17] 最大值与最小值
来源：http://ded.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://aph.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://spr.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ydg.hammf.cn

TS:   Math.max(...arr);
来源：http://yah.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ycl.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xlw.andypj.xyz

Ruby: arr.max;  arr.min
来源：http://iju.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://kcl.cdnleiting.top

[D18] 扁平化嵌套数组
来源：http://iun.birdmap.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mqv.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://gna.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ruc.yj202588.top

TS:   nested.flat();
来源：http://ryb.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wly.yj202588.top

Go:   // 手写双层循环
来源：http://ccw.hammf.cn

Ruby: nested.flatten
来源：http://blf.nwbrower.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://xek.tianlin.xyz

[D19] 按字段分组
来源：http://mxr.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sev.jinqigufen.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gau.redwolf501.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rlf.jyoumei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jyp.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wfb.ybcxt.top

Go:   // 手写 map[string][]T
来源：http://ses.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zvm.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nkd.daria6918.cn

[D20] 统计每个元素出现次数
来源：http://moi.yj20258888.top

Py:   Counter(arr)
来源：http://ver.52xcode.cn

PHP:  array_count_values($arr);
来源：http://cgp.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://etj.gogol.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jxb.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qzq.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://ekv.dashuyun.cn

Ruby: arr.tally
来源：http://fgd.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vdd.zycfv.cn

[D21] 判断是否包含某元素
来源：http://pas.shzxlz.cn

Py:   x in arr
来源：http://uct.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://qsk.zhijiandao.cn

JS:   arr.includes(x)
来源：http://azb.hcnkem.com

TS:   arr.includes(x)
来源：http://xqj.nwbrower.top

Java: list.contains(x)
来源：http://nbp.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://bis.sufxvd.cn

Ruby: arr.include?(x)
来源：http://dcy.ybcxt.top

C#:   list.Contains(x)
来源：http://sjz.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://gkk.ybcxt.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://beu.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xyd.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xik.hysaishi.cn

TS:   [...arr];
来源：http://ipv.hfpthk.cn

Java: new ArrayList<>(list);
来源：http://rao.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vxi.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://eae.tian-w.cn

C#:   new List<int>(list);
来源：http://rru.shangyingyoupin.top

[D23] reduce 累积计算
来源：http://sfr.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hlx.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yis.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hvo.hywenlv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zez.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://owk.daria6918.cn

Go:   // 手写循环
来源：http://gck.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dxt.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jam.guowangkeji.top

[D24] 字典 / Map 基本操作
来源：http://cob.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iac.sxryk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xdh.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sxu.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kov.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aco.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://opa.gotoacloud.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://euv.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nae.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://kbt.zhoulong.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lkq.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gnx.tanke756.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gev.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qaj.9152youxi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iyr.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://afy.chenjidiqi.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yjh.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yma.ctjpmb.com

[D26] 数组转字符串
来源：http://qqw.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://smd.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://dcj.xziqi.cn

JS:   arr.join(", ")
来源：http://hgj.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://mrx.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://ozq.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://zyq.c1oappe.top

Ruby: arr.join(", ")
来源：http://vnq.wangdashe.top

C#:   string.Join(", ", list)
来源：http://ymh.316326.xyz

================================================================================
来源：http://woh.pycfn.com

E. 字符串处理
来源：http://iak.dianchejie.cn

================================================================================
来源：http://lyf.daxiang520.top

[E01] 拼接字符串
来源：http://tqg.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iip.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jdj.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gtf.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://psh.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tzb.yueranfly.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lgf.pengpengdd.cyou

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hnv.fehbvm.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vcu.yvedp.cn

[E02] 重复字符串
来源：http://qcw.aibaodan.cn

Py:   "ab" * 3
来源：http://ycc.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://ckv.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://uyc.jianghu66.top

TS:   "ab".repeat(3)
来源：http://nll.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://syp.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://jja.zhengqikj.top

Ruby: "ab" * 3
来源：http://ose.zdqjudy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wee.dashuyun.cn

[E03] 截取子串
来源：http://ytn.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lsg.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zqn.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zxt.hcnkem.com

TS:   s.slice(1, 4)
来源：http://ikz.haohaochexian.top

Java: s.substring(1, 4)
来源：http://yjb.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://icu.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://xyi.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://ezf.jqgfzy.top

[E04] 查找子串位置
来源：http://emf.cqqwz.cn

Py:   s.find("x");  s.index("x")
来源：http://cwj.yuanzhike.top

PHP:  strpos($s, "x");
来源：http://qmh.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nav.guowangkeji.top

TS:   s.indexOf("x")
来源：http://pin.yuxming.cn

Java: s.indexOf("x")
来源：http://mdg.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://lyj.iojbl.cn

Ruby: s.index("x")
来源：http://khk.bjfxy.top

C#:   s.IndexOf("x")
来源：http://orb.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pug.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qey.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqt.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://shv.yuanzhike.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xth.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vdk.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gfs.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://thd.kuanghao11.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fdq.zhiwuduotai.top

[E06] 替换子串
来源：http://gfr.yuanzhike.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vvj.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://ilk.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qvn.sjlbkw.cn

TS:   s.replaceAll("a", "b")
来源：http://bsw.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bra.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ujd.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xex.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://gkn.xziqi.cn

[E07] 按分隔符拆分
来源：http://zsb.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fyk.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uql.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ofl.aizwys.cn

TS:   s.split(",")
来源：http://ymw.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://zad.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://crd.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://dmi.yuxming.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qgy.aizwys.cn

[E08] 数组按分隔符合并
来源：http://udh.cdnleiting.top

Py:   ",".join(items)
来源：http://eri.havefunace.top

PHP:  implode(",", $items);
来源：http://dbj.sjlbkw.cn

JS:   items.join(",")
来源：http://wds.sweek.top

TS:   items.join(",")
来源：http://qpx.sjlbkw.cn

Java: String.join(",", items)
来源：http://vlx.yuxming.cn

Go:   strings.Join(items, ",")
来源：http://rxf.hfpthk.cn

Ruby: items.join(",")
来源：http://xby.cdnleiting.top

C#:   string.Join(",", items)
来源：http://vbd.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://tnj.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tcn.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ssq.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://mfq.shzxlz.cn

TS:   s.replace(/\s+/g, "")
来源：http://ctx.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://vce.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rdr.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://dzl.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://suh.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://yfg.yuanzhike.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nml.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ery.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://ogu.ywan-chungtsiang.top

TS:   "7".padStart(3, "0")
来源：http://qmi.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://pul.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rcy.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dik.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bej.jinqigfzy.top

[E11] 反转字符串
来源：http://lde.jinqigfzy.top

Py:   s[::-1]
来源：http://boz.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://vls.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://ewi.hysaishi.cn

TS:   [...s].reverse().join("")
来源：http://acw.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fva.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qjz.jqgufenzy.top

Ruby: s.reverse
来源：http://gza.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://skr.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://wdr.bbcook.cn

Py:   s.count("a")
来源：http://jjj.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://wxv.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://nzy.yj20258.top

TS:   s.split("a").length - 1
来源：http://ktn.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://guu.cheryme.top

Go:   strings.Count(s, "a")
来源：http://cct.aibaodan.cn

Ruby: s.count("a")
来源：http://wgm.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://qxm.chenjidiqi.icu

[E13] 逐字符遍历
来源：http://rdi.uphjek.com

Py:   for ch in s: print(ch)
来源：http://oxj.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pgj.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ggf.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://mmf.sufxvd.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pvu.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jjb.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ooo.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vnw.yfazqb.com

[E14] URL 编码与 Base64
来源：http://jbd.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yrn.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zce.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hgt.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nne.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hry.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rnw.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lvy.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hog.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://env.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://toh.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://khq.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fvf.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dni.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rro.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rar.fzhhl.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cte.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://csn.sweek.top

[E16] 数字千分位
来源：http://odb.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://ebx.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://oej.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://gyb.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lwd.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tos.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oey.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wsd.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://zta.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://njd.cheryme.top


<!-- 参考信息 -->