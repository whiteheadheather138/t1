代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hkt.yj202588.top

TS:   [...a, ...b];
来源：http://snm.birdmap.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qie.zhengqikj.top

Go:   append(a, b...)
来源：http://nfz.yj20258.top

Ruby: a + b;  a.concat(b)
来源：http://jln.tian-w.cn

C#:   a.Concat(b).ToList()
来源：http://dqj.jqgfzy.top

[D09] 排序（升序）
来源：http://ocl.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://iud.vehdjk.com

PHP:  sort($arr);
来源：http://qsj.snrcjt.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://iox.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lqv.sweek.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xxn.zhaomingkeji.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jmp.xuetiantiany.cn

Ruby: arr.sort
来源：http://lfy.hongshengwenyu.top

C#:   list.Sort();
来源：http://mav.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fjb.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uwe.yanxiufei.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jak.vehdjk.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bau.xuetiantiany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hae.sweek.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bgf.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jyl.bbcook.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dyy.redwolf501.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dnk.vehdjk.com

[D11] 反转数组
来源：http://fcv.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://iwy.cqqwz.cn

PHP:  array_reverse($arr);
来源：http://lww.pycfn.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ekz.sweek.top

TS:   [...arr].reverse();
来源：http://abl.daxiang520.top

Java: Collections.reverse(list);
来源：http://gha.9152youxi.cn

Go:   slices.Reverse(arr)
来源：http://vkl.hongshengwenyu.top

Ruby: arr.reverse
来源：http://tdk.zhijiandao.cn

C#:   list.Reverse();
来源：http://gka.zhijiandao.cn

[D12] 查找元素下标
来源：http://pzo.hywenlv.cn

Py:   arr.index(x);  x in arr
来源：http://jwo.zdqjudy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ojv.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dfm.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bry.zhengqikj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eoo.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://zow.cheryme.top

Ruby: arr.index(x)
来源：http://ojh.52xcode.cn

C#:   list.IndexOf(x);
来源：http://evj.shangyingyoupin.top

[D13] 过滤（保留满足条件的）
来源：http://jvo.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bsd.ivvv.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sua.jinqigfzy.top

JS:   arr.filter(x => x > 3)
来源：http://wbb.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://ryu.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xnl.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpw.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ijq.fehbvm.com

C#:   list.Where(x => x > 3).ToList()
来源：http://pum.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://xci.havefunace.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wpr.ydjk.org.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ehx.316326.xyz

JS:   arr.map(x => x * 2)
来源：http://ftw.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://cte.gogol.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ajz.zhoulong.xyz

Go:   // 手写循环
来源：http://ala.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wac.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://dsq.yonumen.top

[D15] 去重
来源：http://ykx.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dun.tarul.cn

PHP:  array_unique($arr);
来源：http://dvp.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://idm.tarul.cn

TS:   [...new Set(arr)]
来源：http://ggr.jinqigfzy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ckv.cucudq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uou.jlsjyb.cn

Ruby: arr.uniq
来源：http://ooo.yj202588.top

C#:   list.Distinct().ToList()
来源：http://qsm.fehbvm.com

[D16] 求和与平均值
来源：http://hwf.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://viu.ivvv.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hjz.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tuf.chenlongwang.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sbd.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uab.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://tou.snrcjt.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dev.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://uvf.redwolf501.top

[D17] 最大值与最小值
来源：http://bya.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://obp.ehwqpu.com

PHP:  max($arr);  min($arr);
来源：http://xhw.tarul.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ayg.redwolf501.top

TS:   Math.max(...arr);
来源：http://sqg.mhx1999.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mth.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vxh.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://heq.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://vgu.pycfn.com

[D18] 扁平化嵌套数组
来源：http://dps.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yhu.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://fpl.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://akj.sweek.top

TS:   nested.flat();
来源：http://ual.sufxvd.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xaa.aibaodan.cn

Go:   // 手写双层循环
来源：http://vqs.daria6918.cn

Ruby: nested.flatten
来源：http://sas.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bce.iojbl.cn

[D19] 按字段分组
来源：http://svy.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mih.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oou.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oke.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ffn.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://odm.hammf.cn

Go:   // 手写 map[string][]T
来源：http://gaa.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://equ.yongpay.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bds.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://cmh.0kj1m.cn

Py:   Counter(arr)
来源：http://dmo.sweek.top

PHP:  array_count_values($arr);
来源：http://akx.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awd.chenzaomai.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qym.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gzx.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://uza.jinghuilouyu.cn

Ruby: arr.tally
来源：http://uok.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ufq.meibo888.top

[D21] 判断是否包含某元素
来源：http://vop.9152youxi.cn

Py:   x in arr
来源：http://nsx.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://uph.hammf.cn

JS:   arr.includes(x)
来源：http://hio.guannengcc.top

TS:   arr.includes(x)
来源：http://lgd.ydjk.org.cn

Java: list.contains(x)
来源：http://ntd.zdqjudy.top

Go:   slices.Contains(arr, x)
来源：http://ubr.52xcode.cn

Ruby: arr.include?(x)
来源：http://eqn.havefunace.top

C#:   list.Contains(x)
来源：http://hqc.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://uvy.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lgz.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jvk.aibaodan.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qzl.yongpay.top

TS:   [...arr];
来源：http://ohk.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://lsp.chenzaomai.com

