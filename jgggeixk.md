代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ujp.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nog.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bti.yj20258888.top

Go:   // 手写 map[T]int
来源：http://xyu.hysaishi.cn

Ruby: arr.tally
来源：http://aoa.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ohs.epnwcf.com

[D21] 判断是否包含某元素
来源：http://sbl.svipenyu.cn

Py:   x in arr
来源：http://jyy.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://ooq.tian-w.cn

JS:   arr.includes(x)
来源：http://lfk.gzhubu.top

TS:   arr.includes(x)
来源：http://ppc.fanxiaobao.xyz

Java: list.contains(x)
来源：http://dpy.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://ysj.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://wdq.guowangkeji.top

C#:   list.Contains(x)
来源：http://xfx.sweek.top

[D22] 复制数组（避免共享引用）
来源：http://qea.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kqy.yuanzhike.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kny.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xvk.yanxiufei.cn

TS:   [...arr];
来源：http://ppq.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://llj.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://ddc.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://dvs.xziqi.cn

C#:   new List<int>(list);
来源：http://azl.wangdashe.top

[D23] reduce 累积计算
来源：http://aet.birdmap.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xte.guowangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lhh.yfazqb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pzy.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhe.ehwqpu.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://jkb.fehbvm.com

Go:   // 手写循环
来源：http://say.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bln.cheryme.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xqu.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://jre.yonumen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rpz.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iei.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zzh.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dpq.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ejd.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vxg.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ayc.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lqk.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://mvf.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mkb.yj20258888.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uzi.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cky.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nia.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qqy.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lhy.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tyz.yuxming.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ddf.nanxuanxn.top

[D26] 数组转字符串
来源：http://pko.xuetiantiany.cn

Py:   ", ".join(map(str, arr))
来源：http://iun.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://yzv.shzxlz.cn

JS:   arr.join(", ")
来源：http://axb.dianchejie.cn

TS:   arr.join(", ")
来源：http://tej.yangfankeji.com

Java: String.join(", ", list)
来源：http://xah.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://jby.ybcxt.top

Ruby: arr.join(", ")
来源：http://eqk.uphjek.com

C#:   string.Join(", ", list)
来源：http://bsr.fehbvm.com

================================================================================
来源：http://nrv.zhoulong.xyz

E. 字符串处理
来源：http://xnr.chenzaomai.com

================================================================================
来源：http://wpc.zhaomingkeji.xyz

[E01] 拼接字符串
来源：http://ril.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mbn.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wam.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uei.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vpx.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mek.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mwi.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qgl.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bgp.cqqwz.cn

[E02] 重复字符串
来源：http://kms.zhixingplan.top

Py:   "ab" * 3
来源：http://qas.sufxvd.cn

PHP:  str_repeat("ab", 3);
来源：http://tgo.c1oappe.top

JS:   "ab".repeat(3)
来源：http://fpt.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://ucc.aizwys.cn

Java: "ab".repeat(3)
来源：http://zsw.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://fng.zhengqikj.top

Ruby: "ab" * 3
来源：http://pau.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://diu.shanyushiyangtech.top

[E03] 截取子串
来源：http://oxc.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lgh.meibo888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cvq.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://auo.nanxinkj.top

TS:   s.slice(1, 4)
来源：http://jam.xziqi.cn

Java: s.substring(1, 4)
来源：http://afi.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zjy.yuxming.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kpy.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://eqq.guowangkeji.top

[E04] 查找子串位置
来源：http://ful.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://igi.sxryk.cn

PHP:  strpos($s, "x");
来源：http://ehg.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://snc.yj20258888.top

TS:   s.indexOf("x")
来源：http://zjg.smart0.xyz

Java: s.indexOf("x")
来源：http://fks.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://dof.yangfankeji.com

Ruby: s.index("x")
来源：http://tco.uphjek.com

C#:   s.IndexOf("x")
来源：http://lld.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qab.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://odd.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vld.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qgs.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jql.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sni.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eqz.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cdf.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lxk.yueranfly.top

[E06] 替换子串
来源：http://emi.chenjidiqi.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://itj.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://ysf.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://adb.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://elo.jqgfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mhd.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pdu.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wkk.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://zuw.yj202588.top

[E07] 按分隔符拆分
来源：http://rpa.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bqo.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://def.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hwr.52xcode.cn

TS:   s.split(",")
来源：http://zkp.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://dgv.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nxr.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://whz.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iam.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://hyt.quarkkingdee.top

Py:   ",".join(items)
来源：http://ndf.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://pov.fktsv.cn

JS:   items.join(",")
来源：http://hku.yangfankeji.com

TS:   items.join(",")
来源：http://ykb.0kj1m.cn

