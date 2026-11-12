代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://omw.xuanzx.com

Go:   // 手写双层循环
来源：http://tze.tian-w.cn

Ruby: nested.flatten
来源：http://krm.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://nko.52xcode.cn

[D19] 按字段分组
来源：http://scb.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://plw.0kj1m.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ufo.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://evv.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gqs.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fmc.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://abk.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wua.tarul.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iwv.hammf.cn

[D20] 统计每个元素出现次数
来源：http://dbv.aizwys.cn

Py:   Counter(arr)
来源：http://uvr.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://xip.zhixingplan.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fiq.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hol.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vuj.yuxming.cn

Go:   // 手写 map[T]int
来源：http://czy.shangyingyoupin.top

Ruby: arr.tally
来源：http://vam.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lko.haohaochexian.top

[D21] 判断是否包含某元素
来源：http://rzf.cashguo.top

Py:   x in arr
来源：http://suw.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://xpt.mhx1999.top

JS:   arr.includes(x)
来源：http://ajz.hesvh.cn

TS:   arr.includes(x)
来源：http://fkt.sysykeji.top

Java: list.contains(x)
来源：http://cel.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://tvf.xingfuxueyuan.xyz

Ruby: arr.include?(x)
来源：http://uup.guowangkeji.top

C#:   list.Contains(x)
来源：http://nye.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://eqs.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ler.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kid.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dsq.shanyushiyangkeji.top

TS:   [...arr];
来源：http://uiu.ybcxt.top

Java: new ArrayList<>(list);
来源：http://ciq.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://xtj.ctjpmb.com

Ruby: arr.dup;  arr.clone
来源：http://qxu.ehwqpu.com

C#:   new List<int>(list);
来源：http://jxv.zhengqikj.top

[D23] reduce 累积计算
来源：http://bae.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ajo.gaohongyu789.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qqj.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rvy.xuanzx.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qoq.wangdashe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vks.pycfn.com

Go:   // 手写循环
来源：http://xfn.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cih.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://git.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://dft.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yts.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cbn.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bkr.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://isu.hywenlv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pga.hysaishi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dsr.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ztt.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fhw.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://yly.kuanghao11.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mmz.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tuu.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vcm.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cgs.quarkkingdee.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zws.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mcz.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ane.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://osm.snrcjt.cn

[D26] 数组转字符串
来源：http://uxe.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://vtz.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://qxd.yonumen.top

JS:   arr.join(", ")
来源：http://fym.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://qih.zhengqikj.top

Java: String.join(", ", list)
来源：http://gln.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://mcc.zhongyouzk.top

Ruby: arr.join(", ")
来源：http://rtb.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://nml.yongpay.top

================================================================================
来源：http://fso.9152youxi.cn

E. 字符串处理
来源：http://tzh.nanxuanxn.top

================================================================================
来源：http://pfm.tarul.cn

[E01] 拼接字符串
来源：http://iiw.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zya.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uux.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kbg.shanyushiyangtech.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ssx.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uqm.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://axi.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zye.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ooi.sysykeji.top

[E02] 重复字符串
来源：http://iqi.nanxuanxn.top

Py:   "ab" * 3
来源：http://eeo.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://mqk.hywenlv.cn

JS:   "ab".repeat(3)
来源：http://avk.hcnkem.com

TS:   "ab".repeat(3)
来源：http://flt.zhaomingkeji.xyz

Java: "ab".repeat(3)
来源：http://ulu.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://kjs.yongpay.top

Ruby: "ab" * 3
来源：http://yvm.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mcq.9152youxi.cn

[E03] 截取子串
来源：http://rlt.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://edp.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oof.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qcj.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://jcr.316326.xyz

Java: s.substring(1, 4)
来源：http://azs.ctjpmb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://inj.gaohongyu789.top

Ruby: s[1, 3];  s[1..3]
来源：http://pja.hammf.cn

C#:   s.Substring(1, 3)
来源：http://dlw.aibaodan.cn

[E04] 查找子串位置
来源：http://ujo.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://hhf.jinqigfzy.top

PHP:  strpos($s, "x");
来源：http://iju.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uur.chenlongwang.top

TS:   s.indexOf("x")
来源：http://lgm.sweek.top

Java: s.indexOf("x")
来源：http://mdi.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://sso.yuxming.cn

Ruby: s.index("x")
来源：http://vxv.ctjpmb.com

C#:   s.IndexOf("x")
来源：http://foo.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://imt.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pyz.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bhh.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xmd.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tjw.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gek.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qen.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nua.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vqc.redwolf501.top

[E06] 替换子串
来源：http://tvq.hesvh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uji.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://cpj.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhp.hesvh.cn

TS:   s.replaceAll("a", "b")
来源：http://awn.bbcook.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pei.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wom.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wfc.pengpengdd.cyou

