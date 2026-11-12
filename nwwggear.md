代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bwf.bjfxy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://osd.meibo888.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hlx.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://sli.yanxiufei.cn

Ruby: arr.index(x)
来源：http://hyt.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://eob.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://aqx.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blt.hywenlv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gyb.zhaomingkeji.xyz

JS:   arr.filter(x => x > 3)
来源：http://mpa.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://ero.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://muf.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bqf.dashuyun.cn

Ruby: arr.select { |x| x > 3 }
来源：http://byy.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://grp.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://bii.hammf.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lah.cashguo.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ljw.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://msq.zdqjudy.top

TS:   arr.map(x => x * 2)
来源：http://vmf.aizwys.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eok.nanxinkj.top

Go:   // 手写循环
来源：http://yjd.gaohongyu789.top

Ruby: arr.map { |x| x * 2 }
来源：http://fng.yj202588.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dvk.jyoumei.cn

[D15] 去重
来源：http://khr.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gsd.hesvh.cn

PHP:  array_unique($arr);
来源：http://ziq.meibo888.top

JS:   [...new Set(arr)]
来源：http://zsd.xuanzx.com

TS:   [...new Set(arr)]
来源：http://pvg.hnxiangtu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jen.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://qst.sysykeji.top

Ruby: arr.uniq
来源：http://pib.dashuyun.cn

C#:   list.Distinct().ToList()
来源：http://zye.dashuyun.cn

[D16] 求和与平均值
来源：http://fkt.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fuc.sxryk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cyj.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xmz.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://txs.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fvi.zhengqikj.top

Go:   // 手写循环累加
来源：http://vyj.sweek.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vxn.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://ark.zhengqikj.top

[D17] 最大值与最小值
来源：http://ltf.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://phn.yanxiufei.cn

PHP:  max($arr);  min($arr);
来源：http://uzi.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://non.cdnleiting.top

TS:   Math.max(...arr);
来源：http://hng.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qdl.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cxk.zhixingplan.top

Ruby: arr.max;  arr.min
来源：http://gbm.zhaomingkeji.xyz

C#:   list.Max();  list.Min()
来源：http://pfp.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://wvz.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ceb.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://zpa.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwv.tanke756.top

TS:   nested.flat();
来源：http://wkv.meibo888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nae.yongpay.top

Go:   // 手写双层循环
来源：http://lvq.nanxinkj.top

Ruby: nested.flatten
来源：http://uyp.iojbl.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://soc.zhongyouzk.top

[D19] 按字段分组
来源：http://oyv.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sct.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aiw.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://egu.nanxinkj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aun.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pxz.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://bkn.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpv.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uvn.pycfn.com

[D20] 统计每个元素出现次数
来源：http://nlq.sweek.top

Py:   Counter(arr)
来源：http://jgo.cashguo.top

PHP:  array_count_values($arr);
来源：http://bwl.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gvw.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bjq.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rgl.yonumen.top

Go:   // 手写 map[T]int
来源：http://jsj.fktsv.cn

Ruby: arr.tally
来源：http://mab.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ask.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://eyz.nanxinkj.top

Py:   x in arr
来源：http://cnx.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://yfh.hfpthk.cn

JS:   arr.includes(x)
来源：http://lzf.xinyue.icu

TS:   arr.includes(x)
来源：http://jed.haohaochexian.top

Java: list.contains(x)
来源：http://gkq.svipenyu.cn

Go:   slices.Contains(arr, x)
来源：http://nqb.chenzaomai.com

Ruby: arr.include?(x)
来源：http://hae.chenzaomai.com

C#:   list.Contains(x)
来源：http://gey.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://yre.xingfuxueyuan.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ihy.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aib.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://seb.nanxinkj.top

TS:   [...arr];
来源：http://ica.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://svx.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://ejr.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://sbo.birdmap.top

C#:   new List<int>(list);
来源：http://wgm.andypj.xyz

[D23] reduce 累积计算
来源：http://wju.dianchejie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lcn.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sjj.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jmj.tarul.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kod.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xfz.hnqzz.top

Go:   // 手写循环
来源：http://puf.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qpz.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rjs.hongshengwenyu.top

[D24] 字典 / Map 基本操作
来源：http://ufz.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lky.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ego.tarul.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lce.cqqwz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bux.tian-w.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nvh.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ajq.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ois.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dun.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://qpj.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fbj.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ody.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jnn.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pbf.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oaq.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dvk.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wjm.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aga.jinqigfzy.top

[D26] 数组转字符串
来源：http://ckh.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://dde.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://sqh.gotoacloud.top

JS:   arr.join(", ")
来源：http://jvi.zhiwuduotai.top

TS:   arr.join(", ")
来源：http://ney.ehwqpu.com

Java: String.join(", ", list)
来源：http://cos.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://mgx.uphjek.com

Ruby: arr.join(", ")
来源：http://lnb.hnqzz.top

C#:   string.Join(", ", list)
来源：http://ele.ivvv.top

================================================================================
来源：http://ufa.daria6918.cn

