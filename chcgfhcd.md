代发 wailian999

[D15] 去重
来源：http://ugk.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://juc.hongshengwenyu.top

PHP:  array_unique($arr);
来源：http://mie.jqgfzy.top

JS:   [...new Set(arr)]
来源：http://nab.cashguo.top

TS:   [...new Set(arr)]
来源：http://yeh.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lad.zycfv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bqu.yonumen.top

Ruby: arr.uniq
来源：http://dsm.316326.xyz

C#:   list.Distinct().ToList()
来源：http://cbg.iojbl.cn

[D16] 求和与平均值
来源：http://pma.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zbs.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wex.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fpj.xziqi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ukg.snrcjt.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fuc.svipenyu.cn

Go:   // 手写循环累加
来源：http://onb.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wbf.havefunace.top

C#:   list.Sum();  list.Average()
来源：http://fng.0kj1m.cn

[D17] 最大值与最小值
来源：http://ybl.vqdsnc.cn

Py:   max(arr);  min(arr)
来源：http://wor.sufxvd.cn

PHP:  max($arr);  min($arr);
来源：http://gau.aibaodan.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vvn.52xcode.cn

TS:   Math.max(...arr);
来源：http://lfg.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://bgc.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kod.316326.xyz

Ruby: arr.max;  arr.min
来源：http://jvf.zhengqikj.top

C#:   list.Max();  list.Min()
来源：http://xvc.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://vnp.zhixingplan.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xla.cdnleiting.top

PHP:  array_merge(...$nested);
来源：http://vts.gogol.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rdq.daria6918.cn

TS:   nested.flat();
来源：http://xll.nanxinkj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hbg.fengsongda.top

Go:   // 手写双层循环
来源：http://wbg.guowangkeji.top

Ruby: nested.flatten
来源：http://ezg.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pbo.gogol.net.cn

[D19] 按字段分组
来源：http://wda.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://evn.quarkkingdee.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dtd.yj20258888.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://teq.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xni.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ezy.xziqi.cn

Go:   // 手写 map[string][]T
来源：http://usa.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vtq.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://byk.jinghuilouyu.cn

[D20] 统计每个元素出现次数
来源：http://dob.yj20258.top

Py:   Counter(arr)
来源：http://mqh.tarul.cn

PHP:  array_count_values($arr);
来源：http://gma.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvj.gotoacloud.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eej.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zof.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://ngs.jianghu66.top

Ruby: arr.tally
来源：http://egs.hysaishi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gye.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://fpx.yj20258.top

Py:   x in arr
来源：http://yvz.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://frk.havefunace.top

JS:   arr.includes(x)
来源：http://dlo.redwolf501.top

TS:   arr.includes(x)
来源：http://lld.xuetiantiany.cn

Java: list.contains(x)
来源：http://vbp.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://syc.sweek.top

Ruby: arr.include?(x)
来源：http://dsb.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://dfx.vqdsnc.cn

[D22] 复制数组（避免共享引用）
来源：http://pal.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yjb.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://adf.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ial.shzxlz.cn

TS:   [...arr];
来源：http://vkp.yvedp.cn

Java: new ArrayList<>(list);
来源：http://axz.ybcxt.top

Go:   copied := append([]int(nil), arr...)
来源：http://vyk.ppjwa.cn

Ruby: arr.dup;  arr.clone
来源：http://xww.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://iux.pycfn.com

[D23] reduce 累积计算
来源：http://unq.hywenlv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yty.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mqb.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zsa.zhaomingkeji.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tud.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vlk.zhoulong.xyz

Go:   // 手写循环
来源：http://cda.zycfv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ddt.fengsongda.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wpi.feifeiyinyue.top

[D24] 字典 / Map 基本操作
来源：http://jhv.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lnf.gzhubu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wlr.vqdsnc.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://umg.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eza.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://efy.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://paa.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dyt.jianghu66.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://apg.yonumen.top

[D25] Set 集合去重与交并差
来源：http://mht.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wmv.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vyd.hysaishi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oij.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://drx.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bqb.jqgufenzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://utl.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eex.yueranfly.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://avg.tarul.cn

[D26] 数组转字符串
来源：http://exg.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://can.ppjwa.cn

PHP:  implode(", ", $arr);
来源：http://sqp.redwolf501.top

JS:   arr.join(", ")
来源：http://cye.uphjek.com

TS:   arr.join(", ")
来源：http://tms.zhixingplan.top

Java: String.join(", ", list)
来源：http://pwq.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://zjn.zhengqikj.top

Ruby: arr.join(", ")
来源：http://qhq.meibo888.top

C#:   string.Join(", ", list)
来源：http://fum.hnqzz.top

================================================================================
来源：http://enj.xylfe.cn

E. 字符串处理
来源：http://sks.yuanzhike.top

================================================================================
来源：http://aqd.fzhhl.top

[E01] 拼接字符串
来源：http://jdh.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jsx.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ivx.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxa.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://veb.chenjidiqi.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mfr.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jzh.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cao.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sxu.hywenlv.cn

[E02] 重复字符串
来源：http://llu.yj20258888.top

Py:   "ab" * 3
来源：http://lii.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://ytx.zhaomingkeji.xyz

JS:   "ab".repeat(3)
来源：http://scm.ivvv.top

