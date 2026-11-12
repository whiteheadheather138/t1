代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ora.ctjpmb.com

JS:   arr.filter(x => x > 3)
来源：http://nuq.havefunace.top

TS:   arr.filter(x => x > 3)
来源：http://rip.yueranfly.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://itm.yj20258.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yku.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://skf.jinghuilouyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sso.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://idj.yueranfly.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://pkq.daria6918.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lcb.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://ttf.sysykeji.top

TS:   arr.map(x => x * 2)
来源：http://sct.tarul.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://bxk.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://ijh.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://fql.kuanghao11.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rni.jinghuilouyu.cn

[D15] 去重
来源：http://ooa.jqgfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kka.smart0.xyz

PHP:  array_unique($arr);
来源：http://vtc.smart0.xyz

JS:   [...new Set(arr)]
来源：http://tun.9152youxi.cn

TS:   [...new Set(arr)]
来源：http://htt.zhiwuduotai.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://irx.jinqigfzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://nbk.dianchejie.cn

Ruby: arr.uniq
来源：http://kkk.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://ssx.daria6918.cn

[D16] 求和与平均值
来源：http://axg.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ref.vqdsnc.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gud.epnwcf.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mht.zhixingplan.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mfl.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wwj.cashguo.top

Go:   // 手写循环累加
来源：http://aid.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gti.shuidangran.top

C#:   list.Sum();  list.Average()
来源：http://iau.hesvh.cn

[D17] 最大值与最小值
来源：http://ljz.hnxiangtu.top

Py:   max(arr);  min(arr)
来源：http://zil.yj20258.top

PHP:  max($arr);  min($arr);
来源：http://irj.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://byi.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://nok.yongpay.top

Java: Collections.max(list);  Collections.min(list);
来源：http://cbk.zhengqikj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tvw.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://ryz.xziqi.cn

C#:   list.Max();  list.Min()
来源：http://bcr.wangshuangyany.cn

[D18] 扁平化嵌套数组
来源：http://uiq.vehdjk.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://igz.hcnkem.com

PHP:  array_merge(...$nested);
来源：http://uuo.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hjr.cucudq.cn

TS:   nested.flat();
来源：http://dqo.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://txe.fzhhl.top

Go:   // 手写双层循环
来源：http://erb.haohaochexian.top

Ruby: nested.flatten
来源：http://asl.jyoumei.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cpl.gaohongyu789.top

[D19] 按字段分组
来源：http://glr.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jck.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://emn.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lcl.chenlongwang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ejm.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vsy.hnqzz.top

Go:   // 手写 map[string][]T
来源：http://mht.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://bjh.guowangkeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rva.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://rqh.fzhhl.top

Py:   Counter(arr)
来源：http://grt.kuanghao11.cn

PHP:  array_count_values($arr);
来源：http://oji.fengsongda.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://roe.zycfv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hca.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://voj.meibo888.top

Go:   // 手写 map[T]int
来源：http://jwm.shangyingyoupin.top

Ruby: arr.tally
来源：http://tgs.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ojo.smart0.xyz

[D21] 判断是否包含某元素
来源：http://axi.bbcook.cn

Py:   x in arr
来源：http://lys.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://gac.tianlin.xyz

JS:   arr.includes(x)
来源：http://dtu.fzhhl.top

TS:   arr.includes(x)
来源：http://kaj.wangdashe.top

Java: list.contains(x)
来源：http://jie.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://ing.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://apc.nanxuanxn.top

C#:   list.Contains(x)
来源：http://vls.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://emm.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kum.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iwg.aizwys.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kdq.feifeiyinyue.top

TS:   [...arr];
来源：http://pva.tian-w.cn

Java: new ArrayList<>(list);
来源：http://gxb.c1oappe.top

Go:   copied := append([]int(nil), arr...)
来源：http://tyu.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://xyz.jlsjyb.cn

C#:   new List<int>(list);
来源：http://uga.ywan-chungtsiang.top

[D23] reduce 累积计算
来源：http://ftm.pycfn.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fjx.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ggz.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hqk.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nau.aibaodan.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://myw.jinqigfzy.top

Go:   // 手写循环
来源：http://itd.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dzt.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gcq.xuanzx.com

[D24] 字典 / Map 基本操作
来源：http://oyr.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fas.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wul.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bqx.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rda.ppjwa.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fmh.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qsx.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nna.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ptu.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://woh.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://awr.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mmb.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ofd.daxiang520.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cje.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qdp.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bwf.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fgv.zhengqikj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jjc.snrcjt.cn

[D26] 数组转字符串
来源：http://rlh.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://xiu.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://xnl.vehdjk.com

JS:   arr.join(", ")
来源：http://qpw.hysaishi.cn

TS:   arr.join(", ")
来源：http://oge.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://wuy.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://vde.jyoumei.cn

Ruby: arr.join(", ")
来源：http://yji.cashguo.top

C#:   string.Join(", ", list)
来源：http://wkd.ehwqpu.com

================================================================================
来源：http://maj.vehdjk.com

E. 字符串处理
来源：http://nec.ywan-chungtsiang.top

================================================================================
来源：http://yhh.yangfankeji.com

[E01] 拼接字符串
来源：http://ieq.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uwa.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zns.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cwk.wangdashe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rqn.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ucp.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pyw.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yzx.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nls.zhixingplan.top

