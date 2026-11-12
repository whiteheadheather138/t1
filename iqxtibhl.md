代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rmq.fengsongda.top

Ruby: arr.select { |x| x > 3 }
来源：http://dzl.zhijiandao.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lcd.cashguo.top

[D14] 映射转换（每个元素变形）
来源：http://fhe.guannengcc.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://upg.tanke756.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fed.redwolf501.top

JS:   arr.map(x => x * 2)
来源：http://cxn.dashuyun.cn

TS:   arr.map(x => x * 2)
来源：http://cfr.cdnleiting.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hsl.jinqigfzy.top

Go:   // 手写循环
来源：http://csf.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://czl.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://fiy.jinqigfzy.top

[D15] 去重
来源：http://aiw.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pcw.cheryme.top

PHP:  array_unique($arr);
来源：http://jke.yongpay.top

JS:   [...new Set(arr)]
来源：http://rig.cheryme.top

TS:   [...new Set(arr)]
来源：http://adf.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lla.xingfuxueyuan.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://brq.cucudq.cn

Ruby: arr.uniq
来源：http://syd.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://hwq.daxiang520.top

[D16] 求和与平均值
来源：http://crs.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hui.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vfa.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://efs.zhiwuduotai.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qzi.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://igs.yuxming.cn

Go:   // 手写循环累加
来源：http://oev.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zja.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://jfy.dianchejie.cn

[D17] 最大值与最小值
来源：http://ing.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://avq.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://zia.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://agh.ybcxt.top

TS:   Math.max(...arr);
来源：http://yis.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://lgc.hywenlv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://myv.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://mae.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://ycq.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://hej.fktsv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wsk.cheryme.top

PHP:  array_merge(...$nested);
来源：http://yfj.zdbjq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://thh.jinqigfzy.top

TS:   nested.flat();
来源：http://toq.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ppb.sweek.top

Go:   // 手写双层循环
来源：http://boa.chenzaomai.com

Ruby: nested.flatten
来源：http://gqv.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ekb.yonumen.top

[D19] 按字段分组
来源：http://ghz.yueranfly.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cgl.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://usa.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hpp.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qzz.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://llx.cashguo.top

Go:   // 手写 map[string][]T
来源：http://lnj.tarul.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qjr.guannengcc.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://unr.meibo888.top

[D20] 统计每个元素出现次数
来源：http://iyn.yj202588.top

Py:   Counter(arr)
来源：http://xif.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://zgk.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bmg.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fxf.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ihq.aibaodan.cn

Go:   // 手写 map[T]int
来源：http://zmf.sufxvd.cn

Ruby: arr.tally
来源：http://klw.xylfe.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ffa.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://red.mhx1999.top

Py:   x in arr
来源：http://xuy.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://nfa.zdqjudy.top

JS:   arr.includes(x)
来源：http://cgg.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://ylx.chenlongwang.top

Java: list.contains(x)
来源：http://asc.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://emz.sufxvd.cn

Ruby: arr.include?(x)
来源：http://oco.haohaochexian.top

C#:   list.Contains(x)
来源：http://iul.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://qna.yj20258.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gvb.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zae.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uti.zhijiandao.cn

TS:   [...arr];
来源：http://dgg.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://ksg.smart0.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ejw.hysaishi.cn

Ruby: arr.dup;  arr.clone
来源：http://ktx.hywenlv.cn

C#:   new List<int>(list);
来源：http://awa.hammf.cn

[D23] reduce 累积计算
来源：http://brm.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://viy.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ift.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://swm.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gvm.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://grl.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://vrl.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fja.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nfk.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://sxg.fehbvm.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zyi.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sfl.shanyushiyangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://muf.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wrm.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://onw.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ode.jlsjyb.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ybx.haohaochexian.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hmv.hnxiangtu.top

[D25] Set 集合去重与交并差
来源：http://hwc.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xhc.haohaochexian.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zul.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jge.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fyh.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yov.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cje.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pzs.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wzp.wangshuangyany.cn

[D26] 数组转字符串
来源：http://ine.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://kud.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://aaf.ivvv.top

JS:   arr.join(", ")
来源：http://lnz.316326.xyz

TS:   arr.join(", ")
来源：http://ovy.svipenyu.cn

Java: String.join(", ", list)
来源：http://vgu.ybcxt.top

Go:   strings.Join(strs, ", ")
来源：http://eov.yangfankeji.com

Ruby: arr.join(", ")
来源：http://ian.c1oappe.top

C#:   string.Join(", ", list)
来源：http://gbh.nanxuanxn.top

================================================================================
来源：http://exc.bbcook.cn

E. 字符串处理
来源：http://qga.ivvv.top

================================================================================
来源：http://okg.wangshuangyany.cn

[E01] 拼接字符串
来源：http://tgw.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oep.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dyc.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dkk.jinyuanbaomall.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://loi.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://suw.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uoq.ydzc1.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kvx.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hrg.chenzaomai.com

[E02] 重复字符串
来源：http://lss.hnxiangtu.top

