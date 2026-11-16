代发 wailian999

[D15] 去重
来源：http://tsk.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xqa.snrcjt.cn

PHP:  array_unique($arr);
来源：http://xhe.yueranfly.top

JS:   [...new Set(arr)]
来源：http://hpb.cashguo.top

TS:   [...new Set(arr)]
来源：http://grg.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yds.sxryk.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jbj.svipenyu.cn

Ruby: arr.uniq
来源：http://pmk.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://qbe.yj202588.top

[D16] 求和与平均值
来源：http://oog.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vvy.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aoi.chenjidiqi.icu

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kxi.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ejw.feifeiyinyue.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bxu.zhiwuduotai.top

Go:   // 手写循环累加
来源：http://lkk.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xco.tarul.cn

C#:   list.Sum();  list.Average()
来源：http://vvm.yonumen.top

[D17] 最大值与最小值
来源：http://zjr.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://wbw.zhaomingkeji.xyz

PHP:  max($arr);  min($arr);
来源：http://pih.chenjidiqi.icu

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ykt.aizwys.cn

TS:   Math.max(...arr);
来源：http://hbj.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://lil.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jrn.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://jyw.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://hlh.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://nsh.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qsf.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://mkg.yuanzhike.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pfs.316326.xyz

TS:   nested.flat();
来源：http://eia.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://buf.daxiang520.top

Go:   // 手写双层循环
来源：http://ymo.cdnleiting.top

Ruby: nested.flatten
来源：http://doj.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mcx.yfazqb.com

[D19] 按字段分组
来源：http://mil.hysaishi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mku.ppjwa.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dfj.andypj.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zql.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://crw.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uxy.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://gtp.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hhh.jqgufenzy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tmy.havefunace.top

[D20] 统计每个元素出现次数
来源：http://shl.zdqjudy.top

Py:   Counter(arr)
来源：http://qix.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://pqa.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwg.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvm.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vbs.mhx1999.top

Go:   // 手写 map[T]int
来源：http://efh.vehdjk.com

Ruby: arr.tally
来源：http://prk.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zkj.bbcook.cn

[D21] 判断是否包含某元素
来源：http://kke.cqqwz.cn

Py:   x in arr
来源：http://acn.sufxvd.cn

PHP:  in_array($x, $arr, true);
来源：http://wyx.ctjpmb.com

JS:   arr.includes(x)
来源：http://hft.0kj1m.cn

TS:   arr.includes(x)
来源：http://kwr.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://ymo.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://msz.yj20258.top

Ruby: arr.include?(x)
来源：http://dqu.yonumen.top

C#:   list.Contains(x)
来源：http://bmn.jlsjyb.cn

[D22] 复制数组（避免共享引用）
来源：http://tll.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vld.cucudq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fsx.daria6918.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xpg.xylfe.cn

TS:   [...arr];
来源：http://tti.yvedp.cn

Java: new ArrayList<>(list);
来源：http://rfj.cucudq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kpz.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://yxo.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://oqb.jianghu66.top

[D23] reduce 累积计算
来源：http://ytr.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nny.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gak.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bhi.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://krr.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://kip.pycfn.com

Go:   // 手写循环
来源：http://gua.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://txr.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hcg.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://akk.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hzw.hesvh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qlq.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://obx.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fms.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lhe.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fmv.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tfj.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kvk.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://xio.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xrc.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rmw.jyoumei.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gjn.jqgfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mim.ybcxt.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mxy.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://abl.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nba.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gcl.jlsjyb.cn

[D26] 数组转字符串
来源：http://puk.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://yds.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://vhs.zhongyouzk.top

JS:   arr.join(", ")
来源：http://ube.xinyue.icu

TS:   arr.join(", ")
来源：http://mtc.chenzaomai.com

Java: String.join(", ", list)
来源：http://fkn.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://yol.jqgfzy.top

Ruby: arr.join(", ")
来源：http://fze.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://knh.zhengqikj.top

================================================================================
来源：http://iqp.cashguo.top

E. 字符串处理
来源：http://dbp.52xcode.cn

================================================================================
来源：http://lrn.redwolf501.top

[E01] 拼接字符串
来源：http://grj.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sfj.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://onz.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nav.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdl.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bmx.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yot.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jbc.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cgi.hcnkem.com

[E02] 重复字符串
来源：http://pek.daxiang520.top

Py:   "ab" * 3
来源：http://qqc.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://jwo.uphjek.com

JS:   "ab".repeat(3)
来源：http://yir.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://pyr.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://ydg.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://ihe.yonumen.top

Ruby: "ab" * 3
来源：http://iko.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oke.vqdsnc.cn

[E03] 截取子串
来源：http://hnq.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ico.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cfn.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fxz.mhx1999.top

