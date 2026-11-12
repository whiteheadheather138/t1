代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xdm.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ofr.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qbr.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://mxv.ppjwa.cn

Ruby: arr.tally
来源：http://bff.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dbk.wangdashe.top

[D21] 判断是否包含某元素
来源：http://ffa.zdqjudy.top

Py:   x in arr
来源：http://tpe.cashguo.top

PHP:  in_array($x, $arr, true);
来源：http://vyf.hnqzz.top

JS:   arr.includes(x)
来源：http://ozv.hcnkem.com

TS:   arr.includes(x)
来源：http://hbd.cdnleiting.top

Java: list.contains(x)
来源：http://ekt.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://cfv.yonumen.top

Ruby: arr.include?(x)
来源：http://rls.ydjk.org.cn

C#:   list.Contains(x)
来源：http://hlg.zdqjudy.top

[D22] 复制数组（避免共享引用）
来源：http://gxo.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qoa.ydjk.org.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfv.jlsjyb.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://anh.yj20258.top

TS:   [...arr];
来源：http://lle.uphjek.com

Java: new ArrayList<>(list);
来源：http://zuk.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ygk.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://kqx.yj20258888.top

C#:   new List<int>(list);
来源：http://twl.jlsjyb.cn

[D23] reduce 累积计算
来源：http://sfz.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mxu.nwbrower.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nbc.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yuq.xingfuxueyuan.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqc.pengpengdd.cyou

Java: list.stream().reduce(0, Integer::sum)
来源：http://gbf.yj20258888.top

Go:   // 手写循环
来源：http://xbk.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zpd.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://adp.jqgufenzy.top

[D24] 字典 / Map 基本操作
来源：http://iim.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pbc.wangdashe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oto.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kwj.svipenyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pdf.c1oappe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ytn.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zul.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jcw.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://knc.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://lny.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cae.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xev.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jhn.xuetiantiany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uti.shzxlz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tez.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zly.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ofy.birdmap.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aht.cqqwz.cn

[D26] 数组转字符串
来源：http://ecl.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://nne.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://xmq.andypj.xyz

JS:   arr.join(", ")
来源：http://vzl.sufxvd.cn

TS:   arr.join(", ")
来源：http://las.shuidangran.top

Java: String.join(", ", list)
来源：http://utt.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://eux.guowangkeji.top

Ruby: arr.join(", ")
来源：http://zeb.chenlongwang.top

C#:   string.Join(", ", list)
来源：http://iby.zdbjq.cn

================================================================================
来源：http://nba.xinyue.icu

E. 字符串处理
来源：http://pcg.yanxiufei.cn

================================================================================
来源：http://hbm.shangyingyoupin.top

[E01] 拼接字符串
来源：http://qnq.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kye.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jwm.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://opk.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ktq.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oaz.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mev.gaohongyu789.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qya.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xsz.xylfe.cn

[E02] 重复字符串
来源：http://akx.0kj1m.cn

Py:   "ab" * 3
来源：http://dwl.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://him.ydzc1.top

JS:   "ab".repeat(3)
来源：http://bua.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://won.tanke756.top

Java: "ab".repeat(3)
来源：http://vuf.shangyingyoupin.top

Go:   strings.Repeat("ab", 3)
来源：http://zxx.52xcode.cn

Ruby: "ab" * 3
来源：http://vfw.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tok.pengpengdd.cyou

[E03] 截取子串
来源：http://zbn.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mth.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qyg.guowangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dvg.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://mhl.hysaishi.cn

Java: s.substring(1, 4)
来源：http://ptr.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://glx.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://umb.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://yoc.gzhubu.top

[E04] 查找子串位置
来源：http://exm.guowangkeji.top

Py:   s.find("x");  s.index("x")
来源：http://nfg.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://zui.nwbrower.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uyp.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://wij.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://oxu.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://abt.wangshuangyany.cn

Ruby: s.index("x")
来源：http://jen.shuidangran.top

C#:   s.IndexOf("x")
来源：http://lws.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qfg.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wyi.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rne.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sgw.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bfg.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qet.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xrd.chenzaomai.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ghv.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://byl.ppjwa.cn

[E06] 替换子串
来源：http://wre.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vpw.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://jit.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wpn.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://ogo.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hmz.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://boz.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ijx.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://lco.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://loh.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ftb.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://udi.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://smv.sufxvd.cn

TS:   s.split(",")
来源：http://ski.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://eon.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://czc.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://ste.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rac.xziqi.cn

[E08] 数组按分隔符合并
来源：http://ras.cucudq.cn

Py:   ",".join(items)
来源：http://bkh.zdqjudy.top

