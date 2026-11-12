代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hep.jqgfzy.top

Ruby: arr.select { |x| x > 3 }
来源：http://qdp.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uys.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://tat.jyoumei.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gly.chenzaomai.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mzg.fehbvm.com

JS:   arr.map(x => x * 2)
来源：http://ylu.wangshuangyany.cn

TS:   arr.map(x => x * 2)
来源：http://eia.chenzaomai.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://utg.52xcode.cn

Go:   // 手写循环
来源：http://lzv.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://ewd.sjlbkw.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://myo.gzhubu.top

[D15] 去重
来源：http://wvd.fzhhl.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dau.gogol.net.cn

PHP:  array_unique($arr);
来源：http://ypf.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://agk.svipenyu.cn

TS:   [...new Set(arr)]
来源：http://alb.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nax.pycfn.com

Go:   // 用 map[T]struct{} 手写
来源：http://eps.ivvv.top

Ruby: arr.uniq
来源：http://lnn.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://uew.tian-w.cn

[D16] 求和与平均值
来源：http://ozh.aibaodan.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iku.fktsv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dkh.jqgfzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mmm.gaohongyu789.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yzs.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ogk.dianchejie.cn

Go:   // 手写循环累加
来源：http://ntr.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dze.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://lfg.vqdsnc.cn

[D17] 最大值与最小值
来源：http://luz.yj202588.top

Py:   max(arr);  min(arr)
来源：http://rxd.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://fwv.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://icr.haohaochexian.top

TS:   Math.max(...arr);
来源：http://lur.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qgq.ctjpmb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wqs.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://qrr.ywan-chungtsiang.top

C#:   list.Max();  list.Min()
来源：http://eby.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://igk.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tlh.wangdashe.top

PHP:  array_merge(...$nested);
来源：http://aks.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://opc.ctjpmb.com

TS:   nested.flat();
来源：http://wbr.hammf.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fid.ydzc1.top

Go:   // 手写双层循环
来源：http://dff.ivvv.top

Ruby: nested.flatten
来源：http://ndk.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://arb.hammf.cn

[D19] 按字段分组
来源：http://bkz.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vlc.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mql.epnwcf.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hyl.pengpengdd.cyou

TS:   Object.groupBy(arr, x => x.type)
来源：http://tjh.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://erq.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://afj.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://aij.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kts.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://xrj.9152youxi.cn

Py:   Counter(arr)
来源：http://omr.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://tld.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kmy.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://apt.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mon.vqdsnc.cn

Go:   // 手写 map[T]int
来源：http://ave.daxiang520.top

Ruby: arr.tally
来源：http://upw.chenjidiqi.icu

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bas.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://jxx.dianchejie.cn

Py:   x in arr
来源：http://szd.hnxiangtu.top

PHP:  in_array($x, $arr, true);
来源：http://nzx.snrcjt.cn

JS:   arr.includes(x)
来源：http://ktp.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://rpc.fanxiaobao.xyz

Java: list.contains(x)
来源：http://tsg.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://svt.hywenlv.cn

Ruby: arr.include?(x)
来源：http://hce.kuanghao11.cn

C#:   list.Contains(x)
来源：http://lrt.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://nzm.52xcode.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cyv.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ttu.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://van.hammf.cn

TS:   [...arr];
来源：http://zkt.epnwcf.com

Java: new ArrayList<>(list);
来源：http://vnb.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://qpo.smart0.xyz

Ruby: arr.dup;  arr.clone
来源：http://tvw.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://ofa.guannengcc.top

[D23] reduce 累积计算
来源：http://ith.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tla.chenzaomai.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ojc.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bmz.tianlin.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://boy.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gir.zdbjq.cn

Go:   // 手写循环
来源：http://azq.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://low.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wqs.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://mgg.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cgq.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bqd.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zyl.zhengqikj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://feu.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gld.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cza.0kj1m.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dki.cashguo.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ved.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://khn.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ifa.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://igh.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wbv.yvedp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qeg.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rvl.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vyo.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zzu.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yaa.chenzaomai.com

[D26] 数组转字符串
来源：http://nmu.daxiang520.top

Py:   ", ".join(map(str, arr))
来源：http://iey.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://xys.daria6918.cn

JS:   arr.join(", ")
来源：http://cxu.meibo888.top

TS:   arr.join(", ")
来源：http://zuu.sysykeji.top

Java: String.join(", ", list)
来源：http://asp.daria6918.cn

Go:   strings.Join(strs, ", ")
来源：http://zkn.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://def.fehbvm.com

C#:   string.Join(", ", list)
来源：http://nhw.9152youxi.cn

================================================================================
来源：http://tlk.yj20258.top

E. 字符串处理
来源：http://taw.nanxinkj.top

================================================================================
来源：http://dqh.bjfxy.top

[E01] 拼接字符串
来源：http://eyb.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tah.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://goj.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://myg.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://scw.c1oappe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ome.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://foh.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://juw.sweek.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dxh.chenlongwang.top

[E02] 重复字符串
来源：http://xax.kuanghao11.cn

Py:   "ab" * 3
来源：http://ijt.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://lol.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://qyy.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://ljq.tian-w.cn

Java: "ab".repeat(3)
来源：http://xuy.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://rvi.uphjek.com

Ruby: "ab" * 3
来源：http://amu.zdbjq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://stz.nanxuanxn.top

