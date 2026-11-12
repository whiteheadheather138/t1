代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qdf.yuanzhike.top

JS:   arr.filter(x => x > 3)
来源：http://mpa.zhiwuduotai.top

TS:   arr.filter(x => x > 3)
来源：http://coi.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qfu.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qwo.guannengcc.top

Ruby: arr.select { |x| x > 3 }
来源：http://bho.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ysk.hesvh.cn

[D14] 映射转换（每个元素变形）
来源：http://fcm.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://usb.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gfh.zhongyouzk.top

JS:   arr.map(x => x * 2)
来源：http://rdx.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://udg.ybcxt.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://kcl.fktsv.cn

Go:   // 手写循环
来源：http://jxd.svipenyu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jqj.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mcm.nwbrower.top

[D15] 去重
来源：http://jcl.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vhw.jinqigufen.top

PHP:  array_unique($arr);
来源：http://grm.aizwys.cn

JS:   [...new Set(arr)]
来源：http://tpl.0kj1m.cn

TS:   [...new Set(arr)]
来源：http://cfa.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://alt.chenzaomai.com

Go:   // 用 map[T]struct{} 手写
来源：http://hjc.bjfxy.top

Ruby: arr.uniq
来源：http://wli.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://tur.yuxming.cn

[D16] 求和与平均值
来源：http://zuw.jqgufenzy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jnx.c1oappe.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vky.ydzc1.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bhy.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdn.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lka.jinqigufen.top

Go:   // 手写循环累加
来源：http://hza.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kqa.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://eca.zdqjudy.top

[D17] 最大值与最小值
来源：http://xzj.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://zzs.316326.xyz

PHP:  max($arr);  min($arr);
来源：http://flv.kuanghao11.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hhs.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://izk.ppjwa.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zvo.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vst.fktsv.cn

Ruby: arr.max;  arr.min
来源：http://qkw.sjlbkw.cn

C#:   list.Max();  list.Min()
来源：http://zzx.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://feb.daxiang520.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qtd.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://acu.quarkkingdee.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xdc.ybcxt.top

TS:   nested.flat();
来源：http://khv.cqqwz.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hkf.yfazqb.com

Go:   // 手写双层循环
来源：http://wpn.zhoulong.xyz

Ruby: nested.flatten
来源：http://grw.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ski.xylfe.cn

[D19] 按字段分组
来源：http://qwj.shzxlz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fzg.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://xsl.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nsx.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ecx.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pzf.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://wit.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://txp.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gln.redwolf501.top

[D20] 统计每个元素出现次数
来源：http://kbx.havefunace.top

Py:   Counter(arr)
来源：http://lxc.cucudq.cn

PHP:  array_count_values($arr);
来源：http://ufn.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://onu.sysykeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yvg.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://frr.wangdashe.top

Go:   // 手写 map[T]int
来源：http://ssa.xuetiantiany.cn

Ruby: arr.tally
来源：http://dzw.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jup.jinqigufen.top

[D21] 判断是否包含某元素
来源：http://mcq.havefunace.top

Py:   x in arr
来源：http://fmn.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://gxp.bjfxy.top

JS:   arr.includes(x)
来源：http://vtq.chenlongwang.top

TS:   arr.includes(x)
来源：http://cff.havefunace.top

Java: list.contains(x)
来源：http://hnf.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://hhw.daria6918.cn

Ruby: arr.include?(x)
来源：http://prv.hfpthk.cn

C#:   list.Contains(x)
来源：http://xgv.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://qji.zycfv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ewv.xziqi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nvl.shanyushiyangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fms.guannengcc.top

TS:   [...arr];
来源：http://hpu.vehdjk.com

Java: new ArrayList<>(list);
来源：http://tsb.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ack.fehbvm.com

Ruby: arr.dup;  arr.clone
来源：http://shq.fktsv.cn

C#:   new List<int>(list);
来源：http://cov.nanxuanxn.top

[D23] reduce 累积计算
来源：http://icd.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dnw.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qwy.zdqjudy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sax.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gad.wangshuangyany.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mzc.sjlbkw.cn

Go:   // 手写循环
来源：http://dww.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tfd.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://egw.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://uxo.haohaochexian.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uly.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ecj.wangshuangyany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uhi.chenlongwang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ocd.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yvc.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kch.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hoh.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://umw.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://urs.0kj1m.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qxd.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hko.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zlr.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fpt.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nfr.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qyw.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kup.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hqf.cheryme.top

[D26] 数组转字符串
来源：http://ysk.hnxiangtu.top

Py:   ", ".join(map(str, arr))
来源：http://ebf.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://tqh.vehdjk.com

JS:   arr.join(", ")
来源：http://bkv.chenlongwang.top

TS:   arr.join(", ")
来源：http://mag.fktsv.cn

Java: String.join(", ", list)
来源：http://uhh.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://wdh.jinqigufen.top

Ruby: arr.join(", ")
来源：http://fep.ctjpmb.com

C#:   string.Join(", ", list)
来源：http://gsx.mhx1999.top

================================================================================
来源：http://uaa.sufxvd.cn

E. 字符串处理
来源：http://ypu.sysykeji.top

================================================================================
来源：http://abr.guannengcc.top

[E01] 拼接字符串
来源：http://qqp.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rxt.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nal.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rnk.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xrx.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hyo.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qmj.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xst.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kpt.yvedp.cn

