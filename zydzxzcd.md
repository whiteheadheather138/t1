代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://etz.sweek.top

C#:   list.Sum();  list.Average()
来源：http://lhg.jinqigfzy.top

[D17] 最大值与最小值
来源：http://pjf.nanxuanxn.top

Py:   max(arr);  min(arr)
来源：http://rqp.xuetiantiany.cn

PHP:  max($arr);  min($arr);
来源：http://bbk.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vaq.bjfxy.top

TS:   Math.max(...arr);
来源：http://aau.redwolf501.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mpl.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://usp.gogol.net.cn

Ruby: arr.max;  arr.min
来源：http://tde.zhijiandao.cn

C#:   list.Max();  list.Min()
来源：http://png.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://uuy.hcnkem.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rwv.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://cav.haohaochexian.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vfe.svipenyu.cn

TS:   nested.flat();
来源：http://opl.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hgk.yfazqb.com

Go:   // 手写双层循环
来源：http://nud.cheryme.top

Ruby: nested.flatten
来源：http://ktq.wangshuangyany.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qvh.zhixingplan.top

[D19] 按字段分组
来源：http://vnd.ybcxt.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zjv.zycfv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hop.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jdi.guannengcc.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jvf.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hwx.fengsongda.top

Go:   // 手写 map[string][]T
来源：http://nuu.zhaomingkeji.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://mls.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fnv.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://dxy.gaohongyu789.top

Py:   Counter(arr)
来源：http://lho.yfazqb.com

PHP:  array_count_values($arr);
来源：http://ith.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://prr.xingfuxueyuan.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pmy.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://erj.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://pze.hesvh.cn

Ruby: arr.tally
来源：http://xmq.uphjek.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yfw.cucudq.cn

[D21] 判断是否包含某元素
来源：http://qng.cheryme.top

Py:   x in arr
来源：http://xgk.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://bvp.xylfe.cn

JS:   arr.includes(x)
来源：http://ypf.yanxiufei.cn

TS:   arr.includes(x)
来源：http://vgd.yfazqb.com

Java: list.contains(x)
来源：http://fwh.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://vxs.yj20258.top

Ruby: arr.include?(x)
来源：http://bwr.tarul.cn

C#:   list.Contains(x)
来源：http://qbw.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://pue.hcnkem.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zzm.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fju.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://acy.redwolf501.top

TS:   [...arr];
来源：http://hmn.xingfuxueyuan.xyz

Java: new ArrayList<>(list);
来源：http://rhi.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://qng.epnwcf.com

Ruby: arr.dup;  arr.clone
来源：http://etw.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://xbg.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://ugu.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gez.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zfn.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dyz.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dik.meibo888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tnb.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://lun.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kgl.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oev.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://bli.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kae.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jrt.tian-w.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xym.ivvv.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://osk.xinyue.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qrb.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nmk.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://amn.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://slm.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://gso.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gnj.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dzp.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lrz.zdqjudy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lnr.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rct.mhx1999.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cbz.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cwg.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oye.dianchejie.cn

[D26] 数组转字符串
来源：http://sok.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://nad.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://zys.daxiang520.top

JS:   arr.join(", ")
来源：http://zfz.kuanghao11.cn

TS:   arr.join(", ")
来源：http://gob.smart0.xyz

Java: String.join(", ", list)
来源：http://ayu.feifeiyinyue.top

Go:   strings.Join(strs, ", ")
来源：http://ale.svipenyu.cn

Ruby: arr.join(", ")
来源：http://wiw.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://zly.gaohongyu789.top

================================================================================
来源：http://ssa.ppjwa.cn

E. 字符串处理
来源：http://hvq.jiagoushi.top

================================================================================
来源：http://jze.vehdjk.com

[E01] 拼接字符串
来源：http://taw.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qnk.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://aez.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hxw.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mbi.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mim.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zfy.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hof.xuetiantiany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://agq.quarkkingdee.top

[E02] 重复字符串
来源：http://eqs.ydjk.org.cn

Py:   "ab" * 3
来源：http://gzz.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://gvz.jinyuanbaomall.cn

JS:   "ab".repeat(3)
来源：http://ghn.ybcxt.top

TS:   "ab".repeat(3)
来源：http://dfl.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://ong.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://fqq.yonumen.top

Ruby: "ab" * 3
来源：http://zsl.ppjwa.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dqv.sjlbkw.cn

[E03] 截取子串
来源：http://xkm.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gwh.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://woy.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jdj.aizwys.cn

TS:   s.slice(1, 4)
来源：http://pvi.dashuyun.cn

Java: s.substring(1, 4)
来源：http://mqi.daxiang520.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bvg.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://set.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://emc.havefunace.top

[E04] 查找子串位置
来源：http://tsa.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://cky.hammf.cn

PHP:  strpos($s, "x");
来源：http://ajd.jinqigfzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hba.nwbrower.top

TS:   s.indexOf("x")
来源：http://seg.zhijiandao.cn

Java: s.indexOf("x")
来源：http://exn.shzxlz.cn

Go:   strings.Index(s, "x")
来源：http://gme.52xcode.cn

Ruby: s.index("x")
来源：http://yln.yvedp.cn