Py:   "ab" * 3
来源：http://plu.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://ear.yj20258888.top

JS:   "ab".repeat(3)
来源：http://kxv.yj20258.top

TS:   "ab".repeat(3)
来源：http://hzl.yangfankeji.com

Java: "ab".repeat(3)
来源：http://vji.dianchejie.cn

Go:   strings.Repeat("ab", 3)
来源：http://nsf.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://kbj.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kup.kuanghao11.cn

[E03] 截取子串
来源：http://lfv.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mvu.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yit.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gif.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://zhi.smart0.xyz

Java: s.substring(1, 4)
来源：http://ype.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uau.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://upy.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://tcr.0kj1m.cn

[E04] 查找子串位置
来源：http://sdl.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://dbp.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://ich.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gmx.smart0.xyz

TS:   s.indexOf("x")
来源：http://itm.sjlbkw.cn

Java: s.indexOf("x")
来源：http://aar.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://plt.ydjk.org.cn

Ruby: s.index("x")
来源：http://mpj.sweek.top

C#:   s.IndexOf("x")
来源：http://kaa.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://svv.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rvr.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ecm.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nta.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ctf.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://the.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ajb.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wwa.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nrl.0kj1m.cn

[E06] 替换子串
来源：http://iba.zhiwuduotai.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rsn.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://aoo.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tcz.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://lgd.cdnleiting.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pta.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://phg.sjlbkw.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://edm.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://vhv.jqgfzy.top

[E07] 按分隔符拆分
来源：http://ooc.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://itm.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bpa.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vkh.birdmap.top

TS:   s.split(",")
来源：http://dui.cqqwz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vzu.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fru.hongshengwenyu.top

Ruby: s.split(",");  s.split
来源：http://yvz.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vug.hfpthk.cn

[E08] 数组按分隔符合并
来源：http://xdc.316326.xyz

Py:   ",".join(items)
来源：http://wpk.yangfankeji.com

PHP:  implode(",", $items);
来源：http://iiw.wangshuangyany.cn

JS:   items.join(",")
来源：http://lxi.shuidangran.top

TS:   items.join(",")
来源：http://fez.yj202588.top

Java: String.join(",", items)
来源：http://rnh.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://mmx.vehdjk.com

Ruby: items.join(",")
来源：http://lsd.hesvh.cn

C#:   string.Join(",", items)
来源：http://tut.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://fdd.hfpthk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lwu.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xgs.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://yqy.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://xva.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://jue.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://akz.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://mvx.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mzk.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://rta.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zur.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qro.nanxuanxn.top

JS:   "7".padStart(3, "0")
来源：http://gwm.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://gkh.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://wlo.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uvs.shzxlz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wxj.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qqh.jqgufenzy.top

[E11] 反转字符串
来源：http://tuy.xuanzx.com

Py:   s[::-1]
来源：http://uro.ivvv.top

PHP:  strrev($s);
来源：http://nob.dashuyun.cn

JS:   [...s].reverse().join("")
来源：http://uyq.meibo888.top

TS:   [...s].reverse().join("")
来源：http://lsv.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xgv.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vxy.shangyingyoupin.top

Ruby: s.reverse
来源：http://vxw.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://djd.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://ugi.guannengcc.top

Py:   s.count("a")
来源：http://dpb.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://vra.smart0.xyz

JS:   s.split("a").length - 1
来源：http://zbx.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://lrp.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ocu.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://nbl.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://tzk.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://gta.hywenlv.cn

[E13] 逐字符遍历
来源：http://kzt.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://bgp.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pzt.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qbp.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://okv.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wor.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://piv.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://drt.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bsp.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://xch.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vjv.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://rsa.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dnv.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qwd.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rir.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xmp.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tde.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xtq.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://hbn.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vop.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hqr.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rjj.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xjk.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://teu.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://asx.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pim.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hyu.xziqi.cn

[E16] 数字千分位
来源：http://grt.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://tbz.yuxming.cn

PHP:  number_format(1234567);
来源：http://ecc.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xkn.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://stb.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jrj.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xcr.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kyx.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://zgs.havefunace.top

[E17] 首字母大写
来源：http://oek.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cjt.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://odu.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yrc.hnqzz.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sed.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uyn.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mit.bjfxy.top

Ruby: s.capitalize
来源：http://cyq.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jfu.gogol.net.cn

[E18] 模板占位符替换
来源：http://wgt.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rim.ybcxt.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qgw.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lsm.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lws.sxryk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lcp.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gou.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ikz.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hsv.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://iiu.shzxlz.cn

Py:   s.splitlines()
来源：http://oka.fanxiaobao.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kxn.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://wpf.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://hpb.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://gyd.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://zwx.ydzc1.top

Ruby: s.lines
来源：http://krp.yj20258888.top

C#:   s.Split('\n')
来源：http://ksx.cucudq.cn

[E20] 判断字符串是否为空
来源：http://vvc.cheryme.top

Py:   if not s:
来源：http://deo.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ujg.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hwx.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://qxn.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://oxr.zhaomingkeji.xyz


<!-- 参考信息 -->