[E02] 重复字符串
来源：http://wne.xuanzx.com

Py:   "ab" * 3
来源：http://vfx.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://pbp.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://yev.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://xbm.dianchejie.cn

Java: "ab".repeat(3)
来源：http://evs.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://uti.sweek.top

Ruby: "ab" * 3
来源：http://qhq.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jfa.guannengcc.top

[E03] 截取子串
来源：http://xuk.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ohj.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xay.jlsjyb.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jfl.316326.xyz

TS:   s.slice(1, 4)
来源：http://plp.cdnleiting.top

Java: s.substring(1, 4)
来源：http://ijd.chenlongwang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kqw.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://xnc.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://moo.cashguo.top

[E04] 查找子串位置
来源：http://zut.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://spi.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://ijc.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ofv.hongshengwenyu.top

TS:   s.indexOf("x")
来源：http://whb.xinyue.icu

Java: s.indexOf("x")
来源：http://gml.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://ldc.zhengqikj.top

Ruby: s.index("x")
来源：http://kcn.nwbrower.top

C#:   s.IndexOf("x")
来源：http://jue.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pfn.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uee.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wad.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ubm.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hka.yj20258888.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fld.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uja.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://upl.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dmg.epnwcf.com

[E06] 替换子串
来源：http://axz.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://grh.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://wbv.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mcy.ivvv.top

TS:   s.replaceAll("a", "b")
来源：http://izn.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bev.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uym.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mnq.havefunace.top

C#:   s.Replace("a", "b")
来源：http://nmh.shzxlz.cn

[E07] 按分隔符拆分
来源：http://asa.cqqwz.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uth.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sde.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://htp.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://fyd.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://ojo.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jsx.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://tjg.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iln.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://uvd.zycfv.cn

Py:   ",".join(items)
来源：http://ezh.tianlin.xyz

PHP:  implode(",", $items);
来源：http://zad.wangdashe.top

JS:   items.join(",")
来源：http://rjj.cheryme.top

TS:   items.join(",")
来源：http://sxn.kuanghao11.cn

Java: String.join(",", items)
来源：http://ybp.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://doh.hnqzz.top

Ruby: items.join(",")
来源：http://vad.aizwys.cn

C#:   string.Join(",", items)
来源：http://qjj.bjfxy.top

[E09] 去除所有空白字符
来源：http://ych.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://huc.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ldw.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://qpf.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://pns.yj20258.top

Java: s.replaceAll("\\s+", "")
来源：http://xew.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://djg.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://ygk.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cif.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://lhr.xinyue.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://znv.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mhu.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://iim.shanyushiyangkeji.top

TS:   "7".padStart(3, "0")
来源：http://foi.yuxming.cn

Java: String.format("%03d", 7)
来源：http://sot.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yrg.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ixg.yvedp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://phs.smart0.xyz

[E11] 反转字符串
来源：http://vhw.316326.xyz

Py:   s[::-1]
来源：http://tll.cheryme.top

PHP:  strrev($s);
来源：http://gfw.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://eds.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://qqu.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xmv.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jqq.zhengqikj.top

Ruby: s.reverse
来源：http://llo.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://vdf.hammf.cn

[E12] 统计某字符出现次数
来源：http://wps.xziqi.cn

Py:   s.count("a")
来源：http://jss.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://wws.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://fdf.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://ekj.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sjf.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://hju.cucudq.cn

Ruby: s.count("a")
来源：http://nbr.cdnleiting.top

C#:   s.Count(c => c == 'a')
来源：http://eqa.zhijiandao.cn

[E13] 逐字符遍历
来源：http://aay.316326.xyz

Py:   for ch in s: print(ch)
来源：http://qau.hfpthk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fzk.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cta.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lft.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gqt.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hzt.jianghu66.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rra.hcnkem.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zom.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://iye.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xla.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wke.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dnf.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rzm.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tfb.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ncu.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://anj.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ksv.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://kqe.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yqx.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yzj.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wyt.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cws.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dhe.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hji.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hdn.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsq.sweek.top

[E16] 数字千分位
来源：http://hds.havefunace.top

Py:   f"{1234567:,}"
来源：http://plz.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://yzq.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tpq.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iyy.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yec.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ikb.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ezt.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://cdb.zdbjq.cn

[E17] 首字母大写
来源：http://tef.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mei.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bad.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbc.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gnv.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ooi.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://drv.xingfuxueyuan.xyz

Ruby: s.capitalize
来源：http://hwf.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://imw.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://bsi.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jvu.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nki.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://ims.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://uaw.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ehy.ydzc1.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fek.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hmq.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dpn.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://njc.fktsv.cn

Py:   s.splitlines()
来源：http://fwi.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://trp.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://gab.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://twe.bjfxy.top

Java: s.lines().toList()
来源：http://hhi.cdnleiting.top

Go:   strings.Split(s, "\n")
来源：http://htg.aibaodan.cn

Ruby: s.lines
来源：http://irp.zhoulong.xyz

C#:   s.Split('\n')
来源：http://whu.shuidangran.top

[E20] 判断字符串是否为空
来源：http://jdc.zhiwuduotai.top

Py:   if not s:
来源：http://imq.ydzc1.top


<!-- 参考信息 -->