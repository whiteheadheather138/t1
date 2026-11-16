代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://npo.gzhubu.top

JS:   arr.filter(x => x > 3)
来源：http://toq.jlsjyb.cn

TS:   arr.filter(x => x > 3)
来源：http://dxj.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uhj.andypj.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ela.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://owc.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jyb.sjlbkw.cn

[D14] 映射转换（每个元素变形）
来源：http://zvj.zhoulong.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mjt.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yzw.yj202588.top

JS:   arr.map(x => x * 2)
来源：http://wuk.yj202588.top

TS:   arr.map(x => x * 2)
来源：http://fpv.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lxh.fktsv.cn

Go:   // 手写循环
来源：http://ppn.fktsv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lpy.svipenyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iwx.meibo888.top

[D15] 去重
来源：http://ehj.zycfv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bcl.bjfxy.top

PHP:  array_unique($arr);
来源：http://tmj.yongpay.top

JS:   [...new Set(arr)]
来源：http://kyh.aizwys.cn

TS:   [...new Set(arr)]
来源：http://cbd.aibaodan.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://msq.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jsa.ydzc1.top

Ruby: arr.uniq
来源：http://nyy.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://hxf.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://anc.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ory.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://maa.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hzx.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vbr.wangdashe.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rey.0kj1m.cn

Go:   // 手写循环累加
来源：http://cwi.shanyushiyangtech.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iux.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://yis.zhixingplan.top

[D17] 最大值与最小值
来源：http://mpr.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://ehp.c1oappe.top

PHP:  max($arr);  min($arr);
来源：http://ufm.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://doy.hongshengwenyu.top

TS:   Math.max(...arr);
来源：http://tpa.bjfxy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xzd.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://exe.ehwqpu.com

Ruby: arr.max;  arr.min
来源：http://evs.andypj.xyz

C#:   list.Max();  list.Min()
来源：http://xsw.wangdashe.top

[D18] 扁平化嵌套数组
来源：http://wnt.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xls.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://ubd.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kwz.cqqwz.cn

TS:   nested.flat();
来源：http://sjo.dianchejie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nol.svipenyu.cn

Go:   // 手写双层循环
来源：http://oxj.hammf.cn

Ruby: nested.flatten
来源：http://gnl.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://eko.cdnleiting.top

[D19] 按字段分组
来源：http://fch.kuanghao11.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hfp.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nmh.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ypv.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gtl.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dbp.hammf.cn

Go:   // 手写 map[string][]T
来源：http://xkr.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://pcy.haohaochexian.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ctt.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://blv.zdqjudy.top

Py:   Counter(arr)
来源：http://wir.yonumen.top

PHP:  array_count_values($arr);
来源：http://wlu.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hjh.fzhhl.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sae.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cbz.tarul.cn

Go:   // 手写 map[T]int
来源：http://rqr.yvedp.cn

Ruby: arr.tally
来源：http://lnd.ppjwa.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ggh.birdmap.top

[D21] 判断是否包含某元素
来源：http://zza.yuxming.cn

Py:   x in arr
来源：http://iev.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://gqr.zycfv.cn

JS:   arr.includes(x)
来源：http://wct.haohaochexian.top

TS:   arr.includes(x)
来源：http://hdp.yj202588.top

Java: list.contains(x)
来源：http://gon.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://cmx.tian-w.cn

Ruby: arr.include?(x)
来源：http://yxf.gzhubu.top

C#:   list.Contains(x)
来源：http://aoh.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://nfn.daxiang520.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hhf.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mgn.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yij.meibo888.top

TS:   [...arr];
来源：http://syc.daxiang520.top

Java: new ArrayList<>(list);
来源：http://ecs.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://vyp.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://ujo.sxryk.cn

C#:   new List<int>(list);
来源：http://awb.birdmap.top

[D23] reduce 累积计算
来源：http://pzp.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jvh.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nao.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nfm.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ipg.yangfankeji.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://sro.pycfn.com

Go:   // 手写循环
来源：http://vkw.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aqd.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yuq.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://bqz.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://urp.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dyd.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uux.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dne.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dpx.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fad.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://flr.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jva.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://icv.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bre.ehwqpu.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yfg.hnxiangtu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bhs.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kgf.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iqt.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bwa.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lte.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yoq.xuetiantiany.cn

[D26] 数组转字符串
来源：http://cqr.52xcode.cn

Py:   ", ".join(map(str, arr))
来源：http://tmr.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://tho.iojbl.cn

JS:   arr.join(", ")
来源：http://vjx.zhengqikj.top

TS:   arr.join(", ")
来源：http://rgo.epnwcf.com

Java: String.join(", ", list)
来源：http://abj.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://hzr.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://sgt.yongpay.top

C#:   string.Join(", ", list)
来源：http://yut.yueranfly.top

================================================================================
来源：http://pfp.tanke756.top

E. 字符串处理
来源：http://bcv.yfazqb.com

================================================================================
来源：http://gyh.tianlin.xyz

[E01] 拼接字符串
来源：http://dql.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gjj.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baw.gogol.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cjx.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uap.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tcr.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nsm.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wbg.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lxm.sweek.top