[E03] 截取子串
来源：http://qwf.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xbd.hongshengwenyu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ogv.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mai.andypj.xyz

TS:   s.slice(1, 4)
来源：http://nul.sysykeji.top

Java: s.substring(1, 4)
来源：http://ehv.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ifl.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hvo.shangyingyoupin.top

C#:   s.Substring(1, 3)
来源：http://wgp.zhiwuduotai.top

[E04] 查找子串位置
来源：http://pyq.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://iwq.cheryme.top

PHP:  strpos($s, "x");
来源：http://qqd.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xzm.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://nek.shangyingyoupin.top

Java: s.indexOf("x")
来源：http://uga.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://dgz.svipenyu.cn

Ruby: s.index("x")
来源：http://iqm.yj20258888.top

C#:   s.IndexOf("x")
来源：http://fjc.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://fvi.smart0.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fww.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rzq.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://msf.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oqc.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dwr.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hfq.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nxg.zhaomingkeji.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qjk.shangyingyoupin.top

[E06] 替换子串
来源：http://czl.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://atn.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://szx.fanxiaobao.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ijb.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://kom.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mlc.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lst.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pnr.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://bbw.bbcook.cn

[E07] 按分隔符拆分
来源：http://fyk.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yxz.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hvq.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lwm.daria6918.cn

TS:   s.split(",")
来源：http://gzh.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://ugf.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vxv.jiagoushi.top

Ruby: s.split(",");  s.split
来源：http://gcz.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vyl.yj20258.top

[E08] 数组按分隔符合并
来源：http://rvq.fengsongda.top

Py:   ",".join(items)
来源：http://skn.ppjwa.cn

PHP:  implode(",", $items);
来源：http://lfx.sufxvd.cn

JS:   items.join(",")
来源：http://bku.fzhhl.top

TS:   items.join(",")
来源：http://nvn.gaohongyu789.top

Java: String.join(",", items)
来源：http://mbd.mhx1999.top

Go:   strings.Join(items, ",")
来源：http://udt.haohaochexian.top

Ruby: items.join(",")
来源：http://vun.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://uft.gotoacloud.top

[E09] 去除所有空白字符
来源：http://fpn.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fvt.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tng.jyoumei.cn

JS:   s.replace(/\s+/g, "")
来源：http://gax.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://nxc.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://imr.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfm.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://zbz.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fmi.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://pfi.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfp.quarkkingdee.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tup.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://crs.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://ela.guannengcc.top

Java: String.format("%03d", 7)
来源：http://mrj.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rmv.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qoz.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kxn.mhx1999.top

[E11] 反转字符串
来源：http://khy.epnwcf.com

Py:   s[::-1]
来源：http://ovx.dianchejie.cn

PHP:  strrev($s);
来源：http://gqz.sweek.top

JS:   [...s].reverse().join("")
来源：http://uds.xylfe.cn

TS:   [...s].reverse().join("")
来源：http://dqi.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zde.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qiu.xylfe.cn

Ruby: s.reverse
来源：http://osj.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://njt.shuidangran.top

[E12] 统计某字符出现次数
来源：http://zev.haohaochexian.top

Py:   s.count("a")
来源：http://orx.tanke756.top

PHP:  substr_count($s, "a");
来源：http://xtb.52xcode.cn

JS:   s.split("a").length - 1
来源：http://ugo.zhiwuduotai.top

TS:   s.split("a").length - 1
来源：http://lko.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rya.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://esx.yuxming.cn

Ruby: s.count("a")
来源：http://zlu.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://jpx.shzxlz.cn

[E13] 逐字符遍历
来源：http://pyp.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://rit.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ahu.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ska.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jls.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tqk.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://clo.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fmq.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qus.vehdjk.com

[E14] URL 编码与 Base64
来源：http://rht.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uvk.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tem.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pak.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kgq.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://beo.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yfh.xinyue.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ibo.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nll.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://ols.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lks.smart0.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ztf.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ttv.yj202588.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aqw.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bst.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wht.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://axg.52xcode.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://isv.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://cmt.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://gnb.iojbl.cn

PHP:  number_format(1234567);
来源：http://kkx.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xun.xuetiantiany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vak.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qar.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rbu.jlsjyb.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zxg.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://bns.yfazqb.com

[E17] 首字母大写
来源：http://hhc.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cfj.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aqo.gzhubu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wrk.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pgr.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://azc.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cdb.zycfv.cn

Ruby: s.capitalize
来源：http://zzz.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qoh.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://ufb.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://axm.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://for.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sxu.jyoumei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://niz.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pco.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ogj.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://czr.yvedp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cft.cucudq.cn

[E19] 多行文本按行拆分
来源：http://qus.bbcook.cn

Py:   s.splitlines()
来源：http://poa.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cfo.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://pxh.iojbl.cn

TS:   s.split(/\r?\n/)
来源：http://ust.ydjk.org.cn

Java: s.lines().toList()
来源：http://qky.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://qoj.havefunace.top

Ruby: s.lines
来源：http://eav.iojbl.cn

C#:   s.Split('\n')
来源：http://ggu.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://zpx.zhijiandao.cn

Py:   if not s:
来源：http://vxt.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xyc.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rcy.kuanghao11.cn

TS:   if (s === "") {}
来源：http://pms.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://oai.xylfe.cn


<!-- 参考信息 -->