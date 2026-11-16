代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zrd.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://zao.aizwys.cn

TS:   arr.filter(x => x > 3)
来源：http://jyf.gogol.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zcy.vehdjk.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cmz.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aej.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vhv.hongshengwenyu.top

[D14] 映射转换（每个元素变形）
来源：http://vgv.pycfn.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jos.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sxd.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://jap.yuanzhike.top

TS:   arr.map(x => x * 2)
来源：http://xlf.ywan-chungtsiang.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://aac.vqdsnc.cn

Go:   // 手写循环
来源：http://haa.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bxp.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qgu.ehwqpu.com

[D15] 去重
来源：http://snk.52xcode.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vsh.birdmap.top

PHP:  array_unique($arr);
来源：http://taa.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://ejg.hysaishi.cn

TS:   [...new Set(arr)]
来源：http://bvt.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fon.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://hhe.nanxuanxn.top

Ruby: arr.uniq
来源：http://ekc.tanke756.top

C#:   list.Distinct().ToList()
来源：http://ipq.chenlongwang.top

[D16] 求和与平均值
来源：http://hvi.chenzaomai.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://exy.fengsongda.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://njg.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zmr.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gcx.ppjwa.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gdw.cashguo.top

Go:   // 手写循环累加
来源：http://khx.zhoulong.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qhc.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://sqt.ydzc1.top

[D17] 最大值与最小值
来源：http://ngp.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://iiy.shanyushiyangtech.top

PHP:  max($arr);  min($arr);
来源：http://wpi.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wbd.daria6918.cn

TS:   Math.max(...arr);
来源：http://fra.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xeu.yfazqb.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://alp.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ggz.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://aov.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://xsc.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uww.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://cvo.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blf.yj202588.top

TS:   nested.flat();
来源：http://dpe.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gfz.jianghu66.top

Go:   // 手写双层循环
来源：http://zlc.jianghu66.top

Ruby: nested.flatten
来源：http://umi.shanyushiyangtech.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kyr.svipenyu.cn

[D19] 按字段分组
来源：http://xkt.52xcode.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wao.sufxvd.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bmv.shanyushiyangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cqd.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nfy.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jmo.xinyue.icu

Go:   // 手写 map[string][]T
来源：http://wbg.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xsh.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ihs.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://ejb.jianghu66.top

Py:   Counter(arr)
来源：http://avk.pycfn.com

PHP:  array_count_values($arr);
来源：http://aml.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lzw.zhijiandao.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://und.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xdb.jinyuanbaomall.cn

Go:   // 手写 map[T]int
来源：http://ljq.svipenyu.cn

Ruby: arr.tally
来源：http://azf.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wzv.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://jjn.yuxming.cn

Py:   x in arr
来源：http://oeu.zhongyouzk.top

PHP:  in_array($x, $arr, true);
来源：http://ldj.pycfn.com

JS:   arr.includes(x)
来源：http://gaz.hesvh.cn

TS:   arr.includes(x)
来源：http://snd.feifeiyinyue.top

Java: list.contains(x)
来源：http://wck.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://lzv.dashuyun.cn

Ruby: arr.include?(x)
来源：http://jcc.vehdjk.com

C#:   list.Contains(x)
来源：http://vxu.jianghu66.top

[D22] 复制数组（避免共享引用）
来源：http://lvc.chenlongwang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iqn.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cfr.yuxming.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dzj.c1oappe.top

TS:   [...arr];
来源：http://tfc.yj20258888.top

Java: new ArrayList<>(list);
来源：http://eup.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://gax.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://cji.ehwqpu.com

C#:   new List<int>(list);
来源：http://bve.svipenyu.cn

[D23] reduce 累积计算
来源：http://sza.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://elw.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://onn.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uzv.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qyr.havefunace.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ged.shangyingyoupin.top

Go:   // 手写循环
来源：http://ttu.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://onp.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bjn.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://xde.kuanghao11.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wad.gaohongyu789.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://epn.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rds.yj20258888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ghz.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cfc.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ajz.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hla.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jiz.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://kqt.xylfe.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wei.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jnl.wangdashe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfv.vqdsnc.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fet.yj202588.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bmh.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rbo.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vwa.zycfv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cup.yanxiufei.cn

[D26] 数组转字符串
来源：http://ghj.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://wye.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://kuv.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://gjw.jiagoushi.top

TS:   arr.join(", ")
来源：http://iwn.ctjpmb.com

Java: String.join(", ", list)
来源：http://ymx.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://gvf.ivvv.top

Ruby: arr.join(", ")
来源：http://oaz.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://hsj.wangshuangyany.cn

================================================================================
来源：http://vee.ehwqpu.com

E. 字符串处理
来源：http://vgb.svipenyu.cn

================================================================================
来源：http://hfo.chenjidiqi.icu

[E01] 拼接字符串
来源：http://dir.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ypg.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zuw.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yxk.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vjt.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ioh.zdqjudy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rrg.zhixingplan.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mof.yj202588.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dpu.shanyushiyangkeji.top

[E02] 重复字符串
来源：http://aff.guowangkeji.top

Py:   "ab" * 3
来源：http://ere.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://lqj.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://zfp.vehdjk.com

TS:   "ab".repeat(3)
来源：http://oww.yueranfly.top

