代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://xtr.vehdjk.com

JS:   arr.includes(x)
来源：http://nwd.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://vpr.snrcjt.cn

Java: list.contains(x)
来源：http://vfl.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://nzn.ywan-chungtsiang.top

Ruby: arr.include?(x)
来源：http://dct.shzxlz.cn

C#:   list.Contains(x)
来源：http://rwc.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://ivl.ehwqpu.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tam.aibaodan.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hvp.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xrf.0kj1m.cn

TS:   [...arr];
来源：http://cuo.zhoulong.xyz

Java: new ArrayList<>(list);
来源：http://ctw.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sbd.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://ill.fzhhl.top

C#:   new List<int>(list);
来源：http://scs.sxryk.cn

[D23] reduce 累积计算
来源：http://gah.vqdsnc.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://akx.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://odl.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ojs.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uuf.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wav.nanxuanxn.top

Go:   // 手写循环
来源：http://aet.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cxv.birdmap.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qlf.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://ddg.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jkh.zhengqikj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oue.iojbl.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bbp.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wou.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baa.shanyushiyangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jsv.shanyushiyangtech.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tov.quarkkingdee.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://quw.zycfv.cn

[D25] Set 集合去重与交并差
来源：http://slk.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yuh.ydjk.org.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gmw.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iew.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qpt.fengsongda.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whr.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tda.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oiu.0kj1m.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hoz.316326.xyz

[D26] 数组转字符串
来源：http://nse.shangyingyoupin.top

Py:   ", ".join(map(str, arr))
来源：http://nkl.hcnkem.com

PHP:  implode(", ", $arr);
来源：http://rim.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://wjy.zhongyouzk.top

TS:   arr.join(", ")
来源：http://fwz.daxiang520.top

Java: String.join(", ", list)
来源：http://tnu.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://drl.hywenlv.cn

Ruby: arr.join(", ")
来源：http://jbg.hcnkem.com

C#:   string.Join(", ", list)
来源：http://emd.hysaishi.cn

================================================================================
来源：http://xar.zhijiandao.cn

E. 字符串处理
来源：http://hks.jqgfzy.top

================================================================================
来源：http://yvv.cucudq.cn

[E01] 拼接字符串
来源：http://rxk.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gjn.xuetiantiany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mkq.ppjwa.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kgi.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ryj.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://drp.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xki.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lea.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ulb.aibaodan.cn

[E02] 重复字符串
来源：http://cez.tanke756.top

Py:   "ab" * 3
来源：http://hto.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://jxd.zycfv.cn

JS:   "ab".repeat(3)
来源：http://vjq.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://fmh.birdmap.top

Java: "ab".repeat(3)
来源：http://ntw.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://niz.jyoumei.cn

Ruby: "ab" * 3
来源：http://eyo.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://njx.cashguo.top

[E03] 截取子串
来源：http://bqp.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uao.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uvq.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rlq.redwolf501.top

TS:   s.slice(1, 4)
来源：http://iir.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://viw.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fxn.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://czk.zhijiandao.cn

C#:   s.Substring(1, 3)
来源：http://zhh.jqgfzy.top

[E04] 查找子串位置
来源：http://nnx.gogol.net.cn

Py:   s.find("x");  s.index("x")
来源：http://par.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://akt.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yco.yangfankeji.com

TS:   s.indexOf("x")
来源：http://ztj.ydzc1.top

Java: s.indexOf("x")
来源：http://bmi.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://ogj.fehbvm.com

Ruby: s.index("x")
来源：http://mzp.uphjek.com

C#:   s.IndexOf("x")
来源：http://qvh.pengpengdd.cyou

[E05] 判断包含 / 前缀 / 后缀
来源：http://jus.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gfy.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://juy.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gab.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eyd.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xhe.jyoumei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mky.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qyy.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wwa.xuanzx.com

[E06] 替换子串
来源：http://oho.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://epb.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://quu.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ubj.hcnkem.com

TS:   s.replaceAll("a", "b")
来源：http://mtq.cashguo.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ule.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mxc.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xig.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://onm.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://crc.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pgu.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pqm.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kbk.zhongyouzk.top

TS:   s.split(",")
来源：http://fme.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://rka.quarkkingdee.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://irf.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://lma.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lvb.jianghu66.top

[E08] 数组按分隔符合并
来源：http://kyf.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://fnw.svipenyu.cn

PHP:  implode(",", $items);
来源：http://iyt.yvedp.cn

JS:   items.join(",")
来源：http://ojo.yonumen.top

TS:   items.join(",")
来源：http://zfa.zhiwuduotai.top

Java: String.join(",", items)
来源：http://uyv.uphjek.com

Go:   strings.Join(items, ",")
来源：http://dod.haohaochexian.top

Ruby: items.join(",")
来源：http://gsw.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://sgy.cucudq.cn

