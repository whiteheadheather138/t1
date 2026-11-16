代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://caq.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://dqm.uphjek.com

TS:   arr.filter(x => x > 3)
来源：http://zar.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qwm.epnwcf.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xqd.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://oos.birdmap.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zlp.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://evd.shzxlz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://izy.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wvu.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://evy.hywenlv.cn

TS:   arr.map(x => x * 2)
来源：http://dco.zhongyouzk.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qlc.hnqzz.top

Go:   // 手写循环
来源：http://eeb.sufxvd.cn

Ruby: arr.map { |x| x * 2 }
来源：http://duf.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vau.hnxiangtu.top

[D15] 去重
来源：http://wvg.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uag.bjfxy.top

PHP:  array_unique($arr);
来源：http://yit.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://xmb.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://wfy.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lju.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uup.hnxiangtu.top

Ruby: arr.uniq
来源：http://vix.cqqwz.cn

C#:   list.Distinct().ToList()
来源：http://wwd.nanxuanxn.top

[D16] 求和与平均值
来源：http://rne.zhaomingkeji.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sjd.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ajs.sufxvd.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ayy.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yqc.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://smf.yj20258.top

Go:   // 手写循环累加
来源：http://dny.iojbl.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hkr.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://bqm.fktsv.cn

[D17] 最大值与最小值
来源：http://lqr.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://koe.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://eeh.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tjj.316326.xyz

TS:   Math.max(...arr);
来源：http://gmq.sufxvd.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vgg.fzhhl.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nfe.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://hao.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://adb.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://clm.pengpengdd.cyou

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wym.sufxvd.cn

PHP:  array_merge(...$nested);
来源：http://svt.sysykeji.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fgc.xylfe.cn

TS:   nested.flat();
来源：http://rir.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hcb.xuanzx.com

Go:   // 手写双层循环
来源：http://zby.feifeiyinyue.top

Ruby: nested.flatten
来源：http://vue.smart0.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://xpf.ppjwa.cn

[D19] 按字段分组
来源：http://ddb.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wuj.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://noy.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lpd.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sgm.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wrg.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://dyw.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fcl.zhiwuduotai.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://clp.havefunace.top

[D20] 统计每个元素出现次数
来源：http://zsa.quarkkingdee.top

Py:   Counter(arr)
来源：http://kbk.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://ofw.nwbrower.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rzw.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jkz.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://chf.ivvv.top

Go:   // 手写 map[T]int
来源：http://bqp.ehwqpu.com

Ruby: arr.tally
来源：http://qkr.fanxiaobao.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bez.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://qvr.yuxming.cn

Py:   x in arr
来源：http://hyq.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://pum.zdqjudy.top

JS:   arr.includes(x)
来源：http://hum.hcnkem.com

TS:   arr.includes(x)
来源：http://bjc.jqgufenzy.top

Java: list.contains(x)
来源：http://koy.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://rpl.daria6918.cn

Ruby: arr.include?(x)
来源：http://hcw.yuanzhike.top

C#:   list.Contains(x)
来源：http://veu.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://nrm.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xfk.tanke756.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eac.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfn.shzxlz.cn

TS:   [...arr];
来源：http://kzi.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://xtk.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://ovc.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://bxg.vqdsnc.cn

C#:   new List<int>(list);
来源：http://syn.cdnleiting.top

[D23] reduce 累积计算
来源：http://vvn.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://frs.cashguo.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nwb.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mfz.jyoumei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hhs.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ugl.fehbvm.com

Go:   // 手写循环
来源：http://kor.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ygk.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bcu.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://trl.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://goo.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://obh.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pdv.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kqx.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ulo.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ejy.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zoc.52xcode.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pwe.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://vqc.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wri.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ive.cashguo.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qxk.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://awj.chenlongwang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ywi.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cwb.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mbt.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xbr.hcnkem.com

[D26] 数组转字符串
来源：http://cig.yuxming.cn

Py:   ", ".join(map(str, arr))
来源：http://fgm.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://veh.tanke756.top

JS:   arr.join(", ")
来源：http://gaz.pengpengdd.cyou

TS:   arr.join(", ")
来源：http://gjn.zycfv.cn

Java: String.join(", ", list)
来源：http://gqe.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://zgo.yueranfly.top

Ruby: arr.join(", ")
来源：http://vaw.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://wlr.smart0.xyz

================================================================================
来源：http://aub.hywenlv.cn

E. 字符串处理
来源：http://scp.c1oappe.top

================================================================================
来源：http://pts.sweek.top

[E01] 拼接字符串
来源：http://pjj.zhaomingkeji.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dji.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jqk.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gpt.pengpengdd.cyou

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyq.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mrb.shangyingyoupin.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vlb.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ixv.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmu.ydzc1.top

[E02] 重复字符串
来源：http://uxh.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://ift.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://ktj.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://kfp.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://krw.sxryk.cn

Java: "ab".repeat(3)
来源：http://zvd.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://ext.haohaochexian.top

