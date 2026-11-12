代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cuh.jinghuilouyu.cn

Go:   // 手写双层循环
来源：http://thb.tian-w.cn

Ruby: nested.flatten
来源：http://myf.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://elp.haohaochexian.top

[D19] 按字段分组
来源：http://lkv.nanxinkj.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dof.ydzc1.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://acu.guannengcc.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hom.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wem.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nux.cheryme.top

Go:   // 手写 map[string][]T
来源：http://zjw.shanyushiyangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://lkn.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yol.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://zvz.iojbl.cn

Py:   Counter(arr)
来源：http://zvz.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://jgo.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjw.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cvh.snrcjt.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vvf.xuetiantiany.cn

Go:   // 手写 map[T]int
来源：http://wft.cdnleiting.top

Ruby: arr.tally
来源：http://hun.hammf.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vhz.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://bvv.jqgufenzy.top

Py:   x in arr
来源：http://mif.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://ywm.cdnleiting.top

JS:   arr.includes(x)
来源：http://zss.yueranfly.top

TS:   arr.includes(x)
来源：http://ubl.redwolf501.top

Java: list.contains(x)
来源：http://rjc.yj202588.top

Go:   slices.Contains(arr, x)
来源：http://dzv.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://dxc.havefunace.top

C#:   list.Contains(x)
来源：http://pos.jinqigufen.top

[D22] 复制数组（避免共享引用）
来源：http://nog.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xyz.yj202588.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ibi.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qvv.bbcook.cn

TS:   [...arr];
来源：http://zfy.wangdashe.top

Java: new ArrayList<>(list);
来源：http://wxf.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://rob.birdmap.top

Ruby: arr.dup;  arr.clone
来源：http://plj.yongpay.top

C#:   new List<int>(list);
来源：http://fpu.ybcxt.top

[D23] reduce 累积计算
来源：http://get.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zkw.zhixingplan.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lqp.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dpq.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dok.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uza.xziqi.cn

Go:   // 手写循环
来源：http://hvw.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://epo.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rzm.xylfe.cn

[D24] 字典 / Map 基本操作
来源：http://jpu.snrcjt.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ncc.feifeiyinyue.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qdx.fanxiaobao.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mmd.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cru.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fjy.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eam.zdqjudy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jgo.yanxiufei.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nof.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://evl.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://per.hnxiangtu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cdg.shangyingyoupin.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lrf.yueranfly.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jok.birdmap.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jku.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mni.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fpx.sufxvd.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ozz.redwolf501.top

[D26] 数组转字符串
来源：http://hxj.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://omd.xziqi.cn

PHP:  implode(", ", $arr);
来源：http://lkb.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://cjw.kuanghao11.cn

TS:   arr.join(", ")
来源：http://omf.ybcxt.top

Java: String.join(", ", list)
来源：http://luu.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://hvx.ywan-chungtsiang.top

Ruby: arr.join(", ")
来源：http://dtf.nanxuanxn.top

C#:   string.Join(", ", list)
来源：http://mvv.ctjpmb.com

================================================================================
来源：http://ozi.yueranfly.top

E. 字符串处理
来源：http://enc.fehbvm.com

================================================================================
来源：http://gwl.tian-w.cn

[E01] 拼接字符串
来源：http://fhr.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kcf.52xcode.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tgj.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://smo.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gim.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uch.xylfe.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wln.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gtr.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fgb.ppjwa.cn

[E02] 重复字符串
来源：http://anx.gogol.net.cn

Py:   "ab" * 3
来源：http://adh.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://lbp.uphjek.com

JS:   "ab".repeat(3)
来源：http://vck.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://yow.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://kgc.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://tzj.zhoulong.xyz

Ruby: "ab" * 3
来源：http://mfv.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qiv.yj20258888.top

[E03] 截取子串
来源：http://cbj.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kst.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pfa.havefunace.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yyc.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://mhk.wangdashe.top

Java: s.substring(1, 4)
来源：http://eft.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dqw.shzxlz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vqk.cheryme.top

C#:   s.Substring(1, 3)
来源：http://gxd.dashuyun.cn

[E04] 查找子串位置
来源：http://gjr.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://dyi.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://qcw.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ylv.ppjwa.cn

TS:   s.indexOf("x")
来源：http://cvj.sufxvd.cn

Java: s.indexOf("x")
来源：http://cxl.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://krl.yj202588.top

Ruby: s.index("x")
来源：http://pui.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://urb.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://hin.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ilb.shanyushiyangtech.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bmy.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uki.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qsm.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qzt.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://htq.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vqh.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cls.gzhubu.top

[E06] 替换子串
来源：http://igf.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nfn.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://pzg.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vfw.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://vct.birdmap.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ssp.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vgj.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mey.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://cxu.jqgfzy.top

[E07] 按分隔符拆分
来源：http://swj.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bos.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gry.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dkf.cdnleiting.top

