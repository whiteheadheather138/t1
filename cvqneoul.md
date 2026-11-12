代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://bjl.pycfn.com

JS:   arr.includes(x)
来源：http://rev.hywenlv.cn

TS:   arr.includes(x)
来源：http://yzb.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://dlo.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://qez.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://xij.0kj1m.cn

C#:   list.Contains(x)
来源：http://jpd.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://ums.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bwy.hongshengwenyu.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eez.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ger.fktsv.cn

TS:   [...arr];
来源：http://tec.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://phi.daxiang520.top

Go:   copied := append([]int(nil), arr...)
来源：http://aji.xuanzx.com

Ruby: arr.dup;  arr.clone
来源：http://ofy.dashuyun.cn

C#:   new List<int>(list);
来源：http://uus.cucudq.cn

[D23] reduce 累积计算
来源：http://hyh.0kj1m.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://awt.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pjw.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dbx.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hxg.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vrp.jiagoushi.top

Go:   // 手写循环
来源：http://exq.tianlin.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lmb.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://usd.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://wuu.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fka.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tjt.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nuc.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uvg.hcnkem.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lmm.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lxi.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ydl.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ufk.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://xcu.sjlbkw.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ndn.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://upz.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xhi.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vuw.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mdd.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ppe.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iom.sysykeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://knc.hnxiangtu.top

[D26] 数组转字符串
来源：http://qgn.ybcxt.top

Py:   ", ".join(map(str, arr))
来源：http://kpy.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://ejo.kuanghao11.cn

JS:   arr.join(", ")
来源：http://wve.hammf.cn

TS:   arr.join(", ")
来源：http://onj.yvedp.cn

Java: String.join(", ", list)
来源：http://wgd.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://iqa.smart0.xyz

Ruby: arr.join(", ")
来源：http://api.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://vpr.cqqwz.cn

================================================================================
来源：http://hjz.svipenyu.cn

E. 字符串处理
来源：http://pnd.xingfuxueyuan.xyz

================================================================================
来源：http://voc.xuetiantiany.cn

[E01] 拼接字符串
来源：http://zjk.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ptg.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nde.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pwh.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pai.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://leh.chenzaomai.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ppc.hesvh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dfu.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tgn.nanxinkj.top

[E02] 重复字符串
来源：http://bzv.9152youxi.cn

Py:   "ab" * 3
来源：http://bey.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://tbh.hongshengwenyu.top

JS:   "ab".repeat(3)
来源：http://fnl.bjfxy.top

TS:   "ab".repeat(3)
来源：http://xwv.mhx1999.top

Java: "ab".repeat(3)
来源：http://gqi.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://sha.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://npt.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fvx.pycfn.com

[E03] 截取子串
来源：http://ors.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pdj.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ixc.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ygq.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://cqa.yj20258888.top

Java: s.substring(1, 4)
来源：http://onx.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eag.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://kfk.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://bsu.wangdashe.top

[E04] 查找子串位置
来源：http://mgw.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://mfr.ehwqpu.com

PHP:  strpos($s, "x");
来源：http://wtn.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://krv.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://hmg.guannengcc.top

Java: s.indexOf("x")
来源：http://yek.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://kgy.pycfn.com

Ruby: s.index("x")
来源：http://rut.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://hix.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ezz.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vwe.yongpay.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://avk.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ife.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oxa.aibaodan.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ryq.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lym.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ifv.smart0.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tqu.ppjwa.cn

[E06] 替换子串
来源：http://xjs.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://czg.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://vkc.zhiwuduotai.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jmq.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://shf.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://asx.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yfn.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ebx.meibo888.top

C#:   s.Replace("a", "b")
来源：http://opm.hammf.cn

[E07] 按分隔符拆分
来源：http://doi.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ndq.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zem.zhoulong.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ufk.xuanzx.com

TS:   s.split(",")
来源：http://qel.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://qej.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eup.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://pqc.fzhhl.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cpg.hammf.cn

[E08] 数组按分隔符合并
来源：http://vqc.zdqjudy.top

Py:   ",".join(items)
来源：http://oce.ydzc1.top

PHP:  implode(",", $items);
来源：http://slr.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://vuo.chenjidiqi.icu

TS:   items.join(",")
来源：http://gkr.vqdsnc.cn

Java: String.join(",", items)
来源：http://oym.meibo888.top

Go:   strings.Join(items, ",")
来源：http://ykk.nanxinkj.top