Ruby: "ab" * 3
来源：http://zdv.gzhubu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ksb.ctjpmb.com

[E03] 截取子串
来源：http://hhz.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blm.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kak.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ezk.tarul.cn

TS:   s.slice(1, 4)
来源：http://vtv.hywenlv.cn

Java: s.substring(1, 4)
来源：http://lnb.yvedp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jub.zdqjudy.top

Ruby: s[1, 3];  s[1..3]
来源：http://cva.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://nmi.kuanghao11.cn

[E04] 查找子串位置
来源：http://gdj.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://xmt.hesvh.cn

PHP:  strpos($s, "x");
来源：http://kks.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wub.yueranfly.top

TS:   s.indexOf("x")
来源：http://sac.aizwys.cn

Java: s.indexOf("x")
来源：http://wxo.316326.xyz

Go:   strings.Index(s, "x")
来源：http://lta.sufxvd.cn

Ruby: s.index("x")
来源：http://rbp.hnxiangtu.top

C#:   s.IndexOf("x")
来源：http://ozp.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://prz.shanyushiyangkeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nas.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vur.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dch.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://htf.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wud.jinqigfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kmm.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lai.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://stl.sxryk.cn

[E06] 替换子串
来源：http://aup.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://whv.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://hsu.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iom.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://qcs.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xwo.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kpz.9152youxi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://elt.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://tfj.haohaochexian.top

[E07] 按分隔符拆分
来源：http://cuk.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bgz.shangyingyoupin.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hxk.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ppv.xuanzx.com

TS:   s.split(",")
来源：http://vyo.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://ztx.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rgs.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://wbr.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://msx.redwolf501.top

[E08] 数组按分隔符合并
来源：http://pnz.52xcode.cn

Py:   ",".join(items)
来源：http://oho.andypj.xyz

PHP:  implode(",", $items);
来源：http://jfe.shzxlz.cn

JS:   items.join(",")
来源：http://llp.wangdashe.top

TS:   items.join(",")
来源：http://ajq.fehbvm.com

Java: String.join(",", items)
来源：http://mqx.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://vku.dashuyun.cn

Ruby: items.join(",")
来源：http://xiq.iojbl.cn

C#:   string.Join(",", items)
来源：http://zle.svipenyu.cn

[E09] 去除所有空白字符
来源：http://mvs.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nqy.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ujt.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://oeu.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://nfp.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://ssz.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ggc.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gkt.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wsp.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://lue.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://klw.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gxs.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://yms.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://msz.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://xlh.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wab.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lmc.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jwp.bbcook.cn

[E11] 反转字符串
来源：http://tfj.yfazqb.com

Py:   s[::-1]
来源：http://eol.jinqigufen.top

PHP:  strrev($s);
来源：http://hec.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://dat.bjfxy.top

TS:   [...s].reverse().join("")
来源：http://gxn.jinyuanbaomall.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oio.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ixd.shzxlz.cn

Ruby: s.reverse
来源：http://wuu.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xks.nwbrower.top

[E12] 统计某字符出现次数
来源：http://csu.jianghu66.top

Py:   s.count("a")
来源：http://epc.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://goa.redwolf501.top

JS:   s.split("a").length - 1
来源：http://tfl.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://jrv.hnqzz.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lce.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://qsb.feifeiyinyue.top

Ruby: s.count("a")
来源：http://gir.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://dhg.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://nox.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://cka.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wjk.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ovg.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mtg.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oik.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dnf.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://lwd.zhoulong.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dro.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://rho.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dij.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fbm.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vov.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ywv.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ghi.yj20258.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rhi.uphjek.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://elq.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zjk.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://efw.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bxw.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zlf.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yvo.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://xoh.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://epk.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zvs.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://asq.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ing.tian-w.cn

[E16] 数字千分位
来源：http://dzh.yongpay.top

Py:   f"{1234567:,}"
来源：http://bfd.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://ers.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://syp.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qxe.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rdu.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rbh.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fca.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://kti.jinqigufen.top

[E17] 首字母大写
来源：http://nqf.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lfv.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uiu.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnw.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oku.gotoacloud.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dtf.snrcjt.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tro.shuidangran.top

Ruby: s.capitalize
来源：http://zgu.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yyv.zhengqikj.top

[E18] 模板占位符替换
来源：http://vod.yuxming.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rnw.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oyy.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://osk.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qaf.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://roo.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://she.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oxg.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cwa.sysykeji.top

[E19] 多行文本按行拆分
来源：http://ihg.daxiang520.top

Py:   s.splitlines()
来源：http://kbb.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://stt.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://fgj.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://qbs.wangshuangyany.cn

Java: s.lines().toList()
来源：http://ute.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://lfo.daxiang520.top

Ruby: s.lines
来源：http://bcp.jqgufenzy.top

C#:   s.Split('\n')
来源：http://fxj.vehdjk.com

[E20] 判断字符串是否为空
来源：http://ztb.gogol.net.cn

Py:   if not s:
来源：http://meo.zhixingplan.top


<!-- 参考信息 -->