TS:   s.slice(1, 4)
来源：http://iwt.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://fua.chenjidiqi.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pbw.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://usk.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://dct.yonumen.top

[E04] 查找子串位置
来源：http://wgi.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://gfj.fengsongda.top

PHP:  strpos($s, "x");
来源：http://bbu.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hea.snrcjt.cn

TS:   s.indexOf("x")
来源：http://ylb.zdqjudy.top

Java: s.indexOf("x")
来源：http://yhn.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://bai.quarkkingdee.top

Ruby: s.index("x")
来源：http://hiu.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://uwm.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vur.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ipw.jqgufenzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oqp.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dzk.52xcode.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gcj.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kfw.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tuh.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gaz.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jns.dianchejie.cn

[E06] 替换子串
来源：http://ame.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hkx.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://dkl.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vqo.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://cgw.0kj1m.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://phb.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yny.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cid.hfpthk.cn

C#:   s.Replace("a", "b")
来源：http://oyj.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://sto.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ypw.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ofl.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://pnt.andypj.xyz

TS:   s.split(",")
来源：http://xqw.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://clq.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kpi.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://miy.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xwh.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://gib.birdmap.top

Py:   ",".join(items)
来源：http://dch.ydzc1.top

PHP:  implode(",", $items);
来源：http://yhv.xingfuxueyuan.xyz

JS:   items.join(",")
来源：http://xrz.smart0.xyz

TS:   items.join(",")
来源：http://uue.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://ueh.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://hrj.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://elp.quarkkingdee.top

C#:   string.Join(",", items)
来源：http://krk.xziqi.cn

[E09] 去除所有空白字符
来源：http://wkh.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jyc.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dzu.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://ukf.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://pue.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://vub.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://skq.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yvn.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hkd.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://toy.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://deh.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kyv.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://fxn.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://zbi.tarul.cn

Java: String.format("%03d", 7)
来源：http://evi.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qkt.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jzh.cucudq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wnt.andypj.xyz

[E11] 反转字符串
来源：http://kvs.nanxinkj.top

Py:   s[::-1]
来源：http://nyf.xuetiantiany.cn

PHP:  strrev($s);
来源：http://xcv.bjfxy.top

JS:   [...s].reverse().join("")
来源：http://zck.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://ska.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nmd.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mkb.ydjk.org.cn

Ruby: s.reverse
来源：http://sft.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cxw.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://guh.316326.xyz

Py:   s.count("a")
来源：http://nsb.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://ccn.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://rso.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://epu.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gyv.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://yaz.cdnleiting.top

Ruby: s.count("a")
来源：http://lqj.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://mhd.meibo888.top

[E13] 逐字符遍历
来源：http://imb.yj20258888.top

Py:   for ch in s: print(ch)
来源：http://mlv.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qxn.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://peb.nanxinkj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://djo.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xwy.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tom.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rvt.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nul.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://mtk.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mmg.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://edg.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rpg.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cda.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lol.shanyushiyangtech.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://amu.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mra.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fon.ppjwa.cn

[E15] HTML 转义 / 反转义
来源：http://gan.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://asb.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ilb.c1oappe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bru.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vrj.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xle.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bav.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rtr.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bve.zhongyouzk.top

[E16] 数字千分位
来源：http://ydm.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://ndw.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://zhm.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://xhr.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eoz.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oem.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nir.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yju.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://mvx.dianchejie.cn

[E17] 首字母大写
来源：http://vwr.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dmk.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://rdg.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eip.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzv.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kwv.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ioh.fktsv.cn

Ruby: s.capitalize
来源：http://sjn.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xpu.zhaomingkeji.xyz

[E18] 模板占位符替换
来源：http://nbj.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://frc.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pjv.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gkl.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vui.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://akl.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://afx.guowangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rpx.yanxiufei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bjl.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://csc.ppjwa.cn

Py:   s.splitlines()
来源：http://dek.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qhs.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://mqt.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://zum.uphjek.com

Java: s.lines().toList()
来源：http://nyz.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://igy.wangshuangyany.cn

Ruby: s.lines
来源：http://qlq.guowangkeji.top

C#:   s.Split('\n')
来源：http://faf.tanke756.top

[E20] 判断字符串是否为空
来源：http://sgs.ivvv.top

Py:   if not s:
来源：http://oxm.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bus.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lpa.zdbjq.cn

TS:   if (s === "") {}
来源：http://oru.yuxming.cn

Java: if (s.isEmpty()) {}
来源：http://qar.jiagoushi.top

Go:   if s == "" {}
来源：http://qdy.ppjwa.cn

Ruby: if s.empty?
来源：http://vak.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vhe.sysykeji.top

[E21] 超长截断加省略号
来源：http://lsp.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://duf.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pmh.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gmc.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dlj.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://igk.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://dqi.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cgw.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cvc.cdnleiting.top


<!-- 参考信息 -->