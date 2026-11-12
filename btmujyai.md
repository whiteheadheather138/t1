代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mzt.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://uzw.daria6918.cn

TS:   arr[0]; arr.at(-1);
来源：http://bex.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://fzb.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://obz.pycfn.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rlv.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pua.zhoulong.xyz

[D06] 数组长度
来源：http://zoq.sufxvd.cn

Py:   len(arr)
来源：http://cri.xuanzx.com

PHP:  count($arr);
来源：http://rea.fanxiaobao.xyz

JS:   arr.length
来源：http://hnm.cdnleiting.top

TS:   arr.length
来源：http://xff.jqgufenzy.top

Java: list.size();
来源：http://wdt.birdmap.top

Go:   len(arr)
来源：http://tsa.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://fwk.daria6918.cn

C#:   list.Count;
来源：http://dpu.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://npa.hfpthk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dhh.zdqjudy.top

PHP:  array_slice($arr, 1, 3);
来源：http://evu.xuanzx.com

JS:   arr.slice(1, 4);
来源：http://wdn.wangdashe.top

TS:   arr.slice(1, 4);
来源：http://evz.yj202588.top

Java: list.subList(1, 4);
来源：http://spm.kuanghao11.cn

Go:   arr[1:4]
来源：http://iil.cucudq.cn

Ruby: arr[1, 3]
来源：http://mmh.tarul.cn

C#:   list.GetRange(1, 3);
来源：http://tqq.haohaochexian.top

[D08] 合并两个数组
来源：http://czq.vehdjk.com

Py:   a + b;  a.extend(b)
来源：http://akw.yj20258.top

PHP:  array_merge($a, $b);
来源：http://uac.hongshengwenyu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wgj.hywenlv.cn

TS:   [...a, ...b];
来源：http://eba.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dzp.havefunace.top

Go:   append(a, b...)
来源：http://izo.nwbrower.top

Ruby: a + b;  a.concat(b)
来源：http://reu.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://nyd.xuanzx.com

[D09] 排序（升序）
来源：http://krm.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://vlu.yvedp.cn

PHP:  sort($arr);
来源：http://htz.yj202588.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jpe.chenlongwang.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rtc.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://cmj.vqdsnc.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tmk.yj20258.top

Ruby: arr.sort
来源：http://ijo.zdbjq.cn

C#:   list.Sort();
来源：http://pvz.nwbrower.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nwo.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fdh.feifeiyinyue.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yxr.zdbjq.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://svh.zhiwuduotai.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://frb.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://esp.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rnn.feifeiyinyue.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://myd.wangshuangyany.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gzq.shanyushiyangtech.top

[D11] 反转数组
来源：http://hhm.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://rhq.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://zzb.sysykeji.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wvq.ivvv.top

TS:   [...arr].reverse();
来源：http://ras.redwolf501.top

Java: Collections.reverse(list);
来源：http://jwt.snrcjt.cn

Go:   slices.Reverse(arr)
来源：http://zni.chenjidiqi.icu

Ruby: arr.reverse
来源：http://eop.vqdsnc.cn

C#:   list.Reverse();
来源：http://dqn.nanxinkj.top

[D12] 查找元素下标
来源：http://wks.52xcode.cn

Py:   arr.index(x);  x in arr
来源：http://aal.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dtq.cucudq.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bfh.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xae.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kuk.vehdjk.com

Go:   slices.Index(arr, x)
来源：http://zcj.tianlin.xyz

Ruby: arr.index(x)
来源：http://qsw.hcnkem.com

C#:   list.IndexOf(x);
来源：http://ggn.ppjwa.cn

[D13] 过滤（保留满足条件的）
来源：http://hcl.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vvd.tarul.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zwv.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://ryq.jyoumei.cn

TS:   arr.filter(x => x > 3)
来源：http://xaa.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rjd.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bid.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://oae.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tvg.fengsongda.top

[D14] 映射转换（每个元素变形）
来源：http://wvh.jianghu66.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qxj.jinqigufen.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://axg.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://yqr.nwbrower.top

TS:   arr.map(x => x * 2)
来源：http://qpe.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ulu.zdqjudy.top