PHP:  implode(",", $items);
来源：http://jku.xuanzx.com

JS:   items.join(",")
来源：http://mys.shangyingyoupin.top

TS:   items.join(",")
来源：http://hmv.sxryk.cn

Java: String.join(",", items)
来源：http://xcw.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://bcl.yj20258.top

Ruby: items.join(",")
来源：http://qow.chenzaomai.com

C#:   string.Join(",", items)
来源：http://fjc.zhaomingkeji.xyz

[E09] 去除所有空白字符
来源：http://ptv.dianchejie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ogs.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ciq.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://pgg.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://pyr.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://gsg.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bsb.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://wtr.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uyn.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://pao.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uaw.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fgw.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://fab.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://qbl.uphjek.com

Java: String.format("%03d", 7)
来源：http://hiz.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sjs.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://abu.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://meb.0kj1m.cn

[E11] 反转字符串
来源：http://evt.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://lex.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://kxz.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://fbv.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://rxj.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://spg.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cmj.9152youxi.cn

Ruby: s.reverse
来源：http://tvk.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://pjv.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://xoa.hammf.cn

Py:   s.count("a")
来源：http://xey.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://oqk.ybcxt.top

JS:   s.split("a").length - 1
来源：http://xmj.yj202588.top

TS:   s.split("a").length - 1
来源：http://iwx.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sfu.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://zux.yueranfly.top

Ruby: s.count("a")
来源：http://imr.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://kdp.hfpthk.cn

[E13] 逐字符遍历
来源：http://iof.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://zjg.hnxiangtu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ljb.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xxm.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zsm.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://moz.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://anv.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qlk.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://epp.fehbvm.com

[E14] URL 编码与 Base64
来源：http://dez.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vtk.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rjr.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zos.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iup.daria6918.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://frl.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vsc.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oic.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bak.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://utx.svipenyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zir.sjlbkw.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vsr.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xob.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sjb.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sin.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rwn.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rux.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mqe.pengpengdd.cyou

[E16] 数字千分位
来源：http://yyb.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://fvp.birdmap.top

PHP:  number_format(1234567);
来源：http://axq.cdnleiting.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lgc.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ygh.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zvb.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yhi.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mrr.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://atx.vehdjk.com

[E17] 首字母大写
来源：http://opv.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nsj.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lia.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdy.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ydj.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://egu.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vuw.svipenyu.cn

Ruby: s.capitalize
来源：http://poh.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hcp.jqgfzy.top

[E18] 模板占位符替换
来源：http://rtg.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ouc.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yuk.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eht.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://upk.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ydt.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wiv.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ydn.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qot.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://xbr.chenjidiqi.icu

Py:   s.splitlines()
来源：http://emn.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ply.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://tqu.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://hig.pycfn.com

Java: s.lines().toList()
来源：http://lrh.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://jeq.xziqi.cn

Ruby: s.lines
来源：http://bbj.shuidangran.top

C#:   s.Split('\n')
来源：http://eyn.sweek.top

[E20] 判断字符串是否为空
来源：http://zcr.shzxlz.cn

Py:   if not s:
来源：http://isq.gotoacloud.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gfu.haohaochexian.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://veh.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://nlq.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://esm.jqgfzy.top

Go:   if s == "" {}
来源：http://coy.fktsv.cn

Ruby: if s.empty?
来源：http://pyr.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jsl.cashguo.top

[E21] 超长截断加省略号
来源：http://eej.zhengqikj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hjj.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://laj.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izn.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yjo.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sbq.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://lfc.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fip.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ogm.sweek.top

[E22] 字节长度与字符长度
来源：http://kwy.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://faw.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osy.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwb.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmc.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sms.nwbrower.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wlb.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://pxy.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ywq.redwolf501.top

================================================================================
来源：http://bzp.aizwys.cn

F. 文件与目录
来源：http://mgc.hysaishi.cn

================================================================================
来源：http://ams.guowangkeji.top

[F01] 读取整个文件
来源：http://rzs.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zbn.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://rrq.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jkk.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mqx.jinghuilouyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ekh.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zrc.ppjwa.cn

Ruby: File.read("a.txt")
来源：http://nex.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://iwr.yangfankeji.com

[F02] 逐行读取文件
来源：http://fij.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ifl.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bva.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://isg.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://drc.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hen.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iaw.xinyue.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jpj.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qtp.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://wgh.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zdq.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://reo.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qdp.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kai.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uvn.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rtz.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://sfm.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wrs.daxiang520.top

[F04] 追加写入文件
来源：http://mie.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eun.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kws.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ryg.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnw.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nwx.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://azp.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://agd.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xdn.shuidangran.top


<!-- 参考信息 -->