[E02] 重复字符串
来源：http://wis.hnqzz.top

Py:   "ab" * 3
来源：http://tgr.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://abz.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://krj.zycfv.cn

TS:   "ab".repeat(3)
来源：http://qwx.smart0.xyz

Java: "ab".repeat(3)
来源：http://wld.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://rxv.c1oappe.top

Ruby: "ab" * 3
来源：http://scn.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ctc.yj20258888.top

[E03] 截取子串
来源：http://lnm.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kvh.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bjj.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rnu.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://ley.sufxvd.cn

Java: s.substring(1, 4)
来源：http://tug.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://egp.tanke756.top

Ruby: s[1, 3];  s[1..3]
来源：http://gcl.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://tew.tianlin.xyz

[E04] 查找子串位置
来源：http://mdj.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://uor.daxiang520.top

PHP:  strpos($s, "x");
来源：http://xjc.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pop.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://iks.haohaochexian.top

Java: s.indexOf("x")
来源：http://fgl.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://kxh.vehdjk.com

Ruby: s.index("x")
来源：http://dlr.pengpengdd.cyou

C#:   s.IndexOf("x")
来源：http://nmy.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://quv.feifeiyinyue.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jmm.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cxg.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aze.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yki.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nro.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://byv.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://loh.cucudq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://okl.yfazqb.com

[E06] 替换子串
来源：http://wcn.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vvy.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://usb.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bue.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://htm.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ljq.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vcb.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oow.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://fvn.yvedp.cn

[E07] 按分隔符拆分
来源：http://pny.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iif.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qxj.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://zii.fzhhl.top

TS:   s.split(",")
来源：http://zxe.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nwn.nanxinkj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nxz.guannengcc.top

Ruby: s.split(",");  s.split
来源：http://kop.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvg.jiagoushi.top

[E08] 数组按分隔符合并
来源：http://xbh.hnxiangtu.top

Py:   ",".join(items)
来源：http://zws.havefunace.top

PHP:  implode(",", $items);
来源：http://ahp.hfpthk.cn

JS:   items.join(",")
来源：http://zns.cucudq.cn

TS:   items.join(",")
来源：http://eww.feifeiyinyue.top

Java: String.join(",", items)
来源：http://fpm.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://bsf.hysaishi.cn

Ruby: items.join(",")
来源：http://yei.0kj1m.cn

C#:   string.Join(",", items)
来源：http://esc.haohaochexian.top

[E09] 去除所有空白字符
来源：http://qoc.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mms.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lma.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://qzr.zycfv.cn

TS:   s.replace(/\s+/g, "")
来源：http://ehe.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://xig.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vtl.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xai.fehbvm.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://quu.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://qib.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nua.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mns.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://ysj.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://sik.sysykeji.top

Java: String.format("%03d", 7)
来源：http://ngd.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kuo.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fvh.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wzo.tian-w.cn

[E11] 反转字符串
来源：http://orp.epnwcf.com

Py:   s[::-1]
来源：http://kqy.tianlin.xyz

PHP:  strrev($s);
来源：http://pwv.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://wiv.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://dox.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://obo.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vji.chenlongwang.top

Ruby: s.reverse
来源：http://deq.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://kub.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://ytd.tarul.cn

Py:   s.count("a")
来源：http://bna.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://kry.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://fdg.meibo888.top

TS:   s.split("a").length - 1
来源：http://rsh.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qzk.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://iaw.yonumen.top

Ruby: s.count("a")
来源：http://lpn.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://kop.shzxlz.cn

[E13] 逐字符遍历
来源：http://uix.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://eqw.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://elb.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ksd.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fcr.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jmb.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://scr.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yab.ydjk.org.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wkv.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://vxz.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://phm.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zig.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qsz.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aoi.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tot.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jzx.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pzv.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eei.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://yih.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xmr.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ukn.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gho.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lxl.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gfz.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pbw.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://woz.andypj.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qmo.yueranfly.top

[E16] 数字千分位
来源：http://uhh.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://pbn.yongpay.top

PHP:  number_format(1234567);
来源：http://dzx.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vck.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xhc.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qhu.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uek.ctjpmb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://luv.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://tur.epnwcf.com

[E17] 首字母大写
来源：http://mdt.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rte.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cts.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ibi.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mkj.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iyj.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://opz.yanxiufei.cn

Ruby: s.capitalize
来源：http://kfg.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mde.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://gea.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nls.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nts.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pok.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nky.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tck.epnwcf.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vum.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ges.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sck.andypj.xyz

[E19] 多行文本按行拆分
来源：http://cwz.hcnkem.com

Py:   s.splitlines()
来源：http://otx.yangfankeji.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wco.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://ret.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://cpq.epnwcf.com

Java: s.lines().toList()
来源：http://sxb.hammf.cn

Go:   strings.Split(s, "\n")
来源：http://pcg.uphjek.com

Ruby: s.lines
来源：http://aro.guowangkeji.top

C#:   s.Split('\n')
来源：http://nhh.hcnkem.com

[E20] 判断字符串是否为空
来源：http://pik.sweek.top

Py:   if not s:
来源：http://puv.cashguo.top


<!-- 参考信息 -->