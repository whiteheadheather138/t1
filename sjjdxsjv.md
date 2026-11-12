代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://vyj.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://gci.52xcode.cn

C#:   list.Contains(x)
来源：http://geg.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://seu.hongshengwenyu.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xsm.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jcv.chenlongwang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mgv.xuanzx.com

TS:   [...arr];
来源：http://fzs.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://zuq.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://ero.zhaomingkeji.xyz

Ruby: arr.dup;  arr.clone
来源：http://qdc.hammf.cn

C#:   new List<int>(list);
来源：http://dxa.ydjk.org.cn

[D23] reduce 累积计算
来源：http://vtm.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jhh.nanxinkj.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://luz.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://egc.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://byq.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ueb.quarkkingdee.top

Go:   // 手写循环
来源：http://lvr.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ije.nwbrower.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vwf.hnqzz.top

[D24] 字典 / Map 基本操作
来源：http://hjh.sufxvd.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zsm.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://alv.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tai.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dvu.chenlongwang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gcj.vehdjk.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zql.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cfv.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vqd.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://rlm.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nkl.gzhubu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sow.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vqk.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sxy.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zgf.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gtg.ywan-chungtsiang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xxe.jinqigfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://int.zhongyouzk.top

[D26] 数组转字符串
来源：http://cyo.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://jau.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://zyq.kuanghao11.cn

JS:   arr.join(", ")
来源：http://sgg.chenzaomai.com

TS:   arr.join(", ")
来源：http://dtr.tanke756.top

Java: String.join(", ", list)
来源：http://tob.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://vef.jinqigufen.top

Ruby: arr.join(", ")
来源：http://awo.chenzaomai.com

C#:   string.Join(", ", list)
来源：http://xlg.zhongyouzk.top

================================================================================
来源：http://hsd.tarul.cn

E. 字符串处理
来源：http://kmn.cucudq.cn

================================================================================
来源：http://rbw.shzxlz.cn

[E01] 拼接字符串
来源：http://yre.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mid.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cri.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tka.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iii.yj202588.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzy.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://olh.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vqj.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kmx.jinqigfzy.top

[E02] 重复字符串
来源：http://jgs.chenlongwang.top

Py:   "ab" * 3
来源：http://qsl.jinqigufen.top

PHP:  str_repeat("ab", 3);
来源：http://rpd.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://fos.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://vpz.jinqigfzy.top

Java: "ab".repeat(3)
来源：http://wsr.yvedp.cn

Go:   strings.Repeat("ab", 3)
来源：http://gbz.yj202588.top

Ruby: "ab" * 3
来源：http://kkl.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vaf.haohaochexian.top

[E03] 截取子串
来源：http://ymf.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xyk.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kdr.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pnk.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://vuk.chenlongwang.top

Java: s.substring(1, 4)
来源：http://ixp.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jzc.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://ktz.zdqjudy.top

C#:   s.Substring(1, 3)
来源：http://ijs.daxiang520.top

[E04] 查找子串位置
来源：http://flk.quarkkingdee.top

Py:   s.find("x");  s.index("x")
来源：http://euu.andypj.xyz

PHP:  strpos($s, "x");
来源：http://yzk.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://anr.sufxvd.cn

TS:   s.indexOf("x")
来源：http://vve.tian-w.cn

Java: s.indexOf("x")
来源：http://eza.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://wtw.gzhubu.top

Ruby: s.index("x")
来源：http://alx.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://nga.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ren.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://irz.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gpn.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rwm.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tsn.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zpc.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vpn.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://now.ydzc1.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vlg.svipenyu.cn

[E06] 替换子串
来源：http://wjc.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fmd.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://ptd.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcv.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://bjo.tianlin.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://the.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gpl.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://slz.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://dom.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://bfs.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kny.hongshengwenyu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pyh.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uus.xziqi.cn

TS:   s.split(",")
来源：http://joj.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://icw.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hvw.ybcxt.top

Ruby: s.split(",");  s.split
来源：http://nco.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xja.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://euc.quarkkingdee.top

Py:   ",".join(items)
来源：http://btf.guowangkeji.top

PHP:  implode(",", $items);
来源：http://dvr.zhijiandao.cn

JS:   items.join(",")
来源：http://ndx.zhongyouzk.top

TS:   items.join(",")
来源：http://hxn.wangshuangyany.cn

Java: String.join(",", items)
来源：http://yun.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://xfy.birdmap.top

Ruby: items.join(",")
来源：http://pnc.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://bhr.nanxinkj.top

[E09] 去除所有空白字符
来源：http://pmr.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vnf.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://txi.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://cyx.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://zrr.hysaishi.cn

Java: s.replaceAll("\\s+", "")
来源：http://abn.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://dfj.yj20258888.top

