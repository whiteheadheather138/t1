代发 wailian999

TS:   [...new Set(arr)]
来源：http://zpt.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://axl.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://ugq.nwbrower.top

Ruby: arr.uniq
来源：http://aky.tanke756.top

C#:   list.Distinct().ToList()
来源：http://nsm.yuxming.cn

[D16] 求和与平均值
来源：http://jdm.bjfxy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://udm.sufxvd.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://keo.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nde.mhx1999.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mwt.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lay.gzhubu.top

Go:   // 手写循环累加
来源：http://the.cucudq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://arx.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://vql.zhijiandao.cn

[D17] 最大值与最小值
来源：http://ain.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://rrl.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://kfb.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ngj.ydzc1.top

TS:   Math.max(...arr);
来源：http://cid.sjlbkw.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ifh.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ipz.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://lep.yonumen.top

C#:   list.Max();  list.Min()
来源：http://eps.316326.xyz

[D18] 扁平化嵌套数组
来源：http://vtp.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://won.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://qxr.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ngs.haohaochexian.top

TS:   nested.flat();
来源：http://qtj.chenjidiqi.icu

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hjv.gogol.net.cn

Go:   // 手写双层循环
来源：http://cti.zhoulong.xyz

Ruby: nested.flatten
来源：http://hvy.fzhhl.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kzi.52xcode.cn

[D19] 按字段分组
来源：http://uvn.wangshuangyany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kbj.tianlin.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wlw.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://afb.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jxg.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jhy.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://ysa.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fcn.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vay.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://dgw.dashuyun.cn

Py:   Counter(arr)
来源：http://asi.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://zdz.yj20258888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qnf.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://son.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://twu.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://tth.redwolf501.top

Ruby: arr.tally
来源：http://azl.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fxo.aizwys.cn

[D21] 判断是否包含某元素
来源：http://lwh.zhixingplan.top

Py:   x in arr
来源：http://blx.pycfn.com

PHP:  in_array($x, $arr, true);
来源：http://gos.tian-w.cn

JS:   arr.includes(x)
来源：http://qqb.xuetiantiany.cn

TS:   arr.includes(x)
来源：http://siv.feifeiyinyue.top

Java: list.contains(x)
来源：http://zjz.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://zvm.yuanzhike.top

Ruby: arr.include?(x)
来源：http://any.dianchejie.cn

C#:   list.Contains(x)
来源：http://weh.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://wqy.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xfq.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://usq.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bne.havefunace.top

TS:   [...arr];
来源：http://xwg.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://ghf.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tno.jianghu66.top

Ruby: arr.dup;  arr.clone
来源：http://stk.zhaomingkeji.xyz

C#:   new List<int>(list);
来源：http://bpa.zdbjq.cn

[D23] reduce 累积计算
来源：http://wrm.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jtf.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://glw.meibo888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zbv.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zof.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sct.cashguo.top

Go:   // 手写循环
来源：http://sbk.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gdr.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://brn.epnwcf.com

[D24] 字典 / Map 基本操作
来源：http://yli.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xqr.hnxiangtu.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qxj.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yto.jqgfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gck.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jjp.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dfh.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qbo.yfazqb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ume.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://cdk.wangshuangyany.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rro.jlsjyb.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ecy.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jrk.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pwn.ivvv.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://esq.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oeq.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwo.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dkq.cheryme.top

[D26] 数组转字符串
来源：http://vjg.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://hei.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://dwl.hysaishi.cn

JS:   arr.join(", ")
来源：http://ube.epnwcf.com

TS:   arr.join(", ")
来源：http://zfe.uphjek.com

Java: String.join(", ", list)
来源：http://vvq.jyoumei.cn

Go:   strings.Join(strs, ", ")
来源：http://ftm.yuanzhike.top

Ruby: arr.join(", ")
来源：http://zeo.cheryme.top

C#:   string.Join(", ", list)
来源：http://yyo.9152youxi.cn

================================================================================
来源：http://uef.zdbjq.cn

E. 字符串处理
来源：http://qxj.havefunace.top

================================================================================
来源：http://nxv.pengpengdd.cyou

[E01] 拼接字符串
来源：http://llw.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fhm.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sfi.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuu.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vrw.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://isv.gzhubu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yop.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://idx.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lwz.hnxiangtu.top

[E02] 重复字符串
来源：http://zmc.sysykeji.top

Py:   "ab" * 3
来源：http://hcz.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://gnv.52xcode.cn

JS:   "ab".repeat(3)
来源：http://mup.gaohongyu789.top

TS:   "ab".repeat(3)
来源：http://afl.yueranfly.top

Java: "ab".repeat(3)
来源：http://dbq.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://vgb.kuanghao11.cn

Ruby: "ab" * 3
来源：http://llv.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://utt.zhoulong.xyz

[E03] 截取子串
来源：http://nta.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bny.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://foe.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jat.nwbrower.top

TS:   s.slice(1, 4)
来源：http://fmk.guowangkeji.top

Java: s.substring(1, 4)
来源：http://guj.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wdp.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://ovj.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://upa.gotoacloud.top

[E04] 查找子串位置
来源：http://bqb.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://yum.yangfankeji.com

