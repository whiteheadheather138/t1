代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://cir.zhaomingkeji.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ebd.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://eyv.bbcook.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://muo.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gxc.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://qtj.zdqjudy.top

Py:   Counter(arr)
来源：http://vld.hysaishi.cn

PHP:  array_count_values($arr);
来源：http://hwt.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fiv.jinyuanbaomall.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfg.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jik.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://pxu.guannengcc.top

Ruby: arr.tally
来源：http://rtc.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ecc.shzxlz.cn

[D21] 判断是否包含某元素
来源：http://tsn.ybcxt.top

Py:   x in arr
来源：http://brn.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://djt.ehwqpu.com

JS:   arr.includes(x)
来源：http://ksr.shzxlz.cn

TS:   arr.includes(x)
来源：http://bet.nanxinkj.top

Java: list.contains(x)
来源：http://xsp.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://qiu.yfazqb.com

Ruby: arr.include?(x)
来源：http://bgj.ybcxt.top

C#:   list.Contains(x)
来源：http://eqt.nwbrower.top

[D22] 复制数组（避免共享引用）
来源：http://efr.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lst.jinyuanbaomall.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pza.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ptr.vqdsnc.cn

TS:   [...arr];
来源：http://xjn.redwolf501.top

Java: new ArrayList<>(list);
来源：http://ctj.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nmi.chenjidiqi.icu

Ruby: arr.dup;  arr.clone
来源：http://mpz.cqqwz.cn

C#:   new List<int>(list);
来源：http://ihu.jyoumei.cn

[D23] reduce 累积计算
来源：http://kxt.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://but.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xxc.fanxiaobao.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uxh.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nxb.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://svc.jqgufenzy.top

Go:   // 手写循环
来源：http://ptm.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hcd.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fdl.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://ojn.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kix.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uqp.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sjs.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yqq.aibaodan.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://swa.hongshengwenyu.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hmc.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ear.dianchejie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vuy.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://hka.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jjb.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bop.nwbrower.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gkw.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rys.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wvm.iojbl.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yym.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ork.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ano.nanxinkj.top

[D26] 数组转字符串
来源：http://hxt.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://ift.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://lwe.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://kdf.havefunace.top

TS:   arr.join(", ")
来源：http://drk.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://oox.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://omu.uphjek.com

Ruby: arr.join(", ")
来源：http://kwy.redwolf501.top

C#:   string.Join(", ", list)
来源：http://yoq.daria6918.cn

================================================================================
来源：http://fwb.xylfe.cn

E. 字符串处理
来源：http://gth.tian-w.cn

================================================================================
来源：http://tpx.hesvh.cn

[E01] 拼接字符串
来源：http://fwo.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cjs.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fta.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxl.zhaomingkeji.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oze.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pil.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://frg.xingfuxueyuan.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jlu.hcnkem.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mve.hfpthk.cn

[E02] 重复字符串
来源：http://wjm.epnwcf.com

Py:   "ab" * 3
来源：http://ump.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://cyp.vehdjk.com

JS:   "ab".repeat(3)
来源：http://flo.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://zei.snrcjt.cn

Java: "ab".repeat(3)
来源：http://amo.yfazqb.com

Go:   strings.Repeat("ab", 3)
来源：http://fcw.birdmap.top

Ruby: "ab" * 3
来源：http://xez.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bio.vehdjk.com

[E03] 截取子串
来源：http://rxe.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gnf.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hrc.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gkx.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://pkj.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://hqk.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://efp.yuanzhike.top

Ruby: s[1, 3];  s[1..3]
来源：http://avi.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://lxb.yuxming.cn

[E04] 查找子串位置
来源：http://ucn.52xcode.cn

Py:   s.find("x");  s.index("x")
来源：http://hez.cucudq.cn

PHP:  strpos($s, "x");
来源：http://try.ywan-chungtsiang.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rep.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://awo.ppjwa.cn

Java: s.indexOf("x")
来源：http://xnj.snrcjt.cn

Go:   strings.Index(s, "x")
来源：http://hvm.yangfankeji.com

Ruby: s.index("x")
来源：http://trl.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://kgo.tarul.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lcc.zhongyouzk.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://owx.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pjh.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://izi.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://our.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://phh.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xfs.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sfr.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sgu.shangyingyoupin.top

[E06] 替换子串
来源：http://mnw.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://drp.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://rcf.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://asu.andypj.xyz

TS:   s.replaceAll("a", "b")
来源：http://lan.gzhubu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lov.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://exs.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fho.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://iic.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://vnt.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://svh.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jex.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gwv.fehbvm.com

TS:   s.split(",")
来源：http://mkf.yanxiufei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ojc.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vmz.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://cry.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fcq.aizwys.cn

