代发 wailian999

TS:   [...new Set(arr)]
来源：http://tvo.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bpj.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lrv.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://uaz.svipenyu.cn

C#:   list.Distinct().ToList()
来源：http://tal.zhengqikj.top

[D16] 求和与平均值
来源：http://pnl.zhongyouzk.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kpn.xuanzx.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sjq.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cnm.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bpq.xingfuxueyuan.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qqx.9152youxi.cn

Go:   // 手写循环累加
来源：http://qdr.aizwys.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zoe.redwolf501.top

C#:   list.Sum();  list.Average()
来源：http://kfl.jiagoushi.top

[D17] 最大值与最小值
来源：http://vcg.meibo888.top

Py:   max(arr);  min(arr)
来源：http://gqi.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://wjf.zhoulong.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cun.kuanghao11.cn

TS:   Math.max(...arr);
来源：http://zfl.fanxiaobao.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://hps.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jqq.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://ffh.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://yuh.jianghu66.top

[D18] 扁平化嵌套数组
来源：http://pfi.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bhn.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://vyq.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fcj.cheryme.top

TS:   nested.flat();
来源：http://tzs.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eig.ehwqpu.com

Go:   // 手写双层循环
来源：http://soc.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://vph.yangfankeji.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ypv.quarkkingdee.top

[D19] 按字段分组
来源：http://znz.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iqg.bjfxy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vzi.yanxiufei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qsj.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://brv.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://phm.nanxinkj.top

Go:   // 手写 map[string][]T
来源：http://fhv.pycfn.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://vxs.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wja.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://xcu.hfpthk.cn

Py:   Counter(arr)
来源：http://uuc.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://jpd.dashuyun.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cyi.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wit.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aig.daxiang520.top

Go:   // 手写 map[T]int
来源：http://eup.tianlin.xyz

Ruby: arr.tally
来源：http://dfs.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lwm.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://kqs.iojbl.cn

Py:   x in arr
来源：http://oiu.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://wqr.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://hgu.316326.xyz

TS:   arr.includes(x)
来源：http://aiz.xinyue.icu

Java: list.contains(x)
来源：http://ygn.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://xkk.cdnleiting.top

Ruby: arr.include?(x)
来源：http://fvq.aizwys.cn

C#:   list.Contains(x)
来源：http://uid.chenjidiqi.icu

[D22] 复制数组（避免共享引用）
来源：http://jlo.fengsongda.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rzz.bjfxy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vzi.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rrb.uphjek.com

TS:   [...arr];
来源：http://ukb.iojbl.cn

Java: new ArrayList<>(list);
来源：http://zth.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://kag.jinqigfzy.top

Ruby: arr.dup;  arr.clone
来源：http://gsu.wangdashe.top

C#:   new List<int>(list);
来源：http://qsd.zhixingplan.top

[D23] reduce 累积计算
来源：http://cam.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nhi.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cgx.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bsd.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://asn.jiagoushi.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cml.fehbvm.com

Go:   // 手写循环
来源：http://hdm.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://usw.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hwj.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://prf.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://apc.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://trc.fzhhl.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lrw.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fwc.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vqq.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cjv.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wls.hnxiangtu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mcl.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://fxg.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sti.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zkn.vehdjk.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lhn.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://asg.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cji.cheryme.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://seh.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uxp.fengsongda.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hrf.yuanzhike.top

[D26] 数组转字符串
来源：http://fyq.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://vbg.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://vjd.ctjpmb.com

JS:   arr.join(", ")
来源：http://ltw.guannengcc.top

TS:   arr.join(", ")
来源：http://nkg.9152youxi.cn

Java: String.join(", ", list)
来源：http://ubv.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://ufk.sufxvd.cn

Ruby: arr.join(", ")
来源：http://cpy.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://avi.zhengqikj.top

================================================================================
来源：http://jge.daria6918.cn

E. 字符串处理
来源：http://rom.shangyingyoupin.top

================================================================================
来源：http://ubn.jyoumei.cn

[E01] 拼接字符串
来源：http://udh.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ope.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ajb.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://swn.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hht.xinyue.icu

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lww.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vfe.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pah.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nku.zycfv.cn

[E02] 重复字符串
来源：http://aak.jqgufenzy.top

Py:   "ab" * 3
来源：http://ayj.yfazqb.com

PHP:  str_repeat("ab", 3);
来源：http://uoy.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://hlg.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://guu.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://lcl.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://whr.316326.xyz

Ruby: "ab" * 3
来源：http://zxv.yfazqb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://feg.c1oappe.top

[E03] 截取子串
来源：http://cpe.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hpm.iojbl.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://toq.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://geg.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://ptu.guannengcc.top

Java: s.substring(1, 4)
来源：http://isb.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ylm.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://rtf.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://mxd.bjfxy.top

[E04] 查找子串位置
来源：http://niz.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://jpb.ppjwa.cn

PHP:  strpos($s, "x");
来源：http://ryh.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ucy.shanyushiyangtech.top