C#:   s.Replace("a", "b")
来源：http://gmi.tianlin.xyz

[E07] 按分隔符拆分
来源：http://set.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rja.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zqd.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pzo.sxryk.cn

TS:   s.split(",")
来源：http://zvx.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://ctf.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rwj.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://bmn.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hwv.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://lvm.zdbjq.cn

Py:   ",".join(items)
来源：http://cmy.aibaodan.cn

PHP:  implode(",", $items);
来源：http://gxk.yj20258.top

JS:   items.join(",")
来源：http://alk.feifeiyinyue.top

TS:   items.join(",")
来源：http://ujf.pengpengdd.cyou

Java: String.join(",", items)
来源：http://tqb.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://efo.bbcook.cn

Ruby: items.join(",")
来源：http://onl.daxiang520.top

C#:   string.Join(",", items)
来源：http://tfc.9152youxi.cn

[E09] 去除所有空白字符
来源：http://daa.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iud.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ggl.hammf.cn

JS:   s.replace(/\s+/g, "")
来源：http://fvj.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://pca.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://mxl.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lpj.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://eef.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://edr.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://vyw.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jdf.gaohongyu789.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tpl.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://wxv.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://lgd.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://kyw.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gxb.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ysu.ywan-chungtsiang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hur.cucudq.cn

[E11] 反转字符串
来源：http://yoa.bbcook.cn

Py:   s[::-1]
来源：http://klo.meibo888.top

PHP:  strrev($s);
来源：http://pea.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://len.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://bng.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://jpx.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gjb.yfazqb.com

Ruby: s.reverse
来源：http://csc.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://ijp.daxiang520.top

[E12] 统计某字符出现次数
来源：http://ofz.havefunace.top

Py:   s.count("a")
来源：http://cfy.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://rxk.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://gog.xylfe.cn

TS:   s.split("a").length - 1
来源：http://mvc.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yav.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://trn.chenlongwang.top

Ruby: s.count("a")
来源：http://yqn.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://cef.ppjwa.cn

[E13] 逐字符遍历
来源：http://ggh.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://mnv.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://thq.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://viw.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://axs.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ktm.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcs.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://iny.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aqo.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://ulu.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iiw.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ntn.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://waj.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://txb.ctjpmb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://clt.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gxh.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://swt.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ayn.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://hen.meibo888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://taf.hnxiangtu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jdk.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vhv.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qaa.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kpw.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kwi.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pny.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dmy.yj20258888.top

[E16] 数字千分位
来源：http://feu.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://ufw.jiagoushi.top

PHP:  number_format(1234567);
来源：http://pro.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ncx.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rvi.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wtq.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ymv.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mwr.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://odw.shanyushiyangtech.top

[E17] 首字母大写
来源：http://pgo.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fot.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ugg.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uez.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uji.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ctb.aibaodan.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ykd.9152youxi.cn

Ruby: s.capitalize
来源：http://cya.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dpl.hywenlv.cn

[E18] 模板占位符替换
来源：http://uii.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yon.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://twb.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://akg.hongshengwenyu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://oku.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://otc.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dss.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nza.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dxs.xylfe.cn

[E19] 多行文本按行拆分
来源：http://slp.meibo888.top

Py:   s.splitlines()
来源：http://yiz.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qlo.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://oza.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://xcv.shangyingyoupin.top

Java: s.lines().toList()
来源：http://knz.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://ure.zhixingplan.top

Ruby: s.lines
来源：http://drx.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://zzr.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://vwh.pengpengdd.cyou

Py:   if not s:
来源：http://wxu.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eux.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jhp.jianghu66.top

TS:   if (s === "") {}
来源：http://wvi.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://ukw.sjlbkw.cn

Go:   if s == "" {}
来源：http://vvq.ctjpmb.com

Ruby: if s.empty?
来源：http://ldd.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dzw.0kj1m.cn

[E21] 超长截断加省略号
来源：http://xbf.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iyx.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wnu.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dln.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pcs.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hlk.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://dtr.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axj.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mck.hcnkem.com

[E22] 字节长度与字符长度
来源：http://vht.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ndl.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qne.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qlq.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yvp.tian-w.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qer.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yrb.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://epf.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zso.wangshuangyany.cn

================================================================================
来源：http://cmf.bjfxy.top

F. 文件与目录
来源：http://hxb.zycfv.cn

================================================================================
来源：http://dej.svipenyu.cn

[F01] 读取整个文件
来源：http://lsb.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mrf.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://doc.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nca.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zqu.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wkg.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wsp.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://scw.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://hdt.tianlin.xyz

[F02] 逐行读取文件
来源：http://gmx.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vbn.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fjh.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pkh.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpj.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oje.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rrx.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xcg.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jli.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://nwe.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zcc.fktsv.cn


<!-- 参考信息 -->