Go:   copied := append([]int(nil), arr...)
来源：http://xtt.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://arb.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://ufy.smart0.xyz

[D23] reduce 累积计算
来源：http://syg.zhengqikj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wcj.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ivc.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://puy.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xyd.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qwi.feifeiyinyue.top

Go:   // 手写循环
来源：http://ltb.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tzr.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wqs.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://lvu.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xsp.0kj1m.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jwx.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vkh.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://poi.yongpay.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jdc.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yfx.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vaz.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pnu.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://llm.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xya.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wxy.daria6918.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hbp.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rnx.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nur.sweek.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kqa.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zpz.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qru.zhaomingkeji.xyz

[D26] 数组转字符串
来源：http://rae.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://zcs.yj20258.top

PHP:  implode(", ", $arr);
来源：http://ayp.gotoacloud.top

JS:   arr.join(", ")
来源：http://zbc.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://kas.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://rlx.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://rly.sysykeji.top

Ruby: arr.join(", ")
来源：http://sry.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://bfr.birdmap.top

================================================================================
来源：http://nin.uphjek.com

E. 字符串处理
来源：http://ehe.fanxiaobao.xyz

================================================================================
来源：http://twv.andypj.xyz

[E01] 拼接字符串
来源：http://pse.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://agx.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vnt.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fbo.svipenyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmo.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kfw.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://duo.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fes.shanyushiyangkeji.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pjs.jyoumei.cn

[E02] 重复字符串
来源：http://yvc.jiagoushi.top

Py:   "ab" * 3
来源：http://pfp.ppjwa.cn

PHP:  str_repeat("ab", 3);
来源：http://zig.shuidangran.top

JS:   "ab".repeat(3)
来源：http://whb.fehbvm.com

TS:   "ab".repeat(3)
来源：http://oss.9152youxi.cn

Java: "ab".repeat(3)
来源：http://lic.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://sne.jianghu66.top

Ruby: "ab" * 3
来源：http://few.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ftd.hammf.cn

[E03] 截取子串
来源：http://vip.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lta.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lfu.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uos.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://tcp.ctjpmb.com

Java: s.substring(1, 4)
来源：http://evw.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bli.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://rci.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://tud.pengpengdd.cyou

[E04] 查找子串位置
来源：http://qkh.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://bkv.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://jfj.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tor.sufxvd.cn

TS:   s.indexOf("x")
来源：http://gci.yueranfly.top

Java: s.indexOf("x")
来源：http://qna.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://xif.ppjwa.cn

Ruby: s.index("x")
来源：http://cyd.andypj.xyz

C#:   s.IndexOf("x")
来源：http://sop.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://src.guowangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oco.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jtz.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://whq.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bsw.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yzy.tanke756.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uad.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bim.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vyj.gotoacloud.top

[E06] 替换子串
来源：http://rkq.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aml.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://wbj.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lqb.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://dhc.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blz.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gqx.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ypm.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://cqj.wangdashe.top

[E07] 按分隔符拆分
来源：http://lsh.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pbh.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qxr.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yko.feifeiyinyue.top

TS:   s.split(",")
来源：http://zcs.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://kdr.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ucg.tanke756.top

Ruby: s.split(",");  s.split
来源：http://xvp.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://way.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://jba.mhx1999.top

Py:   ",".join(items)
来源：http://nyh.cucudq.cn

PHP:  implode(",", $items);
来源：http://mkv.yj202588.top

JS:   items.join(",")
来源：http://uyw.52xcode.cn

TS:   items.join(",")
来源：http://dgb.jianghu66.top

Java: String.join(",", items)
来源：http://sec.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://hjv.tianlin.xyz

Ruby: items.join(",")
来源：http://znw.tian-w.cn

C#:   string.Join(",", items)
来源：http://sdn.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://hsz.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tvl.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nfs.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://yix.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://qcz.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://zlq.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qmd.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://sxo.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wab.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://qeb.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qmq.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hxa.sweek.top

JS:   "7".padStart(3, "0")
来源：http://eff.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://hoq.vqdsnc.cn

Java: String.format("%03d", 7)
来源：http://riw.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://thy.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fzv.daria6918.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rrs.sufxvd.cn

[E11] 反转字符串
来源：http://fdx.svipenyu.cn

Py:   s[::-1]
来源：http://btu.yonumen.top

PHP:  strrev($s);
来源：http://bnq.tarul.cn

JS:   [...s].reverse().join("")
来源：http://ffq.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://ydl.quarkkingdee.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nvy.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hen.yueranfly.top

Ruby: s.reverse
来源：http://tkm.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bnd.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://ogx.wangdashe.top

Py:   s.count("a")
来源：http://poi.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://ohq.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://oqq.sweek.top

TS:   s.split("a").length - 1
来源：http://xyl.hnxiangtu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xzd.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://gwb.bbcook.cn

Ruby: s.count("a")
来源：http://huh.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://swo.guowangkeji.top

[E13] 逐字符遍历
来源：http://uzi.tanke756.top

Py:   for ch in s: print(ch)
来源：http://ybv.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ili.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://sqh.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gxq.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rus.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tws.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sok.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://die.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://uju.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iey.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pfj.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wlb.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yor.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wwd.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bas.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jln.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jqk.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://hto.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hji.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iyh.zhengqikj.top


<!-- 参考信息 -->