[E08] 数组按分隔符合并
来源：http://apf.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://atm.hnxiangtu.top

PHP:  implode(",", $items);
来源：http://xyh.yuanzhike.top

JS:   items.join(",")
来源：http://gks.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://etx.shangyingyoupin.top

Java: String.join(",", items)
来源：http://vcq.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://trv.kuanghao11.cn

Ruby: items.join(",")
来源：http://unb.hammf.cn

C#:   string.Join(",", items)
来源：http://ckd.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://tsp.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wdd.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://szz.shanyushiyangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://kup.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://xhh.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://hjd.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://phw.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://eke.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iew.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://fhc.sysykeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tzb.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hch.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://xam.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://qkl.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://jvr.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jcf.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ytk.zdbjq.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hjt.vehdjk.com

[E11] 反转字符串
来源：http://sug.sysykeji.top

Py:   s[::-1]
来源：http://onz.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://vbp.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://jye.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://tvt.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ymh.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://frt.daxiang520.top

Ruby: s.reverse
来源：http://kme.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ffj.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://zeg.snrcjt.cn

Py:   s.count("a")
来源：http://xxl.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://ljm.yj20258888.top

JS:   s.split("a").length - 1
来源：http://ytf.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://xud.smart0.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fok.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://aoy.tarul.cn

Ruby: s.count("a")
来源：http://pac.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://smg.kuanghao11.cn

[E13] 逐字符遍历
来源：http://wav.shanyushiyangkeji.top

Py:   for ch in s: print(ch)
来源：http://tie.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kfv.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://aaf.aibaodan.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bjl.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oiy.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sps.0kj1m.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cex.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lzq.cucudq.cn

[E14] URL 编码与 Base64
来源：http://nem.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iih.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://uxn.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gdj.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yeg.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tgi.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wlu.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://emt.dashuyun.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dlr.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://tla.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://eqq.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qwf.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mra.hongshengwenyu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ybq.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pfl.nwbrower.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eiq.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bln.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dnd.redwolf501.top

[E16] 数字千分位
来源：http://xpw.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://qmi.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://cyd.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://dzj.daria6918.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lgo.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yhy.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tgo.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://txu.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://sfp.sweek.top

[E17] 首字母大写
来源：http://vtx.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cze.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hob.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yoi.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://igj.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uhs.xuetiantiany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jol.gogol.net.cn

Ruby: s.capitalize
来源：http://oaw.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tgu.aizwys.cn

[E18] 模板占位符替换
来源：http://giu.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bbd.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jom.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://spt.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://afw.zhiwuduotai.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nnk.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dmt.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://txy.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tci.yfazqb.com

[E19] 多行文本按行拆分
来源：http://iuv.ybcxt.top

Py:   s.splitlines()
来源：http://pmj.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xyr.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://xhb.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://yyk.jinqigufen.top

Java: s.lines().toList()
来源：http://tmh.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://lij.birdmap.top

Ruby: s.lines
来源：http://fak.jyoumei.cn

C#:   s.Split('\n')
来源：http://lhh.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://dja.iojbl.cn

Py:   if not s:
来源：http://ohy.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mij.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mab.tarul.cn

TS:   if (s === "") {}
来源：http://hfg.feifeiyinyue.top

Java: if (s.isEmpty()) {}
来源：http://wdk.meibo888.top

Go:   if s == "" {}
来源：http://ork.hnxiangtu.top

Ruby: if s.empty?
来源：http://gox.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tbc.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://uwy.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ces.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pla.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yxz.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hpv.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xlt.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://dcs.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gwl.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eky.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://syu.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jbz.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lsk.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://beb.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qby.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cnt.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tmu.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://ivx.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ebl.zdbjq.cn

================================================================================
来源：http://snk.quarkkingdee.top

F. 文件与目录
来源：http://ads.kuanghao11.cn

================================================================================
来源：http://nzz.fktsv.cn

[F01] 读取整个文件
来源：http://pjo.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mcj.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://kec.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://boe.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zlh.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://otn.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tvb.cashguo.top

Ruby: File.read("a.txt")
来源：http://xvq.gaohongyu789.top

C#:   File.ReadAllText("a.txt");
来源：http://wgq.guowangkeji.top

[F02] 逐行读取文件
来源：http://puy.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gvc.jqgufenzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xqu.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://quy.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ltg.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vcg.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uvh.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bpy.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vhu.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://srt.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fxn.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ybr.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cao.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://veu.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cuy.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ltd.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://dtm.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yoi.pycfn.com

[F04] 追加写入文件
来源：http://bmk.birdmap.top


<!-- 参考信息 -->