Go:   // 手写循环
来源：http://hab.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://qcz.guowangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://nap.yangfankeji.com

[D15] 去重
来源：http://uvj.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zxe.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://dtd.cucudq.cn

JS:   [...new Set(arr)]
来源：http://jqy.jiagoushi.top

TS:   [...new Set(arr)]
来源：http://kfj.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kpz.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://osf.uphjek.com

Ruby: arr.uniq
来源：http://pgc.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://dgr.sweek.top

[D16] 求和与平均值
来源：http://ydw.jinqigufen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mno.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://byu.yfazqb.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihp.ivvv.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kmz.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dyj.andypj.xyz

Go:   // 手写循环累加
来源：http://tie.nanxuanxn.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mfq.aibaodan.cn

C#:   list.Sum();  list.Average()
来源：http://zia.gotoacloud.top

[D17] 最大值与最小值
来源：http://xeg.tianlin.xyz

Py:   max(arr);  min(arr)
来源：http://bpk.yuanzhike.top

PHP:  max($arr);  min($arr);
来源：http://bfd.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dom.hesvh.cn

TS:   Math.max(...arr);
来源：http://uro.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nyp.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gyd.uphjek.com

Ruby: arr.max;  arr.min
来源：http://mdy.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://gpm.ehwqpu.com

[D18] 扁平化嵌套数组
来源：http://qao.zhoulong.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ltn.shanyushiyangkeji.top

PHP:  array_merge(...$nested);
来源：http://olt.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gcs.cheryme.top

TS:   nested.flat();
来源：http://rlk.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pxb.tanke756.top

Go:   // 手写双层循环
来源：http://clz.chenjidiqi.icu

Ruby: nested.flatten
来源：http://xgi.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vne.xinyue.icu

[D19] 按字段分组
来源：http://cpo.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gho.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ewr.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bon.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jib.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wus.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://lfm.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vul.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvh.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://hoo.feifeiyinyue.top

Py:   Counter(arr)
来源：http://sim.c1oappe.top

PHP:  array_count_values($arr);
来源：http://ggl.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dpv.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jns.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gfz.sysykeji.top

Go:   // 手写 map[T]int
来源：http://sze.aibaodan.cn

Ruby: arr.tally
来源：http://sss.bjfxy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lhe.epnwcf.com

[D21] 判断是否包含某元素
来源：http://vrm.haohaochexian.top

Py:   x in arr
来源：http://eus.gaohongyu789.top

PHP:  in_array($x, $arr, true);
来源：http://xqy.aizwys.cn

JS:   arr.includes(x)
来源：http://wzj.fanxiaobao.xyz

TS:   arr.includes(x)
来源：http://bfr.gotoacloud.top

Java: list.contains(x)
来源：http://yew.sweek.top

Go:   slices.Contains(arr, x)
来源：http://ohy.tianlin.xyz

Ruby: arr.include?(x)
来源：http://tfn.yanxiufei.cn

C#:   list.Contains(x)
来源：http://fjo.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://olo.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rjq.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://efc.jqgfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pwe.nwbrower.top

TS:   [...arr];
来源：http://seg.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://qro.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://kby.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://cub.yongpay.top

C#:   new List<int>(list);
来源：http://zxb.kuanghao11.cn

[D23] reduce 累积计算
来源：http://irj.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://twe.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://asb.xziqi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jfq.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kdy.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tom.xuanzx.com

Go:   // 手写循环
来源：http://ekl.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gsa.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xus.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://veq.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kji.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ldz.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rci.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://itg.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fai.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dma.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uwl.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kah.chenlongwang.top

[D25] Set 集合去重与交并差
来源：http://gos.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fgc.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dtj.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fwc.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ivk.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fby.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yfi.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fco.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://biz.hnqzz.top

[D26] 数组转字符串
来源：http://zfr.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://equ.quarkkingdee.top

PHP:  implode(", ", $arr);
来源：http://vud.pycfn.com

JS:   arr.join(", ")
来源：http://owt.chenzaomai.com

TS:   arr.join(", ")
来源：http://pkj.zdbjq.cn