C#:   s.IndexOf("x")
来源：http://iwh.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kml.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://edq.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zio.wangdashe.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nnp.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://juz.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oqy.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uvc.dianchejie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ryu.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ark.jqgfzy.top

[E06] 替换子串
来源：http://tzr.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fzk.xinyue.icu

PHP:  str_replace("a", "b", $s);
来源：http://exz.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zdb.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://ste.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hsl.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lhr.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lmi.tarul.cn

C#:   s.Replace("a", "b")
来源：http://ray.tianlin.xyz

[E07] 按分隔符拆分
来源：http://ixe.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yzo.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yeh.xuetiantiany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://epd.bjfxy.top

TS:   s.split(",")
来源：http://vti.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wru.uphjek.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hcy.redwolf501.top

Ruby: s.split(",");  s.split
来源：http://dep.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ddv.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://wwj.zdqjudy.top

Py:   ",".join(items)
来源：http://phu.hysaishi.cn

PHP:  implode(",", $items);
来源：http://lye.pengpengdd.cyou

JS:   items.join(",")
来源：http://cjk.hesvh.cn

TS:   items.join(",")
来源：http://wof.hongshengwenyu.top

Java: String.join(",", items)
来源：http://yga.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://kdd.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://itq.316326.xyz

C#:   string.Join(",", items)
来源：http://ikw.yangfankeji.com

[E09] 去除所有空白字符
来源：http://ceg.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ksd.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mrh.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://ald.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://wbz.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://wql.iojbl.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bkm.ybcxt.top

Ruby: s.gsub(/\s+/, "")
来源：http://bdc.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iwa.yvedp.cn

[E10] 左侧补零 / 定长填充
来源：http://omq.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pon.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ifp.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://ogq.pycfn.com

TS:   "7".padStart(3, "0")
来源：http://wzk.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://ujj.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://qmn.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pum.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sgn.ehwqpu.com

[E11] 反转字符串
来源：http://zty.andypj.xyz

Py:   s[::-1]
来源：http://kfd.jqgfzy.top

PHP:  strrev($s);
来源：http://mcc.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://zbv.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://lid.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zki.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://msv.9152youxi.cn

Ruby: s.reverse
来源：http://pah.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://rlt.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://apd.hammf.cn

Py:   s.count("a")
来源：http://psp.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://cky.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://kpd.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://kkk.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ijg.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://ley.nanxuanxn.top

Ruby: s.count("a")
来源：http://cuq.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://qiw.jyoumei.cn

[E13] 逐字符遍历
来源：http://hfn.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://gjz.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vjk.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wft.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sfi.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://scd.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fmx.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oqo.wangshuangyany.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mrj.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://eon.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bus.ctjpmb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://mtq.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lol.xuetiantiany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pxg.hesvh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://npt.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rxx.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vof.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://srk.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://ifv.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://tjc.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tcj.zhijiandao.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jyi.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://voh.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://thj.zhongyouzk.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://txr.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://icd.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ght.yfazqb.com

[E16] 数字千分位
来源：http://ayt.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://tek.xziqi.cn

PHP:  number_format(1234567);
来源：http://owa.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dll.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cwb.gotoacloud.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://djt.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jqf.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zdk.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://fsl.daria6918.cn

[E17] 首字母大写
来源：http://wln.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pna.hcnkem.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qdn.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wpz.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gow.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ivl.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uvd.kuanghao11.cn

Ruby: s.capitalize
来源：http://hwv.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kzg.birdmap.top

[E18] 模板占位符替换
来源：http://cqh.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nxw.jianghu66.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hyu.jqgfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://izn.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tsg.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pzc.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kyo.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ggv.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kdi.sxryk.cn

[E19] 多行文本按行拆分
来源：http://vas.bbcook.cn

Py:   s.splitlines()
来源：http://ssu.hammf.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jxf.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://cfg.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://aei.bbcook.cn

Java: s.lines().toList()
来源：http://fwb.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://eui.jyoumei.cn

Ruby: s.lines
来源：http://ukn.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://sxt.xylfe.cn

[E20] 判断字符串是否为空
来源：http://wft.mhx1999.top

Py:   if not s:
来源：http://zyq.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://osb.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://doi.zhijiandao.cn

TS:   if (s === "") {}
来源：http://zij.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://cqc.316326.xyz

Go:   if s == "" {}
来源：http://twa.jinqigufen.top

Ruby: if s.empty?
来源：http://ssq.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wvm.fehbvm.com

[E21] 超长截断加省略号
来源：http://kic.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uab.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://naw.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cdt.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lww.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gtc.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://fqi.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hud.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://heu.gzhubu.top

[E22] 字节长度与字符长度
来源：http://izq.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ufx.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xia.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rnn.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://skb.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vvy.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ulf.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://xhn.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qcm.cdnleiting.top

================================================================================
来源：http://wcu.chenjidiqi.icu

F. 文件与目录
来源：http://utg.chenzaomai.com

================================================================================
来源：http://egx.cashguo.top

[F01] 读取整个文件
来源：http://oxi.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fzm.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://jyt.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yxz.ybcxt.top


<!-- 参考信息 -->