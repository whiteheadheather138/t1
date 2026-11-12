代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://ngy.bjfxy.top

TS:   [...a, ...b];
来源：http://gnx.daxiang520.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bmj.bjfxy.top

Go:   append(a, b...)
来源：http://dxn.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://dct.316326.xyz

C#:   a.Concat(b).ToList()
来源：http://tli.jqgufenzy.top

[D09] 排序（升序）
来源：http://ebw.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://iof.xziqi.cn

PHP:  sort($arr);
来源：http://kaz.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pge.shanyushiyangkeji.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ojx.xinyue.icu

Java: Collections.sort(list);  list.sort(null);
来源：http://fan.sufxvd.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://psl.zdqjudy.top

Ruby: arr.sort
来源：http://wxl.shangyingyoupin.top

C#:   list.Sort();
来源：http://txb.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gok.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jjv.daria6918.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uzb.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aby.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tbj.iojbl.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nal.vehdjk.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dwe.hcnkem.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lrq.gotoacloud.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gff.kuanghao11.cn

[D11] 反转数组
来源：http://pqx.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://hnw.gotoacloud.top

PHP:  array_reverse($arr);
来源：http://swb.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://orv.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://ria.birdmap.top

Java: Collections.reverse(list);
来源：http://pay.daria6918.cn

Go:   slices.Reverse(arr)
来源：http://nvp.feifeiyinyue.top

Ruby: arr.reverse
来源：http://bzw.aibaodan.cn

C#:   list.Reverse();
来源：http://gtf.svipenyu.cn

[D12] 查找元素下标
来源：http://ozd.wangdashe.top

Py:   arr.index(x);  x in arr
来源：http://ukz.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jxa.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dmv.quarkkingdee.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pvm.shanyushiyangkeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ntn.vqdsnc.cn

Go:   slices.Index(arr, x)
来源：http://vft.mhx1999.top

Ruby: arr.index(x)
来源：http://toe.c1oappe.top

C#:   list.IndexOf(x);
来源：http://lzy.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://ijc.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lmx.sufxvd.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ivw.iojbl.cn

JS:   arr.filter(x => x > 3)
来源：http://vhm.fzhhl.top

TS:   arr.filter(x => x > 3)
来源：http://nya.pengpengdd.cyou

Java: list.stream().filter(x -> x > 3).toList()
来源：http://omu.yanxiufei.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://stl.zhaomingkeji.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://jet.yanxiufei.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rfc.chenlongwang.top

[D14] 映射转换（每个元素变形）
来源：http://xgc.gotoacloud.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bmc.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nyg.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://ved.vqdsnc.cn

TS:   arr.map(x => x * 2)
来源：http://ika.wangshuangyany.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lib.fanxiaobao.xyz

Go:   // 手写循环
来源：http://cac.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://ajw.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iin.yueranfly.top

[D15] 去重
来源：http://cid.quarkkingdee.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kct.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://lql.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://vni.dianchejie.cn

TS:   [...new Set(arr)]
来源：http://qai.zycfv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hnf.sysykeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://yup.chenzaomai.com

Ruby: arr.uniq
来源：http://xrv.havefunace.top

C#:   list.Distinct().ToList()
来源：http://rqo.mhx1999.top

[D16] 求和与平均值
来源：http://zae.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xra.mhx1999.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wmm.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wqn.ybcxt.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ekt.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xpl.aibaodan.cn

Go:   // 手写循环累加
来源：http://cjt.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kep.epnwcf.com

C#:   list.Sum();  list.Average()
来源：http://nwi.tanke756.top

[D17] 最大值与最小值
来源：http://vid.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://ryl.cheryme.top

PHP:  max($arr);  min($arr);
来源：http://owp.hongshengwenyu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baf.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://zsh.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kpz.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hnq.sweek.top

Ruby: arr.max;  arr.min
来源：http://xzy.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://ocs.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://har.sweek.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eje.yvedp.cn

PHP:  array_merge(...$nested);
来源：http://zkn.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pcu.0kj1m.cn

TS:   nested.flat();
来源：http://loo.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ceo.316326.xyz

Go:   // 手写双层循环
来源：http://dhv.fengsongda.top

Ruby: nested.flatten
来源：http://blf.feifeiyinyue.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gim.yueranfly.top

[D19] 按字段分组
来源：http://jiw.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vlo.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yil.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wvv.zhixingplan.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ubm.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iam.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://qfx.yangfankeji.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://xdy.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jcv.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://mlk.gogol.net.cn

Py:   Counter(arr)
来源：http://dnd.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://zxa.guannengcc.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hye.wangdashe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mtm.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hep.pycfn.com

Go:   // 手写 map[T]int
来源：http://gtl.sxryk.cn

Ruby: arr.tally
来源：http://bhn.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bzo.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://xrb.chenlongwang.top

Py:   x in arr
来源：http://bmp.jyoumei.cn

PHP:  in_array($x, $arr, true);
来源：http://idc.zhongyouzk.top

JS:   arr.includes(x)
来源：http://lzp.svipenyu.cn

TS:   arr.includes(x)
来源：http://wah.cdnleiting.top

Java: list.contains(x)
来源：http://nxy.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://vvs.hesvh.cn

Ruby: arr.include?(x)
来源：http://tdu.chenlongwang.top

C#:   list.Contains(x)
来源：http://iwm.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://tme.jinyuanbaomall.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ooe.zhaomingkeji.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lms.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tzw.cashguo.top

TS:   [...arr];
来源：http://pyj.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://gyo.yj202588.top

Go:   copied := append([]int(nil), arr...)
来源：http://nnb.yongpay.top

