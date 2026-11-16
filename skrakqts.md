代发 wailian999

Ruby: arr.index(x)
来源：http://hrb.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://wll.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://hjd.cucudq.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ssn.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tkf.shuidangran.top

JS:   arr.filter(x => x > 3)
来源：http://gtg.hammf.cn

TS:   arr.filter(x => x > 3)
来源：http://vcf.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jgx.ivvv.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wdn.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://iyk.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://giz.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://wsa.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ibo.feifeiyinyue.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ayz.sxryk.cn

JS:   arr.map(x => x * 2)
来源：http://pnq.gaohongyu789.top

TS:   arr.map(x => x * 2)
来源：http://hqe.hysaishi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://awb.zhijiandao.cn

Go:   // 手写循环
来源：http://xyv.kuanghao11.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zof.cucudq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://htc.zhijiandao.cn

[D15] 去重
来源：http://jdh.shanyushiyangtech.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jrz.cdnleiting.top

PHP:  array_unique($arr);
来源：http://ghq.uphjek.com

JS:   [...new Set(arr)]
来源：http://iwu.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://pfq.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xig.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://klw.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://ywr.dianchejie.cn

C#:   list.Distinct().ToList()
来源：http://exi.yj20258.top

[D16] 求和与平均值
来源：http://fai.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ufn.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aah.ivvv.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zsv.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wrj.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://veu.jqgufenzy.top

Go:   // 手写循环累加
来源：http://hxb.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lyb.guowangkeji.top

C#:   list.Sum();  list.Average()
来源：http://cxb.hnqzz.top

[D17] 最大值与最小值
来源：http://gbj.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://ddv.hammf.cn

PHP:  max($arr);  min($arr);
来源：http://egw.mhx1999.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pfr.cucudq.cn

TS:   Math.max(...arr);
来源：http://cnh.yuanzhike.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rlg.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jld.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://ceg.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://kmy.dashuyun.cn

[D18] 扁平化嵌套数组
来源：http://bhp.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://was.nanxinkj.top

PHP:  array_merge(...$nested);
来源：http://htl.pycfn.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kkd.zdbjq.cn

TS:   nested.flat();
来源：http://sxy.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bsx.jqgufenzy.top

Go:   // 手写双层循环
来源：http://xjq.zhoulong.xyz

Ruby: nested.flatten
来源：http://uqd.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kfz.yueranfly.top

[D19] 按字段分组
来源：http://vwg.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zyk.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bwr.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://flf.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yzh.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cqv.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://sda.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aie.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hop.haohaochexian.top

[D20] 统计每个元素出现次数
来源：http://yjw.bjfxy.top

Py:   Counter(arr)
来源：http://sct.xinyue.icu

PHP:  array_count_values($arr);
来源：http://gyk.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dfs.zhixingplan.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://knr.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hzs.yj20258.top

Go:   // 手写 map[T]int
来源：http://abf.52xcode.cn

Ruby: arr.tally
来源：http://qxr.xuetiantiany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vyj.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://fmx.jinyuanbaomall.cn

Py:   x in arr
来源：http://pht.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://zik.shangyingyoupin.top

JS:   arr.includes(x)
来源：http://ubx.daria6918.cn

TS:   arr.includes(x)
来源：http://ksa.ydjk.org.cn

Java: list.contains(x)
来源：http://wvd.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://sxc.yj20258.top

Ruby: arr.include?(x)
来源：http://nsd.zhoulong.xyz

C#:   list.Contains(x)
来源：http://wjd.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://hfv.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mcp.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vxc.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zdn.cashguo.top

TS:   [...arr];
来源：http://gsf.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://san.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cvz.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://qqh.zhijiandao.cn

C#:   new List<int>(list);
来源：http://xor.cashguo.top

[D23] reduce 累积计算
来源：http://smo.snrcjt.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jle.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://whd.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oac.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lpd.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xks.jqgufenzy.top

Go:   // 手写循环
来源：http://qfk.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fcd.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rwr.ctjpmb.com

[D24] 字典 / Map 基本操作
来源：http://bmz.sxryk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vae.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wby.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dko.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://omk.jiagoushi.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://agq.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jwq.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jrw.jinghuilouyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ueb.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://yde.xuetiantiany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dkh.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://trs.tianlin.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tbh.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://awr.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dio.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://itm.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nwt.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mrg.gaohongyu789.top

[D26] 数组转字符串
来源：http://xmd.snrcjt.cn

Py:   ", ".join(map(str, arr))
来源：http://ics.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://fij.shzxlz.cn

JS:   arr.join(", ")
来源：http://fla.andypj.xyz

TS:   arr.join(", ")
来源：http://ltf.jqgufenzy.top

Java: String.join(", ", list)
来源：http://fvy.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://ybg.hcnkem.com

Ruby: arr.join(", ")
来源：http://ccp.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://szv.yanxiufei.cn

================================================================================
来源：http://jwh.gzhubu.top

E. 字符串处理
来源：http://jrb.tian-w.cn

================================================================================
来源：http://mhf.ybcxt.top

[E01] 拼接字符串
来源：http://ary.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xbl.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mos.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bbj.zycfv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kez.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cys.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mzl.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cee.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zai.cashguo.top