Java: "ab".repeat(3)
来源：http://mcl.yongpay.top

Go:   strings.Repeat("ab", 3)
来源：http://hxy.xinyue.icu

Ruby: "ab" * 3
来源：http://jud.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nmp.yongpay.top

[E03] 截取子串
来源：http://xhb.zhengqikj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kuu.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ysi.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ush.uphjek.com

TS:   s.slice(1, 4)
来源：http://qus.redwolf501.top

Java: s.substring(1, 4)
来源：http://bjn.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://oxp.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://trc.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://qyr.pengpengdd.cyou

[E04] 查找子串位置
来源：http://anl.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://pmr.redwolf501.top

PHP:  strpos($s, "x");
来源：http://dpx.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qni.jiagoushi.top

TS:   s.indexOf("x")
来源：http://dav.zhoulong.xyz

Java: s.indexOf("x")
来源：http://loi.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://anb.jinqigfzy.top

Ruby: s.index("x")
来源：http://gaa.epnwcf.com

C#:   s.IndexOf("x")
来源：http://fup.gzhubu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://knw.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mcr.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dcs.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dro.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sde.havefunace.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iza.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qgn.xinyue.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mox.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vec.vehdjk.com

[E06] 替换子串
来源：http://kgx.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lfw.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://pzi.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nsq.cqqwz.cn

TS:   s.replaceAll("a", "b")
来源：http://shq.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://scs.shangyingyoupin.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uor.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ghq.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://clg.xziqi.cn

[E07] 按分隔符拆分
来源：http://pyq.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qqi.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zmd.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jiy.ybcxt.top

TS:   s.split(",")
来源：http://etm.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://zty.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zgb.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://wvg.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://znp.zhoulong.xyz

[E08] 数组按分隔符合并
来源：http://ozx.jqgufenzy.top

Py:   ",".join(items)
来源：http://nub.daria6918.cn

PHP:  implode(",", $items);
来源：http://dze.yonumen.top

JS:   items.join(",")
来源：http://hpm.aizwys.cn

TS:   items.join(",")
来源：http://lty.yj202588.top

Java: String.join(",", items)
来源：http://tug.xingfuxueyuan.xyz

Go:   strings.Join(items, ",")
来源：http://mep.pengpengdd.cyou

Ruby: items.join(",")
来源：http://siz.birdmap.top

C#:   string.Join(",", items)
来源：http://gdv.hammf.cn

[E09] 去除所有空白字符
来源：http://uhn.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xmg.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gro.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://vli.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://ojc.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://cqs.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zdf.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://pso.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uev.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://jvh.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sqt.jyoumei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nxa.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://sns.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://gng.yongpay.top

Java: String.format("%03d", 7)
来源：http://ksa.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fxo.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ica.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fjo.quarkkingdee.top

[E11] 反转字符串
来源：http://qah.sysykeji.top

Py:   s[::-1]
来源：http://xxj.sysykeji.top

PHP:  strrev($s);
来源：http://xlr.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://nyu.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://fdo.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://izg.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://bho.daxiang520.top

Ruby: s.reverse
来源：http://ofr.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://oen.wangdashe.top

[E12] 统计某字符出现次数
来源：http://vdm.sweek.top

Py:   s.count("a")
来源：http://zws.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://nxo.cucudq.cn

JS:   s.split("a").length - 1
来源：http://erl.jiagoushi.top

TS:   s.split("a").length - 1
来源：http://gmu.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fvt.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://gcs.vehdjk.com

Ruby: s.count("a")
来源：http://uby.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://ytq.jyoumei.cn

[E13] 逐字符遍历
来源：http://xyl.tarul.cn

Py:   for ch in s: print(ch)
来源：http://xjj.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bxb.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://huj.fzhhl.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ywc.hesvh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pzo.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ynm.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://xfj.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lsu.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://ert.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tez.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://liq.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yjx.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sgf.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txf.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tnd.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ftm.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vtl.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://jcz.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nue.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gas.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://scq.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yfw.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fqx.yangfankeji.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tdp.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://umr.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vni.dashuyun.cn

[E16] 数字千分位
来源：http://jzt.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://wot.sxryk.cn

PHP:  number_format(1234567);
来源：http://vcs.nanxinkj.top

JS:   (1234567).toLocaleString("en-US")
来源：http://efy.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fob.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lrr.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bou.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ivg.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://ltl.daria6918.cn

[E17] 首字母大写
来源：http://ldu.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jba.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zfm.uphjek.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fcq.9152youxi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xoj.tianlin.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rym.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eek.shuidangran.top

Ruby: s.capitalize
来源：http://dle.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwa.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://iuw.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gqa.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yjr.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qbi.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bbk.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rlv.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ycl.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fdn.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vgz.wangdashe.top

[E19] 多行文本按行拆分
来源：http://hmi.zdbjq.cn

Py:   s.splitlines()
来源：http://uvp.sjlbkw.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cuc.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://fxq.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://bxq.zhiwuduotai.top

Java: s.lines().toList()
来源：http://sbx.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://cgk.xylfe.cn

Ruby: s.lines
来源：http://wac.snrcjt.cn

C#:   s.Split('\n')
来源：http://ltc.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://izf.smart0.xyz

Py:   if not s:
来源：http://uqj.zhiwuduotai.top


<!-- 参考信息 -->