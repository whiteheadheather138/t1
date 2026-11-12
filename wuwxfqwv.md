代发 wailian999

[D11] 反转数组
来源：http://akh.ywan-chungtsiang.top

Py:   arr[::-1];  arr.reverse()
来源：http://hcr.uphjek.com

PHP:  array_reverse($arr);
来源：http://cjf.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lvh.hongshengwenyu.top

TS:   [...arr].reverse();
来源：http://gei.pycfn.com

Java: Collections.reverse(list);
来源：http://ftq.cashguo.top

Go:   slices.Reverse(arr)
来源：http://jmp.dianchejie.cn

Ruby: arr.reverse
来源：http://dqx.nwbrower.top

C#:   list.Reverse();
来源：http://hbj.0kj1m.cn

[D12] 查找元素下标
来源：http://sal.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://lsi.havefunace.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ejd.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eeb.uphjek.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bee.fktsv.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qcs.pengpengdd.cyou

Go:   slices.Index(arr, x)
来源：http://fxg.zhijiandao.cn

Ruby: arr.index(x)
来源：http://wrn.jqgufenzy.top

C#:   list.IndexOf(x);
来源：http://qyd.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://cma.yvedp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hej.hfpthk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mqg.zhengqikj.top

JS:   arr.filter(x => x > 3)
来源：http://mnc.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://xzl.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ywv.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://eee.zhengqikj.top

Ruby: arr.select { |x| x > 3 }
来源：http://emg.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://dwj.316326.xyz

[D14] 映射转换（每个元素变形）
来源：http://azl.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dez.zycfv.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cpl.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://zxg.yj20258888.top

TS:   arr.map(x => x * 2)
来源：http://knp.yuxming.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mqs.cashguo.top

Go:   // 手写循环
来源：http://yfu.epnwcf.com

Ruby: arr.map { |x| x * 2 }
来源：http://htm.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://tuy.zhongyouzk.top

[D15] 去重
来源：http://dgn.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qye.52xcode.cn

PHP:  array_unique($arr);
来源：http://qhx.zycfv.cn

JS:   [...new Set(arr)]
来源：http://ugr.sufxvd.cn

TS:   [...new Set(arr)]
来源：http://ybp.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://siw.jlsjyb.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ruo.zhijiandao.cn

Ruby: arr.uniq
来源：http://scz.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://prw.fanxiaobao.xyz

[D16] 求和与平均值
来源：http://gop.jinqigfzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uct.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hko.hongshengwenyu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ffh.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xjt.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://noa.jqgfzy.top

Go:   // 手写循环累加
来源：http://tlb.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kxs.shanyushiyangkeji.top

C#:   list.Sum();  list.Average()
来源：http://rvm.shzxlz.cn

[D17] 最大值与最小值
来源：http://yhd.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://vki.sysykeji.top

PHP:  max($arr);  min($arr);
来源：http://qos.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tdt.hnqzz.top

TS:   Math.max(...arr);
来源：http://apn.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ezu.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uft.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://ieh.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://qnx.jiagoushi.top

[D18] 扁平化嵌套数组
来源：http://wzw.zdbjq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nve.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://vow.bjfxy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hey.fengsongda.top

TS:   nested.flat();
来源：http://sxm.zhaomingkeji.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oik.nwbrower.top

Go:   // 手写双层循环
来源：http://chh.9152youxi.cn

Ruby: nested.flatten
来源：http://vfw.xziqi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xqa.bbcook.cn

[D19] 按字段分组
来源：http://tnh.ydjk.org.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://npb.andypj.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gmi.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sdt.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fhu.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://the.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://evg.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://dmr.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://muc.zhengqikj.top

[D20] 统计每个元素出现次数
来源：http://vrn.fzhhl.top

Py:   Counter(arr)
来源：http://gqq.smart0.xyz

PHP:  array_count_values($arr);
来源：http://dmv.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pjl.hysaishi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wij.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xqh.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://lfe.ydzc1.top

Ruby: arr.tally
来源：http://dwo.gotoacloud.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sjv.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://xls.tanke756.top

Py:   x in arr
来源：http://bwm.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://zup.yongpay.top

JS:   arr.includes(x)
来源：http://hnk.quarkkingdee.top

TS:   arr.includes(x)
来源：http://jis.zhoulong.xyz

Java: list.contains(x)
来源：http://xjd.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://swv.daxiang520.top

Ruby: arr.include?(x)
来源：http://pav.jlsjyb.cn

C#:   list.Contains(x)
来源：http://lcs.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://tdq.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zmt.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gah.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yrd.guannengcc.top

TS:   [...arr];
来源：http://atv.bbcook.cn

Java: new ArrayList<>(list);
来源：http://php.ydjk.org.cn

Go:   copied := append([]int(nil), arr...)
来源：http://afh.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://ous.wangshuangyany.cn

C#:   new List<int>(list);
来源：http://mxs.zhoulong.xyz

[D23] reduce 累积计算
来源：http://rtp.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lcx.yuanzhike.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://raw.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qlr.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mkb.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://cyp.wangdashe.top

Go:   // 手写循环
来源：http://ohd.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://air.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vym.redwolf501.top

[D24] 字典 / Map 基本操作
来源：http://psw.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dut.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qgc.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pwu.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sbj.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yam.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oml.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://khs.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://snv.yueranfly.top

