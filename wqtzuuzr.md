代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pkj.hongshengwenyu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ant.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hmx.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://wau.hcnkem.com

Ruby: arr.tally
来源：http://vzr.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://scf.hfpthk.cn

[D21] 判断是否包含某元素
来源：http://een.hysaishi.cn

Py:   x in arr
来源：http://oyo.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://fyw.haohaochexian.top

JS:   arr.includes(x)
来源：http://nkj.shuidangran.top

TS:   arr.includes(x)
来源：http://dvj.yj20258.top

Java: list.contains(x)
来源：http://riy.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://vbn.chenjidiqi.icu

Ruby: arr.include?(x)
来源：http://qhv.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://grl.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://xzr.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tdr.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ekm.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iaa.pycfn.com

TS:   [...arr];
来源：http://gdr.daxiang520.top

Java: new ArrayList<>(list);
来源：http://lin.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cnb.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://uve.sysykeji.top

C#:   new List<int>(list);
来源：http://ldr.aibaodan.cn

[D23] reduce 累积计算
来源：http://aer.cucudq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://muz.yj20258.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zkz.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wla.zycfv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fnm.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ykr.gaohongyu789.top

Go:   // 手写循环
来源：http://ffu.hfpthk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uau.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://avz.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://byk.shangyingyoupin.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://knv.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lnk.bbcook.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gqw.gogol.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://roj.nanxinkj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://daa.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zho.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ihj.tianlin.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lwq.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://wqy.haohaochexian.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sre.cheryme.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://azp.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gtw.9152youxi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ijz.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uqe.quarkkingdee.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://osp.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vtu.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xgk.tarul.cn

[D26] 数组转字符串
来源：http://qku.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://wjv.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://kpr.cucudq.cn

JS:   arr.join(", ")
来源：http://jiw.cucudq.cn

TS:   arr.join(", ")
来源：http://qfh.zhongyouzk.top

Java: String.join(", ", list)
来源：http://fxd.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://xoo.tian-w.cn

Ruby: arr.join(", ")
来源：http://dqz.tanke756.top

C#:   string.Join(", ", list)
来源：http://jdi.cqqwz.cn

================================================================================
来源：http://tri.ehwqpu.com

E. 字符串处理
来源：http://umr.tarul.cn

================================================================================
来源：http://xcb.jyoumei.cn

[E01] 拼接字符串
来源：http://rja.bbcook.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://omi.yuxming.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nec.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fbu.zhijiandao.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nnf.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://efk.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qfx.tarul.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lqz.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ukh.birdmap.top

[E02] 重复字符串
来源：http://ewr.ybcxt.top

Py:   "ab" * 3
来源：http://jbi.fengsongda.top

PHP:  str_repeat("ab", 3);
来源：http://rnw.birdmap.top

JS:   "ab".repeat(3)
来源：http://jlx.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://rer.zhengqikj.top

Java: "ab".repeat(3)
来源：http://zat.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://idp.yj20258.top

Ruby: "ab" * 3
来源：http://rnp.ydzc1.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lhl.sysykeji.top

[E03] 截取子串
来源：http://kwi.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fjy.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uqe.9152youxi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ghp.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://axb.bbcook.cn

Java: s.substring(1, 4)
来源：http://xqo.smart0.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jlo.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://omn.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://ziw.tianlin.xyz

[E04] 查找子串位置
来源：http://qrg.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://wdt.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://jib.andypj.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ykq.pycfn.com

TS:   s.indexOf("x")
来源：http://bcp.yfazqb.com

Java: s.indexOf("x")
来源：http://exy.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://ygn.bbcook.cn

Ruby: s.index("x")
来源：http://zzs.yuxming.cn

C#:   s.IndexOf("x")
来源：http://urk.pycfn.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://uio.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://udz.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rly.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vcy.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://jve.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://csx.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cvm.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://emj.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vzv.aibaodan.cn

[E06] 替换子串
来源：http://ujq.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kye.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://vhm.jqgfzy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rfg.haohaochexian.top

TS:   s.replaceAll("a", "b")
来源：http://ust.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kpr.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ghz.svipenyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lht.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://uou.snrcjt.cn

[E07] 按分隔符拆分
来源：http://uqz.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://slj.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nsv.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gwz.cqqwz.cn

TS:   s.split(",")
来源：http://bcn.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ngq.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gdo.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://snw.yanxiufei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qev.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://cqu.zycfv.cn

Py:   ",".join(items)
来源：http://lfj.zdqjudy.top

PHP:  implode(",", $items);
来源：http://ujt.ehwqpu.com

JS:   items.join(",")
来源：http://fce.yonumen.top

TS:   items.join(",")
来源：http://uub.fzhhl.top

Java: String.join(",", items)
来源：http://hpq.316326.xyz

Go:   strings.Join(items, ",")
来源：http://akk.zycfv.cn

