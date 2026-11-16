代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lil.zycfv.cn

Go:   // 手写双层循环
来源：http://jiy.bjfxy.top

Ruby: nested.flatten
来源：http://cgo.hongshengwenyu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wtb.ctjpmb.com

[D19] 按字段分组
来源：http://yhz.0kj1m.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kuy.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ucj.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gmf.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://qsi.yj20258.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xgn.daxiang520.top

Go:   // 手写 map[string][]T
来源：http://qsd.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpo.zycfv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sya.dashuyun.cn

[D20] 统计每个元素出现次数
来源：http://dkq.guannengcc.top

Py:   Counter(arr)
来源：http://xdv.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://bvs.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://age.ybcxt.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wxw.ydzc1.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oca.yuxming.cn

Go:   // 手写 map[T]int
来源：http://jcg.dashuyun.cn

Ruby: arr.tally
来源：http://fbu.fengsongda.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rky.sysykeji.top

[D21] 判断是否包含某元素
来源：http://lwl.sufxvd.cn

Py:   x in arr
来源：http://bmi.jinqigfzy.top

PHP:  in_array($x, $arr, true);
来源：http://mzy.wangdashe.top

JS:   arr.includes(x)
来源：http://mpk.mhx1999.top

TS:   arr.includes(x)
来源：http://ves.xylfe.cn

Java: list.contains(x)
来源：http://tdk.jinqigufen.top

Go:   slices.Contains(arr, x)
来源：http://kma.xylfe.cn

Ruby: arr.include?(x)
来源：http://hia.52xcode.cn

C#:   list.Contains(x)
来源：http://upi.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://xjh.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xwz.yueranfly.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ttd.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rcw.shanyushiyangtech.top

TS:   [...arr];
来源：http://yjc.daria6918.cn

Java: new ArrayList<>(list);
来源：http://euu.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://zww.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://oyf.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://jko.birdmap.top

[D23] reduce 累积计算
来源：http://rii.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xpb.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tng.zdbjq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tlu.jinqigfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mlm.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ify.birdmap.top

Go:   // 手写循环
来源：http://cyw.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://scq.shanyushiyangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ggn.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://itv.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jfk.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qte.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bay.ybcxt.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://avg.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jmi.snrcjt.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lgz.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uiq.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fhp.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://bho.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyh.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://krj.aibaodan.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uaf.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gjj.hnqzz.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pnw.feifeiyinyue.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bni.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ezv.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqu.shanyushiyangkeji.top

[D26] 数组转字符串
来源：http://lzm.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://wla.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://zqz.guannengcc.top

JS:   arr.join(", ")
来源：http://xii.snrcjt.cn

TS:   arr.join(", ")
来源：http://pxt.tianlin.xyz

Java: String.join(", ", list)
来源：http://vaa.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://mmw.haohaochexian.top

Ruby: arr.join(", ")
来源：http://mkl.jinqigfzy.top

C#:   string.Join(", ", list)
来源：http://cqu.sysykeji.top

================================================================================
来源：http://btj.jlsjyb.cn

E. 字符串处理
来源：http://gwx.zdbjq.cn

================================================================================
来源：http://jzs.yangfankeji.com

[E01] 拼接字符串
来源：http://cvl.svipenyu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nxs.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xgy.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xan.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ecq.pycfn.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ucl.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bft.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jel.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lwi.cheryme.top

[E02] 重复字符串
来源：http://zjc.cqqwz.cn

Py:   "ab" * 3
来源：http://fiw.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://vjo.fzhhl.top

JS:   "ab".repeat(3)
来源：http://zto.bbcook.cn

TS:   "ab".repeat(3)
来源：http://ujh.jlsjyb.cn

Java: "ab".repeat(3)
来源：http://tlu.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://bxn.yvedp.cn

Ruby: "ab" * 3
来源：http://tfv.hnqzz.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zux.hfpthk.cn

[E03] 截取子串
来源：http://wym.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://exs.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tbr.haohaochexian.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://moy.9152youxi.cn

TS:   s.slice(1, 4)
来源：http://ejp.bjfxy.top

Java: s.substring(1, 4)
来源：http://mom.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xpx.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fmm.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://xai.gaohongyu789.top

[E04] 查找子串位置
来源：http://dsb.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://wvf.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://pvi.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ojd.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://voy.smart0.xyz

Java: s.indexOf("x")
来源：http://hsu.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://chk.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://wgp.wangdashe.top

C#:   s.IndexOf("x")
来源：http://knc.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yqb.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://khc.hysaishi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kbo.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://avr.snrcjt.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zcw.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xvu.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tse.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nlf.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hmx.zhiwuduotai.top

[E06] 替换子串
来源：http://xaa.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dmo.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://bpg.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rvr.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://zlt.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://glr.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lfa.meibo888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zbt.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://uaf.guannengcc.top

[E07] 按分隔符拆分
来源：http://bwm.hnxiangtu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fsw.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xka.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gad.hammf.cn