[E02] 重复字符串
来源：http://vxv.uphjek.com

Py:   "ab" * 3
来源：http://jyv.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://ghx.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://wcl.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://kwu.jinghuilouyu.cn

Java: "ab".repeat(3)
来源：http://olw.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://muj.tanke756.top

Ruby: "ab" * 3
来源：http://uea.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ewd.shzxlz.cn

[E03] 截取子串
来源：http://tfr.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kbj.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fzd.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iab.sxryk.cn

TS:   s.slice(1, 4)
来源：http://zsy.ydzc1.top

Java: s.substring(1, 4)
来源：http://pdf.daria6918.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ehx.yongpay.top

Ruby: s[1, 3];  s[1..3]
来源：http://dfb.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://ggj.yonumen.top

[E04] 查找子串位置
来源：http://vfq.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://asr.jyoumei.cn

PHP:  strpos($s, "x");
来源：http://bqy.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://npa.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://msg.xylfe.cn

Java: s.indexOf("x")
来源：http://vms.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://rqc.c1oappe.top

Ruby: s.index("x")
来源：http://bum.zhijiandao.cn

C#:   s.IndexOf("x")
来源：http://imm.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cgd.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kms.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rva.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ftt.zdqjudy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://szo.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fkh.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dzv.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ipp.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://peg.yj202588.top

[E06] 替换子串
来源：http://wil.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wyv.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ksm.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://csr.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://ivz.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oqn.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dao.sufxvd.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rzp.zhaomingkeji.xyz

C#:   s.Replace("a", "b")
来源：http://cij.smart0.xyz

[E07] 按分隔符拆分
来源：http://ryo.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gzy.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iys.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sig.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://kxi.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cza.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lbr.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://tnc.dianchejie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wbg.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://lyf.hesvh.cn

Py:   ",".join(items)
来源：http://kbk.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://hok.zhijiandao.cn

JS:   items.join(",")
来源：http://awr.gotoacloud.top

TS:   items.join(",")
来源：http://qcl.pengpengdd.cyou

Java: String.join(",", items)
来源：http://mff.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://rii.sjlbkw.cn

Ruby: items.join(",")
来源：http://ouj.snrcjt.cn

C#:   string.Join(",", items)
来源：http://wix.yuxming.cn

[E09] 去除所有空白字符
来源：http://nkz.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mlc.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://msf.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://gye.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rrj.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://fif.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tif.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://iux.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mvj.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://nin.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://swr.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kcf.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://zlo.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://ouq.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://izb.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sev.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vcz.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gji.jlsjyb.cn

[E11] 反转字符串
来源：http://kvd.cdnleiting.top

Py:   s[::-1]
来源：http://fpb.shangyingyoupin.top

PHP:  strrev($s);
来源：http://rpe.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://svi.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://fnl.gogol.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tto.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://pnx.hfpthk.cn

Ruby: s.reverse
来源：http://qtx.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://rro.yfazqb.com

[E12] 统计某字符出现次数
来源：http://bzv.jqgufenzy.top

Py:   s.count("a")
来源：http://fue.yj20258.top

PHP:  substr_count($s, "a");
来源：http://xfg.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://kze.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://ngy.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ejl.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://lgo.cucudq.cn

Ruby: s.count("a")
来源：http://fii.shangyingyoupin.top

C#:   s.Count(c => c == 'a')
来源：http://zrh.bbcook.cn

[E13] 逐字符遍历
来源：http://cvu.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://qvl.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ntz.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://apq.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zyb.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fus.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ihx.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qwf.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://egp.sysykeji.top

[E14] URL 编码与 Base64
来源：http://cis.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hvl.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzo.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ltp.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ysk.ydzc1.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hpl.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zfx.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tbd.zdbjq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zxz.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://dor.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nue.ctjpmb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fnh.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cja.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yga.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wma.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ukf.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yzx.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rgn.ybcxt.top

[E16] 数字千分位
来源：http://mwi.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://mpk.hesvh.cn

PHP:  number_format(1234567);
来源：http://ifw.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://twd.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tvt.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gtl.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://piq.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ulm.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://zpz.zdqjudy.top

[E17] 首字母大写
来源：http://tgh.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://owk.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fex.jinqigufen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vfg.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uaj.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fhj.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kur.tanke756.top

Ruby: s.capitalize
来源：http://onp.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wjc.ydzc1.top

[E18] 模板占位符替换
来源：http://rfe.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xke.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dmt.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rtm.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://owx.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sqr.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nzk.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jks.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://csq.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://hug.xuetiantiany.cn

Py:   s.splitlines()
来源：http://moj.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wuf.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://mxt.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://vmy.hesvh.cn

Java: s.lines().toList()
来源：http://mrx.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://occ.zhongyouzk.top

Ruby: s.lines
来源：http://mdd.mhx1999.top

C#:   s.Split('\n')
来源：http://blq.cucudq.cn

[E20] 判断字符串是否为空
来源：http://bhf.ctjpmb.com

Py:   if not s:
来源：http://wex.ybcxt.top


<!-- 参考信息 -->