TS:   "ab".repeat(3)
来源：http://yed.gogol.net.cn

Java: "ab".repeat(3)
来源：http://pvz.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://ybv.nwbrower.top

Ruby: "ab" * 3
来源：http://jyw.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lux.yanxiufei.cn

[E03] 截取子串
来源：http://aot.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://suy.bjfxy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eib.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cxf.hcnkem.com

TS:   s.slice(1, 4)
来源：http://uvq.zhixingplan.top

Java: s.substring(1, 4)
来源：http://vzd.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cpc.bbcook.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qle.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://ksb.gotoacloud.top

[E04] 查找子串位置
来源：http://fcf.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://axe.yuxming.cn

PHP:  strpos($s, "x");
来源：http://mxl.chenlongwang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://why.yangfankeji.com

TS:   s.indexOf("x")
来源：http://vhx.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://whm.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://tcs.zhengqikj.top

Ruby: s.index("x")
来源：http://vye.wangshuangyany.cn

C#:   s.IndexOf("x")
来源：http://uab.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ikv.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://krq.fengsongda.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qmw.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ynx.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ure.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dlw.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lex.shanyushiyangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cdy.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yeh.sjlbkw.cn

[E06] 替换子串
来源：http://dvr.shangyingyoupin.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lhs.zdqjudy.top

PHP:  str_replace("a", "b", $s);
来源：http://who.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aev.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://ziq.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qlg.yj20258.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rnd.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bdk.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://xke.fengsongda.top

[E07] 按分隔符拆分
来源：http://nre.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://svo.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uul.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nwi.yangfankeji.com

TS:   s.split(",")
来源：http://bca.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mnt.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://igt.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://ypp.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wwd.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://avm.hnxiangtu.top

Py:   ",".join(items)
来源：http://rmr.daxiang520.top

PHP:  implode(",", $items);
来源：http://xrg.hnxiangtu.top

JS:   items.join(",")
来源：http://rgf.nanxuanxn.top

TS:   items.join(",")
来源：http://pae.hesvh.cn

Java: String.join(",", items)
来源：http://odu.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://fmt.daxiang520.top

Ruby: items.join(",")
来源：http://sad.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://sfj.ybcxt.top

[E09] 去除所有空白字符
来源：http://hmu.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qwm.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xzp.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://ydd.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://uwx.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://mvl.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://lft.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pyh.pengpengdd.cyou

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xrz.zdqjudy.top

[E10] 左侧补零 / 定长填充
来源：http://qex.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ton.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://eyc.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://eqk.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://zrz.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://fit.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rvl.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://odh.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cle.jqgufenzy.top

[E11] 反转字符串
来源：http://atm.xylfe.cn

Py:   s[::-1]
来源：http://mia.9152youxi.cn

PHP:  strrev($s);
来源：http://yau.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://qtb.yfazqb.com

TS:   [...s].reverse().join("")
来源：http://kkg.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vpm.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://quc.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://fmb.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://jhe.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://xga.hysaishi.cn

Py:   s.count("a")
来源：http://pzb.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://hrb.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://rbz.yj202588.top

TS:   s.split("a").length - 1
来源：http://daz.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pcx.meibo888.top

Go:   strings.Count(s, "a")
来源：http://fbe.smart0.xyz

Ruby: s.count("a")
来源：http://omf.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://aks.nwbrower.top

[E13] 逐字符遍历
来源：http://oju.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://jji.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywl.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://igp.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://siq.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fwx.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://suq.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ilm.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fox.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://zuq.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://osz.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rhq.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dqe.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://svy.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pxi.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jcc.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hdt.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ivb.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://fmm.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://etv.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mqb.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aks.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xkm.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qfw.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ttr.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gab.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oyu.cheryme.top

[E16] 数字千分位
来源：http://uat.tian-w.cn

Py:   f"{1234567:,}"
来源：http://xqy.cqqwz.cn

PHP:  number_format(1234567);
来源：http://vlm.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vog.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oiv.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jyh.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bvc.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cuh.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://feb.hnqzz.top

[E17] 首字母大写
来源：http://lsv.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vkz.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ebc.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfi.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ltg.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://snz.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qak.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://lmt.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://paw.wangdashe.top

[E18] 模板占位符替换
来源：http://yyz.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tlb.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ovq.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zxo.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kxg.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cru.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ciy.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ram.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bgl.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://lqi.hywenlv.cn

Py:   s.splitlines()
来源：http://fhs.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aix.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://usr.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://mzj.xziqi.cn

Java: s.lines().toList()
来源：http://ety.tarul.cn

Go:   strings.Split(s, "\n")
来源：http://ech.haohaochexian.top

Ruby: s.lines
来源：http://rzw.vehdjk.com

C#:   s.Split('\n')
来源：http://fsi.yj20258888.top

[E20] 判断字符串是否为空
来源：http://khv.cheryme.top

Py:   if not s:
来源：http://mqa.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyh.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nym.ctjpmb.com

TS:   if (s === "") {}
来源：http://tgu.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://udq.hnqzz.top

Go:   if s == "" {}
来源：http://tom.tian-w.cn

Ruby: if s.empty?
来源：http://ndi.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://whk.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://jhx.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gfr.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://olp.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pkb.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwz.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ypo.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://gbj.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bvg.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gtx.hongshengwenyu.top


<!-- 参考信息 -->