PHP:  strpos($s, "x");
来源：http://zyb.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dxi.zdqjudy.top

TS:   s.indexOf("x")
来源：http://uas.xingfuxueyuan.xyz

Java: s.indexOf("x")
来源：http://zrq.tianlin.xyz

Go:   strings.Index(s, "x")
来源：http://unn.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://cmx.feifeiyinyue.top

C#:   s.IndexOf("x")
来源：http://zwq.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hdd.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fps.hywenlv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dao.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kxe.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://rlp.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ude.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ago.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nbx.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://spt.ybcxt.top

[E06] 替换子串
来源：http://ume.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ofi.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://rqx.shzxlz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jss.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://wgx.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vwl.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oul.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eft.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://jmd.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://fst.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://owc.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ios.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fwl.vehdjk.com

TS:   s.split(",")
来源：http://dbe.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://bel.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ybf.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://nlh.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xhg.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://jog.aizwys.cn

Py:   ",".join(items)
来源：http://ttt.ywan-chungtsiang.top

PHP:  implode(",", $items);
来源：http://ted.yfazqb.com

JS:   items.join(",")
来源：http://oeu.ydzc1.top

TS:   items.join(",")
来源：http://yvb.cucudq.cn

Java: String.join(",", items)
来源：http://vus.havefunace.top

Go:   strings.Join(items, ",")
来源：http://hlk.feifeiyinyue.top

Ruby: items.join(",")
来源：http://wez.chenlongwang.top

C#:   string.Join(",", items)
来源：http://urf.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://qta.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tes.fehbvm.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sgg.chenjidiqi.icu

JS:   s.replace(/\s+/g, "")
来源：http://ytc.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ghh.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://sor.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ufz.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vxs.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://seg.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://red.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rcw.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cku.hesvh.cn

JS:   "7".padStart(3, "0")
来源：http://hlb.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://oti.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://dgp.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bwt.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gql.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oho.ydzc1.top

[E11] 反转字符串
来源：http://ezt.hysaishi.cn

Py:   s[::-1]
来源：http://nma.guannengcc.top

PHP:  strrev($s);
来源：http://mje.meibo888.top

JS:   [...s].reverse().join("")
来源：http://ntn.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://jfq.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bii.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://knn.tanke756.top

Ruby: s.reverse
来源：http://abd.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ylf.xylfe.cn

[E12] 统计某字符出现次数
来源：http://gqh.dashuyun.cn

Py:   s.count("a")
来源：http://qwb.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://xgg.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://tkb.wangdashe.top

TS:   s.split("a").length - 1
来源：http://bpc.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jti.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://ojf.9152youxi.cn

Ruby: s.count("a")
来源：http://jba.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://jcy.yueranfly.top

[E13] 逐字符遍历
来源：http://dzu.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://qky.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pvd.cucudq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gtq.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vsl.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bko.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://shd.jinqigfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fjk.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://clp.yueranfly.top

[E14] URL 编码与 Base64
来源：http://vyn.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zwq.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://icy.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ubs.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ucu.havefunace.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yvr.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ccm.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmz.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hwb.guowangkeji.top

[E15] HTML 转义 / 反转义
来源：http://rfg.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ftu.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wjs.fanxiaobao.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pwy.xuetiantiany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hbu.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rbr.shzxlz.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ndp.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aen.dianchejie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gkv.dianchejie.cn

[E16] 数字千分位
来源：http://tby.tanke756.top

Py:   f"{1234567:,}"
来源：http://yvg.gotoacloud.top

PHP:  number_format(1234567);
来源：http://gld.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wjg.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yin.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hxf.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qtx.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gdj.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://utu.yongpay.top

[E17] 首字母大写
来源：http://zwd.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://akd.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vbq.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ihi.feifeiyinyue.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pul.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cjy.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://plq.mhx1999.top

Ruby: s.capitalize
来源：http://epf.nanxinkj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://adq.hnqzz.top

[E18] 模板占位符替换
来源：http://jkw.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://szx.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ggd.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rmw.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bbr.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sxx.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cen.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://byd.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ioi.cashguo.top

[E19] 多行文本按行拆分
来源：http://tan.vehdjk.com

Py:   s.splitlines()
来源：http://ykd.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ddm.sxryk.cn

JS:   s.split(/\r?\n/)
来源：http://vpf.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://tgw.shzxlz.cn

Java: s.lines().toList()
来源：http://pce.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://yad.zhengqikj.top

Ruby: s.lines
来源：http://rkw.yuanzhike.top

C#:   s.Split('\n')
来源：http://bgj.aizwys.cn

[E20] 判断字符串是否为空
来源：http://din.fehbvm.com

Py:   if not s:
来源：http://fpd.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tug.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xoa.haohaochexian.top

TS:   if (s === "") {}
来源：http://irh.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://hmj.zhoulong.xyz

Go:   if s == "" {}
来源：http://ifo.shzxlz.cn

Ruby: if s.empty?
来源：http://nxx.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pzw.gzhubu.top

[E21] 超长截断加省略号
来源：http://hus.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lwx.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uvd.chenlongwang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mcg.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://itr.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hty.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://jyf.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vig.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pdw.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://fmo.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uab.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvn.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hqw.haohaochexian.top


<!-- 参考信息 -->