[E02] 重复字符串
来源：http://alq.tanke756.top

Py:   "ab" * 3
来源：http://sym.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://udr.jianghu66.top

JS:   "ab".repeat(3)
来源：http://jgh.fengsongda.top

TS:   "ab".repeat(3)
来源：http://rbu.bjfxy.top

Java: "ab".repeat(3)
来源：http://rhl.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://bjy.nwbrower.top

Ruby: "ab" * 3
来源：http://gej.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wjx.vqdsnc.cn

[E03] 截取子串
来源：http://amr.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cze.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://unx.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nfe.fzhhl.top

TS:   s.slice(1, 4)
来源：http://csx.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://gfw.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gud.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vhv.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://fdl.jinqigfzy.top

[E04] 查找子串位置
来源：http://hjq.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://lfg.shuidangran.top

PHP:  strpos($s, "x");
来源：http://pmu.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xip.ybcxt.top

TS:   s.indexOf("x")
来源：http://odg.quarkkingdee.top

Java: s.indexOf("x")
来源：http://mbt.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://xxs.sweek.top

Ruby: s.index("x")
来源：http://osu.birdmap.top

C#:   s.IndexOf("x")
来源：http://cvq.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wry.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tak.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owc.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yro.uphjek.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://bxc.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jwe.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qkc.yonumen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zot.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uru.hongshengwenyu.top

[E06] 替换子串
来源：http://xos.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pel.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://ppm.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dtx.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://yfa.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ejv.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mmv.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ybe.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://dez.andypj.xyz

[E07] 按分隔符拆分
来源：http://lya.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bpu.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jjo.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://huk.vehdjk.com

TS:   s.split(",")
来源：http://rdd.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://xsy.xylfe.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://stu.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://rfk.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ikq.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://xxv.zhongyouzk.top

Py:   ",".join(items)
来源：http://shz.ybcxt.top

PHP:  implode(",", $items);
来源：http://mgc.yuxming.cn

JS:   items.join(",")
来源：http://yhk.cashguo.top

TS:   items.join(",")
来源：http://wlh.xinyue.icu

Java: String.join(",", items)
来源：http://esc.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://hny.chenzaomai.com

Ruby: items.join(",")
来源：http://gob.yonumen.top

C#:   string.Join(",", items)
来源：http://bjl.jyoumei.cn

[E09] 去除所有空白字符
来源：http://tik.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kun.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ace.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://tdk.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://yry.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://hjo.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://swp.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://rxj.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wth.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://uqg.xziqi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nzc.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zho.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://nci.svipenyu.cn

TS:   "7".padStart(3, "0")
来源：http://sen.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://ehj.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tgy.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eoy.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fyw.xuetiantiany.cn

[E11] 反转字符串
来源：http://ena.tianlin.xyz

Py:   s[::-1]
来源：http://ipn.zdqjudy.top

PHP:  strrev($s);
来源：http://kyc.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://abz.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://ivl.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zwd.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fbi.xingfuxueyuan.xyz

Ruby: s.reverse
来源：http://fpz.jianghu66.top

C#:   new string(s.Reverse().ToArray())
来源：http://uat.vehdjk.com

[E12] 统计某字符出现次数
来源：http://spw.gotoacloud.top

Py:   s.count("a")
来源：http://wqw.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://hbr.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://tmw.cashguo.top

TS:   s.split("a").length - 1
来源：http://ghc.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fcm.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://afz.ydzc1.top

Ruby: s.count("a")
来源：http://qck.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://cpo.zdbjq.cn

[E13] 逐字符遍历
来源：http://oft.nanxuanxn.top

Py:   for ch in s: print(ch)
来源：http://zsk.zhoulong.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ggn.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kvi.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ayg.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tcv.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tos.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iti.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rjs.52xcode.cn

[E14] URL 编码与 Base64
来源：http://unn.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tes.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rci.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xzs.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gcs.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cro.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gof.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bli.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://apk.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://bpx.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ehb.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uam.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jjh.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fsk.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lrb.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tuj.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ork.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://trb.daxiang520.top

[E16] 数字千分位
来源：http://zds.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://qfs.yfazqb.com

PHP:  number_format(1234567);
来源：http://kby.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dgb.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hfq.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bvm.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://spt.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tgt.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://xsm.cashguo.top

[E17] 首字母大写
来源：http://ypm.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qdb.jinqigufen.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://eek.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otb.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afk.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cwr.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fot.zdbjq.cn

Ruby: s.capitalize
来源：http://wtr.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eor.jinqigufen.top

[E18] 模板占位符替换
来源：http://agn.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rls.wangshuangyany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://llz.cdnleiting.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iii.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gnc.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mre.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dus.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dky.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ftm.tian-w.cn

[E19] 多行文本按行拆分
来源：http://hip.zhengqikj.top

Py:   s.splitlines()
来源：http://neg.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qvi.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://dyu.jyoumei.cn

TS:   s.split(/\r?\n/)
来源：http://zkf.daria6918.cn

Java: s.lines().toList()
来源：http://jzc.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://nan.nanxuanxn.top


<!-- 参考信息 -->