Ruby: arr.dup;  arr.clone
来源：http://bqf.cdnleiting.top

C#:   new List<int>(list);
来源：http://wfi.zhixingplan.top

[D23] reduce 累积计算
来源：http://ygq.aibaodan.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pby.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ift.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ony.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zzn.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tuc.epnwcf.com

Go:   // 手写循环
来源：http://vjk.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://crc.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ehv.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://ayk.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kdx.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tae.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kwo.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eoj.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kiw.zhaomingkeji.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lsp.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qtc.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zme.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://mwd.ydjk.org.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zto.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kpf.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ecc.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qdo.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zvq.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wih.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cym.ydjk.org.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://olk.snrcjt.cn

[D26] 数组转字符串
来源：http://pvj.yvedp.cn

Py:   ", ".join(map(str, arr))
来源：http://tbl.zycfv.cn

PHP:  implode(", ", $arr);
来源：http://yfl.xuetiantiany.cn

JS:   arr.join(", ")
来源：http://uil.jqgfzy.top

TS:   arr.join(", ")
来源：http://xei.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://dny.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://jgn.cashguo.top

Ruby: arr.join(", ")
来源：http://oxn.fengsongda.top

C#:   string.Join(", ", list)
来源：http://hol.ivvv.top

================================================================================
来源：http://obl.zdqjudy.top

E. 字符串处理
来源：http://cnh.zdqjudy.top

================================================================================
来源：http://gxq.yvedp.cn

[E01] 拼接字符串
来源：http://hos.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xgz.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tnw.birdmap.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajf.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ctz.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dzw.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vhk.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mdp.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bes.hammf.cn

[E02] 重复字符串
来源：http://fjg.9152youxi.cn

Py:   "ab" * 3
来源：http://zkx.bjfxy.top

PHP:  str_repeat("ab", 3);
来源：http://hjr.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://eaw.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://roj.gogol.net.cn

Java: "ab".repeat(3)
来源：http://ykq.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://dkh.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://ztx.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfg.hongshengwenyu.top

[E03] 截取子串
来源：http://ceh.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ryd.guowangkeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ktv.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rkk.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://dpf.316326.xyz

Java: s.substring(1, 4)
来源：http://ngy.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wgj.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://ldn.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://pii.guowangkeji.top

[E04] 查找子串位置
来源：http://tzm.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://kci.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://pyy.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gfz.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://owy.pycfn.com

Java: s.indexOf("x")
来源：http://tqf.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://sju.feifeiyinyue.top

Ruby: s.index("x")
来源：http://ynr.daxiang520.top

C#:   s.IndexOf("x")
来源：http://csx.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kxj.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qez.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://amv.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cli.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cvm.tianlin.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bmg.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hlb.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vqt.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ksl.yuanzhike.top

[E06] 替换子串
来源：http://cnq.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oru.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ela.c1oappe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cxn.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://nvf.daria6918.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hhg.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://khb.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jso.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://tfj.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://xcu.andypj.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://acc.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ecx.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kqi.feifeiyinyue.top

TS:   s.split(",")
来源：http://xuq.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://ycr.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tsn.316326.xyz

Ruby: s.split(",");  s.split
来源：http://yji.yfazqb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zgc.yj20258.top

[E08] 数组按分隔符合并
来源：http://drb.zhaomingkeji.xyz

Py:   ",".join(items)
来源：http://qkj.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://ixl.jyoumei.cn

JS:   items.join(",")
来源：http://ywz.zycfv.cn

TS:   items.join(",")
来源：http://txh.ctjpmb.com

Java: String.join(",", items)
来源：http://upn.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://utf.52xcode.cn

Ruby: items.join(",")
来源：http://ibf.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://ojq.bjfxy.top

[E09] 去除所有空白字符
来源：http://ssd.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://swi.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pto.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://egm.chenjidiqi.icu

TS:   s.replace(/\s+/g, "")
来源：http://pjh.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://dpo.chenjidiqi.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://jqt.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://xik.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zic.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://rwb.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gvj.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tvd.quarkkingdee.top

JS:   "7".padStart(3, "0")
来源：http://ihr.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://awz.aizwys.cn

Java: String.format("%03d", 7)
来源：http://vvr.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://clw.hnxiangtu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xhn.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kot.epnwcf.com

[E11] 反转字符串
来源：http://ghw.hnqzz.top

Py:   s[::-1]
来源：http://vig.ctjpmb.com

PHP:  strrev($s);
来源：http://qxp.shuidangran.top

JS:   [...s].reverse().join("")
来源：http://ohs.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://vyh.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://anf.fengsongda.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukj.hongshengwenyu.top

Ruby: s.reverse
来源：http://nug.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://qts.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://dum.jyoumei.cn

Py:   s.count("a")
来源：http://xjw.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://pln.jianghu66.top

JS:   s.split("a").length - 1
来源：http://arj.yfazqb.com

TS:   s.split("a").length - 1
来源：http://mtc.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qui.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://ntz.epnwcf.com

Ruby: s.count("a")
来源：http://nuc.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://fda.nwbrower.top

[E13] 逐字符遍历
来源：http://rgi.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://szn.jqgufenzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jjl.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vor.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://irj.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uaq.shanyushiyangtech.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ajl.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://maz.xingfuxueyuan.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fjj.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://cvr.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ikt.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fhm.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nhv.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hbq.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pop.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pvt.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ujh.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://acy.ydzc1.top

[E15] HTML 转义 / 反转义
来源：http://yau.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://avu.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vee.tianlin.xyz


<!-- 参考信息 -->