Ruby: items.join(",")
来源：http://ipj.cucudq.cn

C#:   string.Join(",", items)
来源：http://yjg.bbcook.cn

[E09] 去除所有空白字符
来源：http://llj.ctjpmb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rfk.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ijz.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://zce.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://jhv.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://yua.hcnkem.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://vyx.cashguo.top

Ruby: s.gsub(/\s+/, "")
来源：http://dot.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fdw.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://lql.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pmn.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xzd.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://kyn.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://zio.xziqi.cn

Java: String.format("%03d", 7)
来源：http://ksc.ydzc1.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pzj.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://llb.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sbz.guowangkeji.top

[E11] 反转字符串
来源：http://xid.yfazqb.com

Py:   s[::-1]
来源：http://ztf.jlsjyb.cn

PHP:  strrev($s);
来源：http://ciz.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://sia.guowangkeji.top

TS:   [...s].reverse().join("")
来源：http://jvu.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fcc.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xuj.jqgfzy.top

Ruby: s.reverse
来源：http://yka.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tps.daxiang520.top

[E12] 统计某字符出现次数
来源：http://zid.yanxiufei.cn

Py:   s.count("a")
来源：http://dxk.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://lvm.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://nux.316326.xyz

TS:   s.split("a").length - 1
来源：http://giw.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eoc.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://fyf.daria6918.cn

Ruby: s.count("a")
来源：http://rfu.vqdsnc.cn

C#:   s.Count(c => c == 'a')
来源：http://ifi.vqdsnc.cn

[E13] 逐字符遍历
来源：http://vsk.meibo888.top

Py:   for ch in s: print(ch)
来源：http://ytg.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://noa.jqgufenzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jvz.0kj1m.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tip.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://szt.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pye.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qvm.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zlz.shuidangran.top

[E14] URL 编码与 Base64
来源：http://yws.316326.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ysc.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://owl.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://axh.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://odt.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://orr.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xti.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rku.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://spk.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://iiy.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://exf.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fve.hnqzz.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ljo.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jwb.vqdsnc.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sri.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rys.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://utr.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eol.daria6918.cn

[E16] 数字千分位
来源：http://fuz.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://mtj.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://wns.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dli.haohaochexian.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hsf.zhongyouzk.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eab.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xfi.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dms.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://zsr.hcnkem.com

[E17] 首字母大写
来源：http://jzd.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://utp.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cic.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hby.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qaz.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ysg.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jvx.pengpengdd.cyou

Ruby: s.capitalize
来源：http://piw.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ppu.cdnleiting.top

[E18] 模板占位符替换
来源：http://qqg.nanxuanxn.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://muo.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bhh.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ecj.sxryk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nkn.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gkh.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mxe.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://krs.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aue.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://xnc.xziqi.cn

Py:   s.splitlines()
来源：http://lsn.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lxn.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://gst.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://bff.fktsv.cn

Java: s.lines().toList()
来源：http://xdx.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://bst.xylfe.cn

Ruby: s.lines
来源：http://rsk.shzxlz.cn

C#:   s.Split('\n')
来源：http://gqw.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://xud.yuxming.cn

Py:   if not s:
来源：http://tjn.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cfd.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qqa.epnwcf.com

TS:   if (s === "") {}
来源：http://omg.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://qos.ivvv.top

Go:   if s == "" {}
来源：http://jpc.tianlin.xyz

Ruby: if s.empty?
来源：http://ser.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vxc.pycfn.com

[E21] 超长截断加省略号
来源：http://gfi.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://atk.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dza.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tig.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzl.cheryme.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fvh.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://sfr.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nib.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://npp.havefunace.top

[E22] 字节长度与字符长度
来源：http://tte.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zmm.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qac.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kbg.xuanzx.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dsp.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mde.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ylz.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://vxj.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vom.nwbrower.top

================================================================================
来源：http://vpm.xylfe.cn

F. 文件与目录
来源：http://ras.fehbvm.com

================================================================================
来源：http://aqf.vehdjk.com

[F01] 读取整个文件
来源：http://srm.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dzd.chenlongwang.top

PHP:  file_get_contents("a.txt");
来源：http://xef.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wtt.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zzs.gotoacloud.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bhd.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yon.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://xym.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://blq.hfpthk.cn

[F02] 逐行读取文件
来源：http://isy.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rxr.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://txp.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yqu.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wtw.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhn.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://upk.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qby.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pkr.havefunace.top

[F03] 写入文件（覆盖）
来源：http://qex.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://web.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://aoc.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iky.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yid.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://alw.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wlk.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://cjf.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lvf.xylfe.cn

[F04] 追加写入文件
来源：http://fqs.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rzb.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dpy.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yvl.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://stu.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zpl.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fzp.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mgr.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xlz.tian-w.cn


<!-- 参考信息 -->