E. 字符串处理
来源：http://nwk.jiagoushi.top

================================================================================
来源：http://ivq.chenjidiqi.icu

[E01] 拼接字符串
来源：http://tfp.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ohv.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fin.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ano.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ckq.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ctt.jinyuanbaomall.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fjx.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://exf.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bnr.zdqjudy.top

[E02] 重复字符串
来源：http://nvv.gotoacloud.top

Py:   "ab" * 3
来源：http://qxx.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://kfb.nanxinkj.top

JS:   "ab".repeat(3)
来源：http://wmn.cheryme.top

TS:   "ab".repeat(3)
来源：http://jni.ydjk.org.cn

Java: "ab".repeat(3)
来源：http://uge.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://zes.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://vhh.jqgufenzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wnk.vqdsnc.cn

[E03] 截取子串
来源：http://kib.c1oappe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vlg.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rbz.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://doe.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://vyn.sysykeji.top

Java: s.substring(1, 4)
来源：http://xye.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bda.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jvq.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://mzr.bbcook.cn

[E04] 查找子串位置
来源：http://brk.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://klu.gaohongyu789.top

PHP:  strpos($s, "x");
来源：http://nmi.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cfb.ybcxt.top

TS:   s.indexOf("x")
来源：http://tlz.9152youxi.cn

Java: s.indexOf("x")
来源：http://wqu.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://ywn.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://zai.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://yxc.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://hxk.sxryk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://frm.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pft.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sbi.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://grr.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ggk.fzhhl.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jke.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nww.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xcv.meibo888.top

[E06] 替换子串
来源：http://pvw.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kxy.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://ssg.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://noq.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://rat.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hxh.yueranfly.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fga.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rwp.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://xdw.ctjpmb.com

[E07] 按分隔符拆分
来源：http://ycg.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xrx.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yvg.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://eao.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://wrk.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://hxj.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uni.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://ard.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://woz.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://lvr.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://mff.yj20258.top

PHP:  implode(",", $items);
来源：http://adt.fehbvm.com

JS:   items.join(",")
来源：http://mzc.havefunace.top

TS:   items.join(",")
来源：http://smn.smart0.xyz

Java: String.join(",", items)
来源：http://lxq.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://fyh.haohaochexian.top

Ruby: items.join(",")
来源：http://hqz.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://apd.svipenyu.cn

[E09] 去除所有空白字符
来源：http://hsa.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctr.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jgv.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://ksm.cdnleiting.top

TS:   s.replace(/\s+/g, "")
来源：http://wwi.nwbrower.top

Java: s.replaceAll("\\s+", "")
来源：http://bpw.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rwm.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://mow.yueranfly.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dfe.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://hrb.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kwn.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kdt.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://qyy.fzhhl.top

TS:   "7".padStart(3, "0")
来源：http://nmn.316326.xyz

Java: String.format("%03d", 7)
来源：http://cel.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://yqc.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pxi.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aps.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://tre.chenjidiqi.icu

Py:   s[::-1]
来源：http://wyq.yuanzhike.top

PHP:  strrev($s);
来源：http://flh.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://vvf.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://fzp.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tsc.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eyy.hywenlv.cn

Ruby: s.reverse
来源：http://lll.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://wfw.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://tty.xinyue.icu

Py:   s.count("a")
来源：http://tbt.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://cgx.yonumen.top

JS:   s.split("a").length - 1
来源：http://zhv.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://plj.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kqm.sweek.top

Go:   strings.Count(s, "a")
来源：http://lrm.yj20258888.top

Ruby: s.count("a")
来源：http://tlr.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://hgs.hnxiangtu.top

[E13] 逐字符遍历
来源：http://ygz.quarkkingdee.top

Py:   for ch in s: print(ch)
来源：http://pjc.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fqs.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ecb.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://flq.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jal.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cgp.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pcp.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nsc.andypj.xyz

[E14] URL 编码与 Base64
来源：http://iqb.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://krb.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qbe.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xxn.jyoumei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uhr.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pba.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://psg.ywan-chungtsiang.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tae.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mpa.sweek.top

[E15] HTML 转义 / 反转义
来源：http://ebu.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://alx.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fle.guowangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mli.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qtd.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pid.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://euw.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ppq.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uyu.jqgufenzy.top

[E16] 数字千分位
来源：http://hpx.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://cwp.bbcook.cn

PHP:  number_format(1234567);
来源：http://uiv.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wgg.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nvt.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://azz.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vyb.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fed.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://ott.cheryme.top

[E17] 首字母大写
来源：http://eef.fengsongda.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ewe.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ewu.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hqh.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tuy.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xhn.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hzv.daxiang520.top

Ruby: s.capitalize
来源：http://xdo.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://acx.ctjpmb.com

[E18] 模板占位符替换
来源：http://iwc.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bsv.fengsongda.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://byg.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://why.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wnt.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ozu.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fua.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sth.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xjc.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://xge.xuanzx.com

Py:   s.splitlines()
来源：http://sga.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mnt.zhiwuduotai.top


<!-- 参考信息 -->