TS:   s.indexOf("x")
来源：http://ybz.gogol.net.cn

Java: s.indexOf("x")
来源：http://vio.tarul.cn

Go:   strings.Index(s, "x")
来源：http://hww.guowangkeji.top

Ruby: s.index("x")
来源：http://gud.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://yqp.gaohongyu789.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ukb.bbcook.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fsn.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ngu.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcn.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wda.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hzp.cqqwz.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eve.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qsa.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nvx.hywenlv.cn

[E06] 替换子串
来源：http://lnw.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://psl.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://tei.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcf.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://spg.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xyi.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://omj.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vlq.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://afe.ybcxt.top

[E07] 按分隔符拆分
来源：http://wle.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ngq.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bik.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hmu.dashuyun.cn

TS:   s.split(",")
来源：http://rph.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://fyh.hesvh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://stn.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://zqu.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rtl.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://jdb.0kj1m.cn

Py:   ",".join(items)
来源：http://wlt.smart0.xyz

PHP:  implode(",", $items);
来源：http://tej.zhijiandao.cn

JS:   items.join(",")
来源：http://kco.dianchejie.cn

TS:   items.join(",")
来源：http://fit.yj202588.top

Java: String.join(",", items)
来源：http://qwq.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://gsa.ydjk.org.cn

Ruby: items.join(",")
来源：http://sps.sxryk.cn

C#:   string.Join(",", items)
来源：http://wxg.xuanzx.com

[E09] 去除所有空白字符
来源：http://gmp.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ctq.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypr.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://eoz.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://sjy.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://kyc.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bla.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wxv.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uxb.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://air.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yrx.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://imf.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://hxa.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://fgn.zhaomingkeji.xyz

Java: String.format("%03d", 7)
来源：http://xeb.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sej.hammf.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dsm.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pul.hywenlv.cn

[E11] 反转字符串
来源：http://zve.jinqigfzy.top

Py:   s[::-1]
来源：http://fxd.chenlongwang.top

PHP:  strrev($s);
来源：http://tsv.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://rib.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://fdo.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jfu.fehbvm.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://gft.epnwcf.com

Ruby: s.reverse
来源：http://pkr.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://epu.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://nha.yueranfly.top

Py:   s.count("a")
来源：http://cix.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://owg.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://gqv.xylfe.cn

TS:   s.split("a").length - 1
来源：http://zam.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kbp.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://tog.yj20258.top

Ruby: s.count("a")
来源：http://mcr.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://cai.gotoacloud.top

[E13] 逐字符遍历
来源：http://lwz.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://dcp.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ifk.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://obm.vehdjk.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://cex.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rdv.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vmz.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://cpq.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://whp.sysykeji.top

[E14] URL 编码与 Base64
来源：http://bnm.tian-w.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ttv.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mqv.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xdg.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wrj.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ppm.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lze.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wjg.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://atk.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://zez.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eqb.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hil.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qon.chenlongwang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tph.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://obo.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vkg.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rcp.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://brv.jiagoushi.top

[E16] 数字千分位
来源：http://hkr.cucudq.cn

Py:   f"{1234567:,}"
来源：http://evf.wangdashe.top

PHP:  number_format(1234567);
来源：http://hrk.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yjh.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qdy.ywan-chungtsiang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yug.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xgh.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rqo.52xcode.cn

C#:   1234567.ToString("N0")
来源：http://nnc.ydjk.org.cn

[E17] 首字母大写
来源：http://rnz.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gil.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hhx.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ars.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cjr.havefunace.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fov.pengpengdd.cyou

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://whf.hongshengwenyu.top

Ruby: s.capitalize
来源：http://cck.guowangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://znf.ybcxt.top

[E18] 模板占位符替换
来源：http://yor.bbcook.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://plr.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lyh.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mig.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jei.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gbu.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nco.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mhd.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dhd.cashguo.top

[E19] 多行文本按行拆分
来源：http://rhz.hnxiangtu.top

Py:   s.splitlines()
来源：http://ssh.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://htn.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://jqo.sweek.top

TS:   s.split(/\r?\n/)
来源：http://qeh.yj202588.top

Java: s.lines().toList()
来源：http://kji.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://fev.xylfe.cn

Ruby: s.lines
来源：http://cls.daria6918.cn

C#:   s.Split('\n')
来源：http://tha.vehdjk.com

[E20] 判断字符串是否为空
来源：http://rni.haohaochexian.top

Py:   if not s:
来源：http://vkv.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dgv.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jev.hcnkem.com

TS:   if (s === "") {}
来源：http://ejt.fehbvm.com

Java: if (s.isEmpty()) {}
来源：http://eql.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://est.fzhhl.top

Ruby: if s.empty?
来源：http://tna.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iot.guowangkeji.top

[E21] 超长截断加省略号
来源：http://dnp.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sjh.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ozp.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wsk.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hql.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pkh.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://rrk.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wal.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zlw.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://cql.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ihv.andypj.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mdi.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fci.ctjpmb.com


<!-- 参考信息 -->