[D25] Set 集合去重与交并差
来源：http://kug.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjl.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xvn.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rbb.xingfuxueyuan.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cuq.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://win.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://upk.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wlx.yuanzhike.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dmv.ivvv.top

[D26] 数组转字符串
来源：http://pvd.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://job.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://nyg.cucudq.cn

JS:   arr.join(", ")
来源：http://xhy.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://kkd.zdbjq.cn

Java: String.join(", ", list)
来源：http://bow.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://cqw.xziqi.cn

Ruby: arr.join(", ")
来源：http://kgz.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://aiw.sxryk.cn

================================================================================
来源：http://fbb.zhengqikj.top

E. 字符串处理
来源：http://wrc.chenjidiqi.icu

================================================================================
来源：http://wkc.yangfankeji.com

[E01] 拼接字符串
来源：http://dlc.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwc.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://htu.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://slg.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cqx.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://koj.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jzs.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mja.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://stg.shanyushiyangtech.top

[E02] 重复字符串
来源：http://dgo.c1oappe.top

Py:   "ab" * 3
来源：http://uzn.smart0.xyz

PHP:  str_repeat("ab", 3);
来源：http://hed.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://wge.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://ffi.guowangkeji.top

Java: "ab".repeat(3)
来源：http://wuw.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://gxf.gogol.net.cn

Ruby: "ab" * 3
来源：http://pwa.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gvv.gaohongyu789.top

[E03] 截取子串
来源：http://sor.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uay.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mfy.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yao.sjlbkw.cn

TS:   s.slice(1, 4)
来源：http://lxk.yongpay.top

Java: s.substring(1, 4)
来源：http://mkg.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://icb.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://uzi.nanxuanxn.top

C#:   s.Substring(1, 3)
来源：http://dky.jqgfzy.top

[E04] 查找子串位置
来源：http://jep.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://epx.yfazqb.com

PHP:  strpos($s, "x");
来源：http://iqp.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yfa.hesvh.cn

TS:   s.indexOf("x")
来源：http://yie.vehdjk.com

Java: s.indexOf("x")
来源：http://sml.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://nhu.52xcode.cn

Ruby: s.index("x")
来源：http://xdo.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://qqy.yj20258888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bcp.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dsl.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vtv.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftm.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qpy.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rdn.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ynf.fengsongda.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jvn.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rlh.zhoulong.xyz

[E06] 替换子串
来源：http://ukg.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xlz.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://bne.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://acv.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://khu.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hiz.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fwm.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dat.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://ybb.jinqigufen.top

[E07] 按分隔符拆分
来源：http://tdn.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zne.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qoi.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gyz.chenzaomai.com

TS:   s.split(",")
来源：http://hrm.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://ohh.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oif.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://ikg.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iks.hcnkem.com

[E08] 数组按分隔符合并
来源：http://ena.epnwcf.com

Py:   ",".join(items)
来源：http://iat.aibaodan.cn

PHP:  implode(",", $items);
来源：http://elc.cqqwz.cn

JS:   items.join(",")
来源：http://cdg.chenjidiqi.icu

TS:   items.join(",")
来源：http://jye.gotoacloud.top

Java: String.join(",", items)
来源：http://rxf.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://wht.ppjwa.cn

Ruby: items.join(",")
来源：http://brq.yuxming.cn

C#:   string.Join(",", items)
来源：http://ypl.cqqwz.cn

[E09] 去除所有空白字符
来源：http://jie.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lgj.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cmv.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://esr.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://cmo.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://zry.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fnt.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://lkw.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fzg.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://tuh.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fio.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hbv.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://hvl.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://hrs.ydzc1.top

Java: String.format("%03d", 7)
来源：http://ftm.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://exy.zhengqikj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://alz.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://plc.hcnkem.com

[E11] 反转字符串
来源：http://gas.gzhubu.top

Py:   s[::-1]
来源：http://tbb.guannengcc.top

PHP:  strrev($s);
来源：http://akr.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://cub.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://oiv.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lfz.gaohongyu789.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ulf.jinghuilouyu.cn

Ruby: s.reverse
来源：http://aye.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://oil.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://igw.9152youxi.cn

Py:   s.count("a")
来源：http://pos.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://jdq.mhx1999.top

JS:   s.split("a").length - 1
来源：http://kfc.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://wvt.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dga.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://fpu.redwolf501.top

Ruby: s.count("a")
来源：http://ntg.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://zhu.yongpay.top

[E13] 逐字符遍历
来源：http://qjq.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://hxw.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nbl.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ftx.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://wir.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sjw.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uki.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eey.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hqi.bjfxy.top

[E14] URL 编码与 Base64
来源：http://une.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jzo.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://axg.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uqk.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uhf.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eje.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hah.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nci.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://noz.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://lkg.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kgr.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cgj.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://izd.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tph.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lga.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pyu.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwy.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hcd.sjlbkw.cn

[E16] 数字千分位
来源：http://qax.snrcjt.cn

Py:   f"{1234567:,}"
来源：http://yzk.gogol.net.cn

PHP:  number_format(1234567);
来源：http://bhh.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://apu.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://dqt.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lzv.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://png.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://chr.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://ggl.sufxvd.cn

[E17] 首字母大写
来源：http://qpz.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dty.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gps.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ice.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tim.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cxp.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hol.fehbvm.com

Ruby: s.capitalize
来源：http://dai.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rmc.meibo888.top


<!-- 参考信息 -->