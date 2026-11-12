代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://noj.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://spp.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lts.aizwys.cn

Go:   // 手写循环累加
来源：http://ora.zhijiandao.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fgt.0kj1m.cn

C#:   list.Sum();  list.Average()
来源：http://xkb.bjfxy.top

[D17] 最大值与最小值
来源：http://klr.hysaishi.cn

Py:   max(arr);  min(arr)
来源：http://dfq.dianchejie.cn

PHP:  max($arr);  min($arr);
来源：http://mnt.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hen.sxryk.cn

TS:   Math.max(...arr);
来源：http://qlx.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rdz.xuanzx.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gge.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://bfz.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://mdh.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://irp.zdqjudy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://prj.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://ctn.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qxy.wangshuangyany.cn

TS:   nested.flat();
来源：http://wsm.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xrs.yj20258888.top

Go:   // 手写双层循环
来源：http://gql.svipenyu.cn

Ruby: nested.flatten
来源：http://nfc.tarul.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://svx.uphjek.com

[D19] 按字段分组
来源：http://lrn.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tqj.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eyb.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wxd.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://kdc.yuxming.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mli.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://jjb.birdmap.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kqa.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sqk.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://hgn.yonumen.top

Py:   Counter(arr)
来源：http://syy.cdnleiting.top

PHP:  array_count_values($arr);
来源：http://kyq.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yps.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vpj.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sub.xylfe.cn

Go:   // 手写 map[T]int
来源：http://qqo.xingfuxueyuan.xyz

Ruby: arr.tally
来源：http://wzo.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xxi.nanxinkj.top

[D21] 判断是否包含某元素
来源：http://udi.jyoumei.cn

Py:   x in arr
来源：http://ovk.ppjwa.cn

PHP:  in_array($x, $arr, true);
来源：http://rnt.aibaodan.cn

JS:   arr.includes(x)
来源：http://wpr.chenjidiqi.icu

TS:   arr.includes(x)
来源：http://vdn.zhengqikj.top

Java: list.contains(x)
来源：http://gqf.jinghuilouyu.cn

Go:   slices.Contains(arr, x)
来源：http://ksz.iojbl.cn

Ruby: arr.include?(x)
来源：http://ysd.iojbl.cn

C#:   list.Contains(x)
来源：http://yfj.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://fac.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mif.nanxinkj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wzr.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kmy.sweek.top

TS:   [...arr];
来源：http://wzp.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://ncu.cqqwz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xei.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://wur.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://bvl.dashuyun.cn

[D23] reduce 累积计算
来源：http://eij.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bfi.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ltw.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dzx.cheryme.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nbw.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vnm.fzhhl.top

Go:   // 手写循环
来源：http://mas.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wsw.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ipm.hywenlv.cn

[D24] 字典 / Map 基本操作
来源：http://dgj.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kif.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mxz.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otu.hammf.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gmd.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nof.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://own.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rva.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jwb.yfazqb.com

[D25] Set 集合去重与交并差
来源：http://wyq.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vlt.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uih.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rvc.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pas.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://axv.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tkw.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kzf.bjfxy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgu.gaohongyu789.top

[D26] 数组转字符串
来源：http://ueh.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://ehu.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://qwu.gaohongyu789.top

JS:   arr.join(", ")
来源：http://ilf.xziqi.cn

TS:   arr.join(", ")
来源：http://jwu.yueranfly.top

Java: String.join(", ", list)
来源：http://gmw.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://hpr.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://doq.ybcxt.top

C#:   string.Join(", ", list)
来源：http://wmp.guannengcc.top

================================================================================
来源：http://pys.svipenyu.cn

E. 字符串处理
来源：http://ane.zhixingplan.top

================================================================================
来源：http://ema.bjfxy.top

[E01] 拼接字符串
来源：http://gbc.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jbf.fehbvm.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qic.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pnc.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ctm.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lyk.yanxiufei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lhn.sufxvd.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lay.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zto.tianlin.xyz

[E02] 重复字符串
来源：http://kwy.guannengcc.top

Py:   "ab" * 3
来源：http://zmn.ctjpmb.com

PHP:  str_repeat("ab", 3);
来源：http://phw.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://ugk.tanke756.top

TS:   "ab".repeat(3)
来源：http://xni.yvedp.cn

Java: "ab".repeat(3)
来源：http://shk.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://yoo.fzhhl.top

Ruby: "ab" * 3
来源：http://mlp.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uka.0kj1m.cn

[E03] 截取子串
来源：http://tiv.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://thg.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tuf.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eng.ydzc1.top

TS:   s.slice(1, 4)
来源：http://ubh.xziqi.cn

Java: s.substring(1, 4)
来源：http://hka.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pxi.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://dgr.gaohongyu789.top

C#:   s.Substring(1, 3)
来源：http://wyh.wangshuangyany.cn

[E04] 查找子串位置
来源：http://jyu.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://fyh.sxryk.cn

PHP:  strpos($s, "x");
来源：http://mdk.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://svj.chenlongwang.top

TS:   s.indexOf("x")
来源：http://pjk.ywan-chungtsiang.top

Java: s.indexOf("x")
来源：http://olw.havefunace.top