TS:   s.split(",")
来源：http://lgj.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://ker.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uoi.yuxming.cn

Ruby: s.split(",");  s.split
来源：http://crx.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nbr.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://ovt.bjfxy.top

Py:   ",".join(items)
来源：http://qis.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://gyw.gaohongyu789.top

JS:   items.join(",")
来源：http://jvs.ehwqpu.com

TS:   items.join(",")
来源：http://fhv.andypj.xyz

Java: String.join(",", items)
来源：http://ezc.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://anj.jinqigufen.top

Ruby: items.join(",")
来源：http://fnc.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://hix.xinyue.icu

[E09] 去除所有空白字符
来源：http://hrj.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pfd.hnqzz.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://swz.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://xib.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://qcu.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://cco.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vcc.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kfb.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ufo.hnqzz.top

[E10] 左侧补零 / 定长填充
来源：http://ivj.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lth.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tom.tarul.cn

JS:   "7".padStart(3, "0")
来源：http://fth.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://aqj.cashguo.top

Java: String.format("%03d", 7)
来源：http://szc.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ldo.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qug.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mko.mhx1999.top

[E11] 反转字符串
来源：http://tam.c1oappe.top

Py:   s[::-1]
来源：http://iiw.uphjek.com

PHP:  strrev($s);
来源：http://cdc.birdmap.top

JS:   [...s].reverse().join("")
来源：http://txt.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://wwv.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://igy.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nuc.zhengqikj.top

Ruby: s.reverse
来源：http://fad.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xyz.aizwys.cn

[E12] 统计某字符出现次数
来源：http://mlk.yongpay.top

Py:   s.count("a")
来源：http://ibn.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://eth.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://wzz.tanke756.top

TS:   s.split("a").length - 1
来源：http://six.feifeiyinyue.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vhw.quarkkingdee.top

Go:   strings.Count(s, "a")
来源：http://dno.iojbl.cn

Ruby: s.count("a")
来源：http://fwr.hcnkem.com

C#:   s.Count(c => c == 'a')
来源：http://ezz.chenzaomai.com

[E13] 逐字符遍历
来源：http://pzu.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://jbq.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xvb.yvedp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nur.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fvh.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qmi.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://biy.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://acr.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ylo.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://koa.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fcb.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://auh.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://reo.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qqy.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://iux.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ksw.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qgb.gaohongyu789.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wen.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://bzz.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pjk.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ksd.zhongyouzk.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ful.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cnh.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bgu.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fep.hnqzz.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ymh.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sou.dianchejie.cn

[E16] 数字千分位
来源：http://qkj.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://yih.cucudq.cn

PHP:  number_format(1234567);
来源：http://egh.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mnt.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://llk.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rrd.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tjf.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mgj.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://pvn.hammf.cn

[E17] 首字母大写
来源：http://vvf.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lli.hywenlv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bhq.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sdq.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ryp.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ynd.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kii.uphjek.com

Ruby: s.capitalize
来源：http://dfl.redwolf501.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wdd.jianghu66.top

[E18] 模板占位符替换
来源：http://cmt.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mjt.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://izv.9152youxi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hgt.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://gob.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rar.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zkl.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vlo.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vfm.xylfe.cn

[E19] 多行文本按行拆分
来源：http://pnj.hongshengwenyu.top

Py:   s.splitlines()
来源：http://dor.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kpp.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://qig.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://pke.9152youxi.cn

Java: s.lines().toList()
来源：http://iks.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://pvf.yonumen.top

Ruby: s.lines
来源：http://ior.snrcjt.cn

C#:   s.Split('\n')
来源：http://kbs.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://hcy.gaohongyu789.top

Py:   if not s:
来源：http://hso.yvedp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vkd.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gpd.xziqi.cn

TS:   if (s === "") {}
来源：http://zod.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://yal.jianghu66.top

Go:   if s == "" {}
来源：http://cds.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://lsv.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://agl.xziqi.cn

[E21] 超长截断加省略号
来源：http://nea.zdbjq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://srw.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qgd.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rnf.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sui.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://api.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://yfu.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fed.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://puc.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://gbh.quarkkingdee.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://usp.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://idc.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibz.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yya.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bad.tarul.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cai.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://nup.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ceb.hcnkem.com

================================================================================
来源：http://duz.jinyuanbaomall.cn

F. 文件与目录
来源：http://zgl.uphjek.com

================================================================================
来源：http://xrh.chenlongwang.top

[F01] 读取整个文件
来源：http://dbp.ehwqpu.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tdg.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://pah.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://amt.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ybb.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://rwq.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dia.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://ghp.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://lkw.nwbrower.top

[F02] 逐行读取文件
来源：http://agw.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rsh.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ken.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://twz.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://buq.xinyue.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwt.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://knq.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ryz.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ylw.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://kfi.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zhx.hysaishi.cn


<!-- 参考信息 -->