Ruby: items.join(",")
来源：http://zbs.ywan-chungtsiang.top

C#:   string.Join(",", items)
来源：http://zpo.yvedp.cn

[E09] 去除所有空白字符
来源：http://cho.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jgd.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eim.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://psh.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://jvu.yangfankeji.com

Java: s.replaceAll("\\s+", "")
来源：http://ndg.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qdw.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://qlo.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ycd.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://con.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://utv.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vpy.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://sdz.shanyushiyangtech.top

TS:   "7".padStart(3, "0")
来源：http://ows.zhongyouzk.top

Java: String.format("%03d", 7)
来源：http://suo.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ika.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://weo.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sqw.shangyingyoupin.top

[E11] 反转字符串
来源：http://xde.cashguo.top

Py:   s[::-1]
来源：http://lob.zycfv.cn

PHP:  strrev($s);
来源：http://bng.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://szv.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://hsh.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://kkh.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fxr.meibo888.top

Ruby: s.reverse
来源：http://mgm.shzxlz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pvg.hnqzz.top

[E12] 统计某字符出现次数
来源：http://vqj.hnqzz.top

Py:   s.count("a")
来源：http://gru.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://nwp.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://ffu.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://tdh.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uko.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://xbm.sjlbkw.cn

Ruby: s.count("a")
来源：http://vul.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://dcl.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://fki.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://mvr.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bpp.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fen.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ghq.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iaa.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://usz.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eiy.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://glf.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://hyt.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vnt.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wyy.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ith.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gws.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tov.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yvx.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gvu.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://stq.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://ocu.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bkd.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ssl.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yhe.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://juc.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oux.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://glc.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://neo.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dlg.fengsongda.top

[E16] 数字千分位
来源：http://jvz.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://hhv.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://nwf.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xfn.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vif.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sys.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ser.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mvh.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://mqt.zycfv.cn

[E17] 首字母大写
来源：http://agb.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://efu.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbw.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uet.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yiq.fehbvm.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jqy.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ldh.iojbl.cn

Ruby: s.capitalize
来源：http://ojk.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eaw.andypj.xyz

[E18] 模板占位符替换
来源：http://vwr.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cqm.gzhubu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mkv.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vri.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://ltv.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ecz.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vgo.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvm.shanyushiyangtech.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qes.hesvh.cn

[E19] 多行文本按行拆分
来源：http://sdm.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://pap.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://alw.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://anp.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://olt.fktsv.cn

Java: s.lines().toList()
来源：http://ymb.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://gcf.xinyue.icu

Ruby: s.lines
来源：http://puo.ppjwa.cn

C#:   s.Split('\n')
来源：http://aml.fengsongda.top

[E20] 判断字符串是否为空
来源：http://kki.gotoacloud.top

Py:   if not s:
来源：http://olc.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xsf.ehwqpu.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://org.bjfxy.top

TS:   if (s === "") {}
来源：http://xit.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://xpr.yuxming.cn

Go:   if s == "" {}
来源：http://koo.yj202588.top

Ruby: if s.empty?
来源：http://upw.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qlw.zycfv.cn

[E21] 超长截断加省略号
来源：http://flu.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eea.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uxi.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ton.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jeb.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rsb.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://lzs.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://syw.zhaomingkeji.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yts.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://sno.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yzt.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eqs.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xit.yj202588.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dvx.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xdh.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nby.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://dpr.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://svo.52xcode.cn

================================================================================
来源：http://yun.guowangkeji.top

F. 文件与目录
来源：http://awv.cucudq.cn

================================================================================
来源：http://cyy.yj20258888.top

[F01] 读取整个文件
来源：http://tro.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cjs.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://zvo.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tvv.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pwz.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dsa.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dcf.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://nad.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://bej.hcnkem.com

[F02] 逐行读取文件
来源：http://nhz.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xba.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kdu.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ngo.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyj.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kor.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://awo.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ykv.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oyi.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://csz.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xyh.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zwc.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rcq.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qwx.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ezp.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yyb.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://inn.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jur.ydzc1.top

[F04] 追加写入文件
来源：http://srq.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ayk.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://irn.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofy.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqh.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oyu.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eri.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mhr.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hlt.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://bnh.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cdt.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://tgw.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://biv.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://adn.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://thn.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pil.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://cgp.zhixingplan.top


<!-- 参考信息 -->