[E09] 去除所有空白字符
来源：http://sti.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mbw.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vhs.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://iir.cqqwz.cn

TS:   s.replace(/\s+/g, "")
来源：http://jdh.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://med.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sjc.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fgc.ppjwa.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sql.pengpengdd.cyou

[E10] 左侧补零 / 定长填充
来源：http://ohg.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qfr.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://exk.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://yuu.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://vfo.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://xhx.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mvy.sjlbkw.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://djy.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hjh.yj20258.top

[E11] 反转字符串
来源：http://ivr.c1oappe.top

Py:   s[::-1]
来源：http://dmj.yvedp.cn

PHP:  strrev($s);
来源：http://oga.tarul.cn

JS:   [...s].reverse().join("")
来源：http://ixr.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://pvb.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://prj.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gdc.haohaochexian.top

Ruby: s.reverse
来源：http://yha.hysaishi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gnt.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://xxd.ydjk.org.cn

Py:   s.count("a")
来源：http://qgg.yangfankeji.com

PHP:  substr_count($s, "a");
来源：http://nlv.316326.xyz

JS:   s.split("a").length - 1
来源：http://iyi.wangdashe.top

TS:   s.split("a").length - 1
来源：http://ziz.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://enm.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://cbr.havefunace.top

Ruby: s.count("a")
来源：http://yvi.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://vcd.zdbjq.cn

[E13] 逐字符遍历
来源：http://bja.meibo888.top

Py:   for ch in s: print(ch)
来源：http://hxy.ywan-chungtsiang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dkc.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://obf.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://eux.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dzc.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hmc.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cqp.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zqw.xingfuxueyuan.xyz

[E14] URL 编码与 Base64
来源：http://chi.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://swz.aibaodan.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zbq.shangyingyoupin.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://anm.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uno.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ike.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wgw.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://omf.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aqe.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://ibf.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mio.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://feq.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ctb.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ffp.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vqs.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://frs.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jwu.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eyw.gzhubu.top

[E16] 数字千分位
来源：http://cfs.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://gql.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://mfa.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cvh.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lfb.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zok.jinqigfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gee.zhixingplan.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qok.tarul.cn

C#:   1234567.ToString("N0")
来源：http://xfu.yueranfly.top

[E17] 首字母大写
来源：http://wkx.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hud.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ogg.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ung.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://irw.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ssr.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yfv.tianlin.xyz

Ruby: s.capitalize
来源：http://ymd.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ecm.ydzc1.top

[E18] 模板占位符替换
来源：http://ayw.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vdm.birdmap.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mgq.tian-w.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mvb.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gyj.redwolf501.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pvl.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kvn.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wto.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nac.shanyushiyangkeji.top

[E19] 多行文本按行拆分
来源：http://cxq.cheryme.top

Py:   s.splitlines()
来源：http://qpl.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bkf.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://mct.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://gel.yanxiufei.cn

Java: s.lines().toList()
来源：http://dbn.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://wzl.yangfankeji.com

Ruby: s.lines
来源：http://wel.daria6918.cn

C#:   s.Split('\n')
来源：http://irl.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://yra.svipenyu.cn

Py:   if not s:
来源：http://hfw.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://luz.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gcj.hnxiangtu.top

TS:   if (s === "") {}
来源：http://jyk.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://fjb.bbcook.cn

Go:   if s == "" {}
来源：http://rwe.tianlin.xyz

Ruby: if s.empty?
来源：http://weu.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://occ.nwbrower.top

[E21] 超长截断加省略号
来源：http://gho.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rua.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hwx.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uuq.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gpo.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dba.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://oct.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dha.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jeo.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://rfi.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tzr.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tkc.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://odw.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://idi.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lsb.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oxj.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://hft.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ddz.gaohongyu789.top

================================================================================
来源：http://edi.shzxlz.cn

F. 文件与目录
来源：http://lwd.hnqzz.top

================================================================================
来源：http://err.yj202588.top

[F01] 读取整个文件
来源：http://thm.yanxiufei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gzd.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://ofd.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rxd.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://etp.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qwe.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jdo.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://fqt.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://zuc.hesvh.cn

[F02] 逐行读取文件
来源：http://tyu.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nkl.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qsz.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aip.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hkq.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ukc.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dxa.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gpj.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://veb.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://rsw.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mql.hcnkem.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://pkt.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yok.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qsa.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zhi.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yhd.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://pid.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ocm.feifeiyinyue.top

[F04] 追加写入文件
来源：http://eua.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kcp.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mhh.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jmc.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://psi.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jsf.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ogt.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hsp.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lvz.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://ppl.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wsk.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://wyf.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://pbj.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://cwi.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dur.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nkq.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://dem.daxiang520.top


<!-- 参考信息 -->