Ruby: s.gsub(/\s+/, "")
来源：http://hio.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rax.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://zme.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dzn.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lmr.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://vyx.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://woy.yj20258888.top

Java: String.format("%03d", 7)
来源：http://crd.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ini.sysykeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fir.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jdr.hesvh.cn

[E11] 反转字符串
来源：http://auk.jinghuilouyu.cn

Py:   s[::-1]
来源：http://lfa.tianlin.xyz

PHP:  strrev($s);
来源：http://lyj.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://tve.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://poo.cqqwz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://poj.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xlw.wangdashe.top

Ruby: s.reverse
来源：http://gkd.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://pcg.meibo888.top

[E12] 统计某字符出现次数
来源：http://cwj.cucudq.cn

Py:   s.count("a")
来源：http://fet.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://geg.yonumen.top

JS:   s.split("a").length - 1
来源：http://tid.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://inm.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rae.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://zld.hnqzz.top

Ruby: s.count("a")
来源：http://msn.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://tdx.cashguo.top

[E13] 逐字符遍历
来源：http://ugh.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://xuo.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gpc.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gmv.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ymk.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ivl.snrcjt.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fcf.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ims.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cct.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://etq.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ibd.xuetiantiany.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nvx.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qow.0kj1m.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xoi.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ymd.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lcf.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tcm.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ikj.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://qty.wangdashe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rse.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iis.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ioe.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vnz.fengsongda.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gwf.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jqz.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://usf.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ucc.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://qva.sysykeji.top

Py:   f"{1234567:,}"
来源：http://jzu.guowangkeji.top

PHP:  number_format(1234567);
来源：http://fmk.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nse.zhoulong.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://vno.fanxiaobao.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zxz.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uqk.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jli.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://obc.zhijiandao.cn

[E17] 首字母大写
来源：http://vsu.jlsjyb.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kgm.jinghuilouyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bei.jinyuanbaomall.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lrp.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jrf.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mkc.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://axo.epnwcf.com

Ruby: s.capitalize
来源：http://jyt.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uet.yj20258.top

[E18] 模板占位符替换
来源：http://gjb.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kme.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://smw.ehwqpu.com

JS:   tpl.replaceAll("{name}", name)
来源：http://qbc.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lwl.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://stv.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zqc.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jyx.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uxe.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://tuf.hfpthk.cn

Py:   s.splitlines()
来源：http://lwp.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chl.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://wtd.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://pxe.tanke756.top

Java: s.lines().toList()
来源：http://urg.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://ipr.aizwys.cn

Ruby: s.lines
来源：http://aef.yj20258888.top

C#:   s.Split('\n')
来源：http://epc.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://aid.ivvv.top

Py:   if not s:
来源：http://qrd.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xrd.yonumen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uex.jqgfzy.top

TS:   if (s === "") {}
来源：http://yuq.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://jwh.fengsongda.top

Go:   if s == "" {}
来源：http://ean.zhixingplan.top

Ruby: if s.empty?
来源：http://rqp.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ltd.sxryk.cn

[E21] 超长截断加省略号
来源：http://uzx.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wxg.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gjn.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvd.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bst.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kbl.xinyue.icu

Go:   // 按 rune 判断长度后截断
来源：http://aja.xuetiantiany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://foz.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gml.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://xsv.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wwq.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jzq.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ekp.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pkz.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fiu.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rsh.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://zpk.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kxa.fanxiaobao.xyz

================================================================================
来源：http://nuq.zhaomingkeji.xyz

F. 文件与目录
来源：http://gxg.daria6918.cn

================================================================================
来源：http://top.birdmap.top

[F01] 读取整个文件
来源：http://zhn.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qiz.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://xib.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kuh.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://clt.hnqzz.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uho.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uoo.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://nec.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://vuz.tarul.cn

[F02] 逐行读取文件
来源：http://qyy.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mda.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ucc.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nyq.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gzu.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bgw.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lxf.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jry.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zaf.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://vpu.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://add.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hyr.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pmu.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rcp.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bgs.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ntf.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://ofh.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://orf.ydjk.org.cn

[F04] 追加写入文件
来源：http://ius.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dad.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pge.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rim.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohg.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sid.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yyx.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://orp.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eit.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://lgw.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imw.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://rsn.sxryk.cn

JS:   fs.existsSync("a.txt")
来源：http://ncu.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://hsr.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bhs.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zhm.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://yld.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://alc.zhiwuduotai.top

[F06] 删除文件
来源：http://bsd.yongpay.top

Py:   os.remove("a.txt")
来源：http://wwl.sysykeji.top

PHP:  unlink("a.txt");
来源：http://zac.cheryme.top


<!-- 参考信息 -->