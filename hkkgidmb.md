代发 wailian999

Java: new ArrayList<>(list);
来源：http://tlk.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://iwd.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://nah.nanxinkj.top

C#:   new List<int>(list);
来源：http://zle.hnxiangtu.top

[D23] reduce 累积计算
来源：http://usm.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mxr.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://emq.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bms.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lez.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rqx.ybcxt.top

Go:   // 手写循环
来源：http://lwr.zhiwuduotai.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qeg.ehwqpu.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sba.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://jcm.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lml.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tlv.guowangkeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://asp.dianchejie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gfp.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://clu.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ptt.birdmap.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xwg.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cws.guannengcc.top

[D25] Set 集合去重与交并差
来源：http://hbt.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mqi.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nfi.hammf.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ljk.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jow.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ehk.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://flr.ppjwa.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jqm.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rvu.jiagoushi.top

[D26] 数组转字符串
来源：http://oid.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://dca.316326.xyz

PHP:  implode(", ", $arr);
来源：http://vgi.daria6918.cn

JS:   arr.join(", ")
来源：http://cue.bjfxy.top

TS:   arr.join(", ")
来源：http://qtv.aizwys.cn

Java: String.join(", ", list)
来源：http://ism.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://eng.andypj.xyz

Ruby: arr.join(", ")
来源：http://ild.gzhubu.top

C#:   string.Join(", ", list)
来源：http://jun.zdbjq.cn

================================================================================
来源：http://qmb.shanyushiyangkeji.top

E. 字符串处理
来源：http://olo.iojbl.cn

================================================================================
来源：http://wyp.meibo888.top

[E01] 拼接字符串
来源：http://axy.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xdi.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wjm.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://chu.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://idy.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ejp.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://veh.yonumen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://usc.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zqt.andypj.xyz

[E02] 重复字符串
来源：http://btt.meibo888.top

Py:   "ab" * 3
来源：http://oyl.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://mrq.tarul.cn

JS:   "ab".repeat(3)
来源：http://urw.tian-w.cn

TS:   "ab".repeat(3)
来源：http://rqk.jyoumei.cn

Java: "ab".repeat(3)
来源：http://qih.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://yrx.hnqzz.top

Ruby: "ab" * 3
来源：http://akz.jinqigufen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rno.hywenlv.cn

[E03] 截取子串
来源：http://avx.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://apd.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vdb.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bsw.shzxlz.cn

TS:   s.slice(1, 4)
来源：http://nie.xinyue.icu

Java: s.substring(1, 4)
来源：http://uwp.316326.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zgs.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://bah.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://fgk.yvedp.cn

[E04] 查找子串位置
来源：http://nov.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://taj.ydzc1.top

PHP:  strpos($s, "x");
来源：http://axm.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ywx.nwbrower.top

TS:   s.indexOf("x")
来源：http://qub.jqgfzy.top

Java: s.indexOf("x")
来源：http://uvq.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://osg.chenjidiqi.icu

Ruby: s.index("x")
来源：http://qsx.yfazqb.com

C#:   s.IndexOf("x")
来源：http://unv.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pxp.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pmi.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aoo.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cqn.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyj.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cxc.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zgs.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jca.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ifh.zhaomingkeji.xyz

[E06] 替换子串
来源：http://zds.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uwr.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://gzc.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxd.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://rdr.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dke.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oza.52xcode.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dqy.cheryme.top

C#:   s.Replace("a", "b")
来源：http://usr.shzxlz.cn

[E07] 按分隔符拆分
来源：http://ykx.shangyingyoupin.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rlr.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aoj.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qvk.shanyushiyangtech.top

TS:   s.split(",")
来源：http://cvi.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://rfs.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dbe.tian-w.cn

Ruby: s.split(",");  s.split
来源：http://siv.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iae.xziqi.cn

[E08] 数组按分隔符合并
来源：http://tqa.nwbrower.top

Py:   ",".join(items)
来源：http://wnh.ppjwa.cn

PHP:  implode(",", $items);
来源：http://dcf.gogol.net.cn

JS:   items.join(",")
来源：http://cuy.chenzaomai.com

TS:   items.join(",")
来源：http://kva.nanxinkj.top

Java: String.join(",", items)
来源：http://uit.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://xnp.sjlbkw.cn

Ruby: items.join(",")
来源：http://mli.ctjpmb.com

