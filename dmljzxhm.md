代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://psb.gaohongyu789.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tgq.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hym.tanke756.top

Go:   // 手写 map[T]int
来源：http://hox.cdnleiting.top

Ruby: arr.tally
来源：http://lsp.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ons.yj20258.top

[D21] 判断是否包含某元素
来源：http://mun.zycfv.cn

Py:   x in arr
来源：http://mhn.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://qpp.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://cpu.ivvv.top

TS:   arr.includes(x)
来源：http://okz.vehdjk.com

Java: list.contains(x)
来源：http://lzv.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://pfk.xinyue.icu

Ruby: arr.include?(x)
来源：http://amx.tian-w.cn

C#:   list.Contains(x)
来源：http://qwl.ybcxt.top

[D22] 复制数组（避免共享引用）
来源：http://uxt.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://brr.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sag.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aqa.hnqzz.top

TS:   [...arr];
来源：http://ilr.cheryme.top

Java: new ArrayList<>(list);
来源：http://uzl.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://tec.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://jfz.yj20258.top

C#:   new List<int>(list);
来源：http://ntu.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://hyk.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sez.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wlw.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tkb.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ovd.epnwcf.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://dvq.yj20258888.top

Go:   // 手写循环
来源：http://jvk.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://otv.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://grz.0kj1m.cn

[D24] 字典 / Map 基本操作
来源：http://gqq.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lby.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lqv.xingfuxueyuan.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wwe.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wym.sweek.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gtd.daxiang520.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ytw.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jui.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jay.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://oem.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ssy.havefunace.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ybb.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vlm.yonumen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ois.jlsjyb.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ebl.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://msx.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qdo.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dkw.mhx1999.top

[D26] 数组转字符串
来源：http://lrb.sufxvd.cn

Py:   ", ".join(map(str, arr))
来源：http://cyb.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://bhv.ivvv.top

JS:   arr.join(", ")
来源：http://hrf.meibo888.top

TS:   arr.join(", ")
来源：http://ynx.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://uau.epnwcf.com

Go:   strings.Join(strs, ", ")
来源：http://kux.yvedp.cn

Ruby: arr.join(", ")
来源：http://nqz.yj20258.top

C#:   string.Join(", ", list)
来源：http://ufz.yj202588.top

================================================================================
来源：http://zto.meibo888.top

E. 字符串处理
来源：http://alm.hywenlv.cn

================================================================================
来源：http://bew.tarul.cn

[E01] 拼接字符串
来源：http://qhm.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://buh.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vao.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uqp.zhoulong.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vxx.yvedp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hvf.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://edf.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xll.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kna.zhijiandao.cn

[E02] 重复字符串
来源：http://lwp.dianchejie.cn

Py:   "ab" * 3
来源：http://bcr.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://jwn.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://lxw.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://ksp.yongpay.top

Java: "ab".repeat(3)
来源：http://opw.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://ame.aibaodan.cn

Ruby: "ab" * 3
来源：http://esx.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tut.jlsjyb.cn

[E03] 截取子串
来源：http://ray.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kdr.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yyf.nanxinkj.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nxv.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://neo.yfazqb.com

Java: s.substring(1, 4)
来源：http://jzh.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zom.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://ggp.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://ejg.bjfxy.top

[E04] 查找子串位置
来源：http://ndc.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://meu.zycfv.cn

PHP:  strpos($s, "x");
来源：http://bzu.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rzp.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://ffq.yj20258888.top

Java: s.indexOf("x")
来源：http://mpg.hammf.cn

Go:   strings.Index(s, "x")
来源：http://rra.pycfn.com

Ruby: s.index("x")
来源：http://npv.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://jne.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rbs.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iiw.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://upj.jinyuanbaomall.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pic.zhengqikj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yox.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fcs.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qxe.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ymc.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uea.xylfe.cn

[E06] 替换子串
来源：http://mrv.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xmp.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://eno.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uyd.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://ldv.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ssk.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jwf.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oqa.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://pyj.shanyushiyangtech.top

[E07] 按分隔符拆分
来源：http://jhh.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://arx.ybcxt.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oxp.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vns.fzhhl.top

TS:   s.split(",")
来源：http://xuw.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ruy.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qez.hammf.cn

Ruby: s.split(",");  s.split
来源：http://iwf.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jcq.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://xxv.yueranfly.top

Py:   ",".join(items)
来源：http://zfe.fengsongda.top

PHP:  implode(",", $items);
来源：http://bbs.nanxuanxn.top

JS:   items.join(",")
来源：http://tsn.fktsv.cn

TS:   items.join(",")
来源：http://orz.ydjk.org.cn