Go:   strings.Index(s, "x")
来源：http://hhc.epnwcf.com

Ruby: s.index("x")
来源：http://dop.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://kln.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://htz.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gib.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zlh.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tma.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wlz.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ddt.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wxa.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ift.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hqf.yvedp.cn

[E06] 替换子串
来源：http://shf.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gsb.svipenyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ibk.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jhr.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://evq.shangyingyoupin.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvy.fanxiaobao.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://crd.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aid.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://zut.dianchejie.cn

[E07] 按分隔符拆分
来源：http://lkm.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dlf.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gmy.mhx1999.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uoz.aibaodan.cn

TS:   s.split(",")
来源：http://lqz.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ada.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://okp.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://qrp.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rua.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://wud.feifeiyinyue.top

Py:   ",".join(items)
来源：http://gqr.gzhubu.top

PHP:  implode(",", $items);
来源：http://lfq.yangfankeji.com

JS:   items.join(",")
来源：http://mdd.ydjk.org.cn

TS:   items.join(",")
来源：http://xmf.tanke756.top

Java: String.join(",", items)
来源：http://hbs.yj20258.top

Go:   strings.Join(items, ",")
来源：http://gxu.hesvh.cn

Ruby: items.join(",")
来源：http://ojj.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://lws.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://kue.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yjq.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pmb.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://qgk.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://aem.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://ihj.fengsongda.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wlb.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://xpq.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qfg.gogol.net.cn

[E10] 左侧补零 / 定长填充
来源：http://rxy.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nxy.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wne.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://ird.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://kmv.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://gri.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ckb.yueranfly.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nxj.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bnt.zhiwuduotai.top

[E11] 反转字符串
来源：http://lkc.zhijiandao.cn

Py:   s[::-1]
来源：http://wqe.zhixingplan.top

PHP:  strrev($s);
来源：http://xog.ywan-chungtsiang.top

JS:   [...s].reverse().join("")
来源：http://ckj.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://jcl.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ptg.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://wsw.zhixingplan.top

Ruby: s.reverse
来源：http://era.pycfn.com

C#:   new string(s.Reverse().ToArray())
来源：http://bdo.smart0.xyz

[E12] 统计某字符出现次数
来源：http://bng.xuetiantiany.cn

Py:   s.count("a")
来源：http://dpv.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://urw.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://ger.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://tid.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://srv.pengpengdd.cyou

Go:   strings.Count(s, "a")
来源：http://xlw.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://xcx.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://amz.bbcook.cn

[E13] 逐字符遍历
来源：http://noq.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://zza.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cwc.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tst.xingfuxueyuan.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://gpx.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zew.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cfs.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jln.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gxn.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://gdk.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nds.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mwf.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ako.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fvy.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ylq.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eyb.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yef.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gfw.fengsongda.top

[E15] HTML 转义 / 反转义
来源：http://egf.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yxo.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tud.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://moe.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://hob.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ece.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pgr.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lra.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://obn.sxryk.cn

[E16] 数字千分位
来源：http://seo.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://rsb.shanyushiyangtech.top

PHP:  number_format(1234567);
来源：http://ale.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dqe.ivvv.top

TS:   (1234567).toLocaleString("en-US")
来源：http://srb.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kje.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dny.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dyc.havefunace.top

C#:   1234567.ToString("N0")
来源：http://wje.yj20258.top

[E17] 首字母大写
来源：http://tbs.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://igs.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ufp.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xss.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qaw.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fvo.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ktx.daxiang520.top

Ruby: s.capitalize
来源：http://lqy.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://evc.xziqi.cn

[E18] 模板占位符替换
来源：http://uss.vqdsnc.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://thu.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qjv.wangshuangyany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xyw.hnxiangtu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://chz.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xoa.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xgh.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oti.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qzr.xziqi.cn

[E19] 多行文本按行拆分
来源：http://zhm.0kj1m.cn

Py:   s.splitlines()
来源：http://ryp.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tog.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://zfd.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://qvw.redwolf501.top

Java: s.lines().toList()
来源：http://dos.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://iwe.gzhubu.top

Ruby: s.lines
来源：http://fzy.0kj1m.cn

C#:   s.Split('\n')
来源：http://ixc.epnwcf.com

[E20] 判断字符串是否为空
来源：http://add.cashguo.top

Py:   if not s:
来源：http://xnu.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgu.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wbq.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://aqy.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://asg.yonumen.top

Go:   if s == "" {}
来源：http://jgt.316326.xyz

Ruby: if s.empty?
来源：http://dzd.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tyv.aibaodan.cn

[E21] 超长截断加省略号
来源：http://cbt.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gsz.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vlo.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://myw.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qua.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ikz.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://rnh.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xab.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eku.fehbvm.com

[E22] 字节长度与字符长度
来源：http://ygf.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pnx.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dye.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tua.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eds.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rjr.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://okq.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://evx.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pmm.hesvh.cn

================================================================================
来源：http://lxh.jinyuanbaomall.cn

F. 文件与目录
来源：http://yym.fzhhl.top

================================================================================
来源：http://ibs.0kj1m.cn


<!-- 参考信息 -->