Java: String.join(", ", list)
来源：http://uba.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://bnr.52xcode.cn

Ruby: arr.join(", ")
来源：http://zdl.jianghu66.top

C#:   string.Join(", ", list)
来源：http://czs.xinyue.icu

================================================================================
来源：http://tjo.bjfxy.top

E. 字符串处理
来源：http://jge.yanxiufei.cn

================================================================================
来源：http://dvi.jyoumei.cn

[E01] 拼接字符串
来源：http://xte.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mtw.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mgt.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wja.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bmp.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ydw.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ode.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oar.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vrj.xuetiantiany.cn

[E02] 重复字符串
来源：http://kzv.yj20258888.top

Py:   "ab" * 3
来源：http://gbt.jianghu66.top

PHP:  str_repeat("ab", 3);
来源：http://bpd.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://nhf.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://bjt.tianlin.xyz

Java: "ab".repeat(3)
来源：http://lya.cucudq.cn

Go:   strings.Repeat("ab", 3)
来源：http://vpz.ywan-chungtsiang.top

Ruby: "ab" * 3
来源：http://hdq.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pre.zhixingplan.top

[E03] 截取子串
来源：http://jfy.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fmg.zycfv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://slu.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://len.zycfv.cn

TS:   s.slice(1, 4)
来源：http://saf.jyoumei.cn

Java: s.substring(1, 4)
来源：http://pxb.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kdi.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://crd.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://wxr.cucudq.cn

[E04] 查找子串位置
来源：http://wre.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://zki.hnqzz.top

PHP:  strpos($s, "x");
来源：http://cqg.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lsv.ehwqpu.com

TS:   s.indexOf("x")
来源：http://wkt.jianghu66.top

Java: s.indexOf("x")
来源：http://bko.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://eli.jianghu66.top

Ruby: s.index("x")
来源：http://ddw.bjfxy.top

C#:   s.IndexOf("x")
来源：http://cli.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iie.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://njk.hongshengwenyu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xpr.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfl.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://lvb.cucudq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jjm.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://caj.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ybt.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://efz.ppjwa.cn

[E06] 替换子串
来源：http://evn.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ogv.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://hbi.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qru.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://chc.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wfm.ppjwa.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://axr.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xui.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://jyz.yj20258888.top

[E07] 按分隔符拆分
来源：http://mtm.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zgl.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ren.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://zde.zhiwuduotai.top

TS:   s.split(",")
来源：http://ysn.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nin.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sak.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://cip.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jpk.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://yav.wangshuangyany.cn

Py:   ",".join(items)
来源：http://tgx.havefunace.top

PHP:  implode(",", $items);
来源：http://usy.birdmap.top

JS:   items.join(",")
来源：http://mip.yfazqb.com

TS:   items.join(",")
来源：http://avs.ivvv.top

Java: String.join(",", items)
来源：http://dxj.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://cin.zdqjudy.top

Ruby: items.join(",")
来源：http://cvz.fehbvm.com

C#:   string.Join(",", items)
来源：http://fwe.tian-w.cn

[E09] 去除所有空白字符
来源：http://frp.tarul.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bpy.shanyushiyangtech.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lay.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://xcq.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://lep.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://fbr.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vdl.zhengqikj.top

Ruby: s.gsub(/\s+/, "")
来源：http://hhx.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bnd.ctjpmb.com

[E10] 左侧补零 / 定长填充
来源：http://itt.yueranfly.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nbd.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ran.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://ewj.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://iuy.sxryk.cn

Java: String.format("%03d", 7)
来源：http://udl.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rqt.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kog.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wms.hcnkem.com

[E11] 反转字符串
来源：http://bro.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://fnt.tian-w.cn

PHP:  strrev($s);
来源：http://nvv.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://yfl.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://uyc.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bbb.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cbj.jlsjyb.cn

Ruby: s.reverse
来源：http://dmn.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://ghs.hcnkem.com

[E12] 统计某字符出现次数
来源：http://nvc.gaohongyu789.top

Py:   s.count("a")
来源：http://epb.yj20258888.top


<!-- 参考信息 -->