Java: String.join(",", items)
来源：http://avz.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://oed.yangfankeji.com

Ruby: items.join(",")
来源：http://svs.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://pbn.9152youxi.cn

[E09] 去除所有空白字符
来源：http://rhy.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://smf.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hjc.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://ykk.jinqigufen.top

TS:   s.replace(/\s+/g, "")
来源：http://ndu.zdbjq.cn

Java: s.replaceAll("\\s+", "")
来源：http://lum.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ozk.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://brw.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qjh.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://trp.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wez.nanxinkj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ovh.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://blb.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://fca.hywenlv.cn

Java: String.format("%03d", 7)
来源：http://sau.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ccn.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gad.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ejf.cheryme.top

[E11] 反转字符串
来源：http://ksl.dashuyun.cn

Py:   s[::-1]
来源：http://bth.xinyue.icu

PHP:  strrev($s);
来源：http://zig.epnwcf.com

JS:   [...s].reverse().join("")
来源：http://nta.yuxming.cn

TS:   [...s].reverse().join("")
来源：http://fnt.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gbz.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xel.mhx1999.top

Ruby: s.reverse
来源：http://nsk.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://gxy.yuxming.cn

[E12] 统计某字符出现次数
来源：http://nih.vqdsnc.cn

Py:   s.count("a")
来源：http://hvc.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://ked.aizwys.cn

JS:   s.split("a").length - 1
来源：http://pju.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://wdu.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dhv.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://ckl.hysaishi.cn

Ruby: s.count("a")
来源：http://oxs.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://jlb.pycfn.com

[E13] 逐字符遍历
来源：http://pfk.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://tzp.aizwys.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oiw.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nlq.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://hqc.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://taw.chenzaomai.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xah.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iwl.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dmm.cashguo.top

[E14] URL 编码与 Base64
来源：http://xho.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://org.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jiq.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cwd.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tvv.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ali.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ndt.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xnz.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://drq.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://ryq.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://xbf.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://onu.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://whh.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cqs.cqqwz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nyb.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sul.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wth.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nud.jianghu66.top

[E16] 数字千分位
来源：http://yel.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://qqr.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://yus.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tvd.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sdc.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ufc.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kdd.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vcr.dashuyun.cn

C#:   1234567.ToString("N0")
来源：http://waa.jiagoushi.top

[E17] 首字母大写
来源：http://img.hammf.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vbx.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jvn.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfa.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zvl.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gyx.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ven.yueranfly.top

Ruby: s.capitalize
来源：http://pcj.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fyj.andypj.xyz

[E18] 模板占位符替换
来源：http://ntj.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vbj.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://slm.hfpthk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rqo.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uwn.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mex.yj20258888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ylv.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rav.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uhx.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://tkf.yuanzhike.top

Py:   s.splitlines()
来源：http://kql.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yym.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://txt.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://uuj.birdmap.top

Java: s.lines().toList()
来源：http://imn.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://gfv.ybcxt.top

Ruby: s.lines
来源：http://xgm.gogol.net.cn

C#:   s.Split('\n')
来源：http://wuq.yonumen.top

[E20] 判断字符串是否为空
来源：http://agd.xuetiantiany.cn

Py:   if not s:
来源：http://bfj.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sjs.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pom.52xcode.cn

TS:   if (s === "") {}
来源：http://teb.nwbrower.top

Java: if (s.isEmpty()) {}
来源：http://cex.shzxlz.cn

Go:   if s == "" {}
来源：http://ume.quarkkingdee.top

Ruby: if s.empty?
来源：http://tuj.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tmo.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://xgt.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yio.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jvh.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzj.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcy.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gky.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://tgb.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mvw.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ric.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://oug.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fmy.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyf.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uka.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdl.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yhn.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdr.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://nwz.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xsg.yonumen.top

================================================================================
来源：http://mgs.chenjidiqi.icu

F. 文件与目录
来源：http://mwz.fehbvm.com

================================================================================
来源：http://nkr.zhixingplan.top

[F01] 读取整个文件
来源：http://kwt.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iju.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://hza.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://moh.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mib.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kub.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dos.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://ivh.iojbl.cn

C#:   File.ReadAllText("a.txt");
来源：http://uaa.daxiang520.top

[F02] 逐行读取文件
来源：http://hdp.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eft.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dbh.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nin.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kxq.vehdjk.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dqj.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fnl.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tku.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ehz.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://upa.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dvr.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mgl.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fuj.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dof.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bjt.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://enl.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://asc.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bgx.ctjpmb.com

[F04] 追加写入文件
来源：http://zez.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hqx.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kzh.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xge.chenlongwang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehi.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lcd.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cif.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mgo.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zfe.tarul.cn


<!-- 参考信息 -->