TS:   s.split(",")
来源：http://kby.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://eis.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qre.yj202588.top

Ruby: s.split(",");  s.split
来源：http://nqk.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://scd.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://qmi.nanxuanxn.top

Py:   ",".join(items)
来源：http://joz.epnwcf.com

PHP:  implode(",", $items);
来源：http://hsm.fengsongda.top

JS:   items.join(",")
来源：http://ryk.pengpengdd.cyou

TS:   items.join(",")
来源：http://yuz.yvedp.cn

Java: String.join(",", items)
来源：http://bnr.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://lao.dianchejie.cn

Ruby: items.join(",")
来源：http://xlc.yongpay.top

C#:   string.Join(",", items)
来源：http://aoj.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://odf.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fpf.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hvq.fktsv.cn

JS:   s.replace(/\s+/g, "")
来源：http://gtr.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://wer.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://aby.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gpx.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://aqy.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yag.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://gey.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xzz.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fst.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://mxc.cheryme.top

TS:   "7".padStart(3, "0")
来源：http://xfv.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://cnq.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fmh.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ghx.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zoi.zdqjudy.top

[E11] 反转字符串
来源：http://eah.hnxiangtu.top

Py:   s[::-1]
来源：http://biq.jiagoushi.top

PHP:  strrev($s);
来源：http://wva.hesvh.cn

JS:   [...s].reverse().join("")
来源：http://vac.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://bgz.redwolf501.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yoz.zhongyouzk.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nrw.aibaodan.cn

Ruby: s.reverse
来源：http://xym.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://igt.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://xih.mhx1999.top

Py:   s.count("a")
来源：http://htc.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://ube.jianghu66.top

JS:   s.split("a").length - 1
来源：http://tqp.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://osy.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fjt.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://taw.zhiwuduotai.top

Ruby: s.count("a")
来源：http://itc.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://vnp.tarul.cn

[E13] 逐字符遍历
来源：http://ztp.bbcook.cn

Py:   for ch in s: print(ch)
来源：http://hja.gaohongyu789.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kym.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uvj.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fti.wangdashe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dfm.chenzaomai.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://noq.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cis.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mpc.xinyue.icu

[E14] URL 编码与 Base64
来源：http://vyy.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zde.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ivj.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qwj.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ufc.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyj.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdl.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rlx.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dtx.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://ysm.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://clr.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hxc.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nub.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bgi.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://quc.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kri.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cml.smart0.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ymr.cheryme.top

[E16] 数字千分位
来源：http://pkx.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://lyn.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://hek.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jew.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mhu.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rqh.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pcf.shangyingyoupin.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cyz.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://cgu.feifeiyinyue.top

[E17] 首字母大写
来源：http://uto.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pbq.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gns.shzxlz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovw.zhoulong.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://soq.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rdh.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kuh.cashguo.top

Ruby: s.capitalize
来源：http://xqg.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dbt.cucudq.cn

[E18] 模板占位符替换
来源：http://cig.bjfxy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://off.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kii.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ztm.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://twf.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iwt.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dsq.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hhd.gotoacloud.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ktz.cdnleiting.top

[E19] 多行文本按行拆分
来源：http://ayi.yongpay.top

Py:   s.splitlines()
来源：http://rpr.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zad.316326.xyz

JS:   s.split(/\r?\n/)
来源：http://bdu.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://wpj.bbcook.cn

Java: s.lines().toList()
来源：http://nic.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://hot.yangfankeji.com

Ruby: s.lines
来源：http://qzt.gaohongyu789.top

C#:   s.Split('\n')
来源：http://syq.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://ryt.yj202588.top

Py:   if not s:
来源：http://qnp.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gvq.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fjb.tarul.cn

TS:   if (s === "") {}
来源：http://avv.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://gvp.aizwys.cn

Go:   if s == "" {}
来源：http://awc.hammf.cn

Ruby: if s.empty?
来源：http://utg.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sks.yvedp.cn

[E21] 超长截断加省略号
来源：http://ynd.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cxp.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pdj.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://byu.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cft.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://quv.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://qga.fanxiaobao.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qrj.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eum.guannengcc.top

[E22] 字节长度与字符长度
来源：http://hma.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iqh.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nau.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://giz.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrm.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ctk.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oyc.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://wxc.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://glt.shangyingyoupin.top

================================================================================
来源：http://yqq.quarkkingdee.top

F. 文件与目录
来源：http://sxt.yangfankeji.com

================================================================================
来源：http://bpi.wangshuangyany.cn

[F01] 读取整个文件
来源：http://yeh.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vwe.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://qhn.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ddm.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ojf.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://syj.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vro.hesvh.cn

Ruby: File.read("a.txt")
来源：http://bgv.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://nga.nwbrower.top

[F02] 逐行读取文件
来源：http://fvv.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://keh.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zmr.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://svw.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spr.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://quh.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hox.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dvo.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vif.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://rxp.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ogj.hcnkem.com


<!-- 参考信息 -->