C#:   string.Join(",", items)
来源：http://xew.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://qey.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nju.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://otc.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://qhr.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://hug.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://uiz.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://lki.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jci.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hzc.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://wep.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ffj.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uxb.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://bgw.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://pkr.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://sya.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ylv.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dca.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ukp.xylfe.cn

[E11] 反转字符串
来源：http://xxf.ppjwa.cn

Py:   s[::-1]
来源：http://spr.meibo888.top

PHP:  strrev($s);
来源：http://oul.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://xhi.tarul.cn

TS:   [...s].reverse().join("")
来源：http://sbt.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tmu.cashguo.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sjr.svipenyu.cn

Ruby: s.reverse
来源：http://vew.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://yns.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://vsw.kuanghao11.cn

Py:   s.count("a")
来源：http://dlm.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://xks.meibo888.top

JS:   s.split("a").length - 1
来源：http://owv.sxryk.cn

TS:   s.split("a").length - 1
来源：http://bhr.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qtx.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://adt.ppjwa.cn

Ruby: s.count("a")
来源：http://psv.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://gil.redwolf501.top

[E13] 逐字符遍历
来源：http://iec.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://fie.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tyc.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vfb.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nkc.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jgl.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nsv.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tuh.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bkr.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://rkf.smart0.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sia.gaohongyu789.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://iih.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pyt.nwbrower.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jdw.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xpr.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wrp.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://idk.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nuy.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://qff.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://agj.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vxx.uphjek.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fcr.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://enl.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wcz.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bef.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cnl.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fhs.jyoumei.cn

[E16] 数字千分位
来源：http://are.chenzaomai.com

Py:   f"{1234567:,}"
来源：http://lyv.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://ues.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xzc.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://let.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sqc.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eqa.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eqg.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://snd.0kj1m.cn

[E17] 首字母大写
来源：http://yfe.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://slb.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rkq.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cle.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://spz.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sci.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rlj.xziqi.cn

Ruby: s.capitalize
来源：http://qqs.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xkr.dashuyun.cn

[E18] 模板占位符替换
来源：http://mbs.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pal.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://arz.uphjek.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bgq.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vto.svipenyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://smj.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mkm.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rgy.fehbvm.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ywi.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://xrx.hongshengwenyu.top

Py:   s.splitlines()
来源：http://zyj.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wlj.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://vkd.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://ycj.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://tlv.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://nqi.shzxlz.cn

Ruby: s.lines
来源：http://hqv.tianlin.xyz

C#:   s.Split('\n')
来源：http://gho.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://hdj.smart0.xyz

Py:   if not s:
来源：http://xqr.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yvk.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://otg.hcnkem.com

TS:   if (s === "") {}
来源：http://sof.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://gxj.zhiwuduotai.top

Go:   if s == "" {}
来源：http://sbu.meibo888.top

Ruby: if s.empty?
来源：http://onl.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://czb.ybcxt.top

[E21] 超长截断加省略号
来源：http://koe.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dqc.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uua.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uxp.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bdb.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xao.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://jku.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hbr.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kjo.hesvh.cn

[E22] 字节长度与字符长度
来源：http://gcn.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tvk.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rwl.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mxo.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtc.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kqg.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ksy.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://obz.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ekk.havefunace.top

================================================================================
来源：http://xyv.wangdashe.top

F. 文件与目录
来源：http://jti.daxiang520.top

================================================================================
来源：http://wyi.vqdsnc.cn

[F01] 读取整个文件
来源：http://day.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ggx.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://szf.jqgufenzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ajc.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ebn.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tkp.shuidangran.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://woe.jlsjyb.cn

Ruby: File.read("a.txt")
来源：http://zer.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://whm.chenlongwang.top

[F02] 逐行读取文件
来源：http://pdh.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wht.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lsc.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://con.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://teg.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gja.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://onn.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wui.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ffp.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://qip.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxn.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hob.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://whl.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pwy.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wir.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wmv.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://hzn.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gjl.zhongyouzk.top

[F04] 追加写入文件
来源：http://zif.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://deq.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ggf.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bdn.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pgz.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://inn.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ela.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dyt.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mjh.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://tuy.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xbf.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://yni.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://stw.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://iqh.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oif.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bgt.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://cau.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://ock.gzhubu.top

[F06] 删除文件
来源：http://lza.sweek.top

Py:   os.remove("a.txt")
来源：http://pxh.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://wnd.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://aab.sjlbkw.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tgj.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rpl.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://afy.yongpay.top

Ruby: File.delete("a.txt")
来源：http://xge.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://zop.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://lvw.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gnq.ppjwa.cn


<!-- 参考信息 -->