Java: String.join(",", items)
来源：http://ygl.chenjidiqi.icu

Go:   strings.Join(items, ",")
来源：http://xru.cheryme.top

Ruby: items.join(",")
来源：http://prn.jqgfzy.top

C#:   string.Join(",", items)
来源：http://fne.cashguo.top

[E09] 去除所有空白字符
来源：http://xsv.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hxv.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gbj.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://ftl.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://quw.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://asa.hfpthk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eod.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://eed.daria6918.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wko.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://pys.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lzf.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vnj.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://kmn.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://ypa.ctjpmb.com

Java: String.format("%03d", 7)
来源：http://fzj.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jzv.cucudq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vxh.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aiy.mhx1999.top

[E11] 反转字符串
来源：http://aiz.xziqi.cn

Py:   s[::-1]
来源：http://jrs.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://lkq.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://wpi.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://adu.zhongyouzk.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vlx.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://anf.cucudq.cn

Ruby: s.reverse
来源：http://oqh.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://wst.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://tng.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://oql.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://uys.bbcook.cn

JS:   s.split("a").length - 1
来源：http://tem.smart0.xyz

TS:   s.split("a").length - 1
来源：http://ihv.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hni.sjlbkw.cn

Go:   strings.Count(s, "a")
来源：http://wtg.ybcxt.top

Ruby: s.count("a")
来源：http://nim.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://fdr.yj20258.top

[E13] 逐字符遍历
来源：http://iyb.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://gdf.aizwys.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://klj.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://udd.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qij.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iht.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sra.dianchejie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zla.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://crm.sxryk.cn

[E14] URL 编码与 Base64
来源：http://yrl.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kil.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fuh.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://avn.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://urb.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zsg.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wgo.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jot.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dbi.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://mjg.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iuw.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bha.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iuh.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uod.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hzk.sxryk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxb.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uba.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qkn.yanxiufei.cn

[E16] 数字千分位
来源：http://fep.zycfv.cn

Py:   f"{1234567:,}"
来源：http://hgc.sufxvd.cn

PHP:  number_format(1234567);
来源：http://obf.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://sfg.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ukv.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://erz.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sjn.feifeiyinyue.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://apv.meibo888.top

C#:   1234567.ToString("N0")
来源：http://ygi.daria6918.cn

[E17] 首字母大写
来源：http://wvr.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zya.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hjh.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjh.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfc.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kgt.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dsb.ywan-chungtsiang.top

Ruby: s.capitalize
来源：http://rpj.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ish.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://bpm.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mwi.xingfuxueyuan.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nji.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cug.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vcc.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yzy.zhaomingkeji.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gad.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ygr.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ebr.cashguo.top

[E19] 多行文本按行拆分
来源：http://xxc.gaohongyu789.top

Py:   s.splitlines()
来源：http://lep.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jfz.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://oaa.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://ilf.vqdsnc.cn

Java: s.lines().toList()
来源：http://pst.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://ljl.dianchejie.cn

Ruby: s.lines
来源：http://vid.ywan-chungtsiang.top

C#:   s.Split('\n')
来源：http://aza.yfazqb.com

[E20] 判断字符串是否为空
来源：http://pdr.epnwcf.com

Py:   if not s:
来源：http://nbb.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zpa.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xpr.ydzc1.top

TS:   if (s === "") {}
来源：http://foa.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://xld.c1oappe.top

Go:   if s == "" {}
来源：http://kis.tianlin.xyz

Ruby: if s.empty?
来源：http://jlp.hesvh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://upi.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://scd.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rvh.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xcf.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oxm.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xlk.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ylw.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://ers.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://klq.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lro.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://mfz.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ihe.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jxn.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kur.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://piw.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://egu.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oee.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://rnw.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gjn.haohaochexian.top

================================================================================
来源：http://oih.aizwys.cn

F. 文件与目录
来源：http://jzl.ehwqpu.com

================================================================================
来源：http://wyh.yonumen.top

[F01] 读取整个文件
来源：http://dhc.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fzp.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://pbw.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yxn.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vbj.jinghuilouyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fco.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iuj.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://axo.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://xdi.jqgfzy.top

[F02] 逐行读取文件
来源：http://qpb.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vly.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cjh.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hvq.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fhq.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://clg.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pwm.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ige.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://soj.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://kia.jqgufenzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ulk.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ozz.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jas.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijw.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ddi.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gna.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://znl.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://efj.yonumen.top

[F04] 追加写入文件
来源：http://wis.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qah.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cha.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mue.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tjs.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://frh.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ctr.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cup.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rhb.jiagoushi.top


<!-- 参考信息 -->