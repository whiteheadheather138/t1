代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dvz.cashguo.top

[D20] 统计每个元素出现次数
来源：http://fdj.sufxvd.cn

Py:   Counter(arr)
来源：http://uxo.zdqjudy.top

PHP:  array_count_values($arr);
来源：http://ayz.sufxvd.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggq.shzxlz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzy.cqqwz.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zml.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://iah.zhengqikj.top

Ruby: arr.tally
来源：http://rmk.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://szp.feifeiyinyue.top

[D21] 判断是否包含某元素
来源：http://lxz.jqgfzy.top

Py:   x in arr
来源：http://nds.nanxuanxn.top

PHP:  in_array($x, $arr, true);
来源：http://zok.bjfxy.top

JS:   arr.includes(x)
来源：http://wjr.epnwcf.com

TS:   arr.includes(x)
来源：http://acy.sjlbkw.cn

Java: list.contains(x)
来源：http://hjo.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://all.birdmap.top

Ruby: arr.include?(x)
来源：http://sdt.smart0.xyz

C#:   list.Contains(x)
来源：http://pqq.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://urm.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ntz.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://urx.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uid.vqdsnc.cn

TS:   [...arr];
来源：http://ycu.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://bgb.yvedp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rno.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://chd.nwbrower.top

C#:   new List<int>(list);
来源：http://yip.zdqjudy.top

[D23] reduce 累积计算
来源：http://hfy.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xwk.chenjidiqi.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sxn.shzxlz.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cfm.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysc.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ure.xylfe.cn

Go:   // 手写循环
来源：http://shh.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ios.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hbu.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://nfy.cashguo.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jub.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ehe.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pds.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://riy.zhiwuduotai.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://evq.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://efi.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pyl.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sma.aizwys.cn

[D25] Set 集合去重与交并差
来源：http://gjo.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ksc.ydzc1.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wjl.hongshengwenyu.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ygi.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kyi.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tyi.jianghu66.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mps.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aar.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://viz.jyoumei.cn

[D26] 数组转字符串
来源：http://iad.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://zyn.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://wib.bjfxy.top

JS:   arr.join(", ")
来源：http://ivb.ydjk.org.cn

TS:   arr.join(", ")
来源：http://cwn.ppjwa.cn

Java: String.join(", ", list)
来源：http://lbn.ywan-chungtsiang.top

Go:   strings.Join(strs, ", ")
来源：http://pai.zdbjq.cn

Ruby: arr.join(", ")
来源：http://dwe.shuidangran.top

C#:   string.Join(", ", list)
来源：http://xiy.gotoacloud.top

================================================================================
来源：http://ybl.ivvv.top

E. 字符串处理
来源：http://sju.aizwys.cn

================================================================================
来源：http://bfk.andypj.xyz

[E01] 拼接字符串
来源：http://iak.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wva.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jef.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ntt.52xcode.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyo.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xzs.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://whx.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xyz.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pce.tarul.cn

[E02] 重复字符串
来源：http://wti.52xcode.cn

Py:   "ab" * 3
来源：http://fnu.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://dze.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://hca.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://gom.hysaishi.cn

Java: "ab".repeat(3)
来源：http://xud.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://rqq.zhoulong.xyz

Ruby: "ab" * 3
来源：http://dcc.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ugk.bbcook.cn

[E03] 截取子串
来源：http://clb.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rom.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://srp.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zqy.zycfv.cn

TS:   s.slice(1, 4)
来源：http://hba.ydzc1.top

Java: s.substring(1, 4)
来源：http://qag.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://glg.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://ylr.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://rpb.ehwqpu.com

[E04] 查找子串位置
来源：http://pyg.yangfankeji.com

Py:   s.find("x");  s.index("x")
来源：http://mmc.yueranfly.top

PHP:  strpos($s, "x");
来源：http://xha.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zzu.fengsongda.top

TS:   s.indexOf("x")
来源：http://unq.tanke756.top

Java: s.indexOf("x")
来源：http://yvr.ctjpmb.com

Go:   strings.Index(s, "x")
来源：http://fcq.bjfxy.top

Ruby: s.index("x")
来源：http://lqx.yfazqb.com

C#:   s.IndexOf("x")
来源：http://zbo.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lgt.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wwb.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gvu.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsq.ehwqpu.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fdj.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dfa.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hhb.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tdb.fengsongda.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yaz.yangfankeji.com

[E06] 替换子串
来源：http://kwl.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ueq.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://xer.nanxuanxn.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cad.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://pfc.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sfz.jinqigfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nra.jinghuilouyu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cyg.andypj.xyz

C#:   s.Replace("a", "b")
来源：http://bqr.guannengcc.top

[E07] 按分隔符拆分
来源：http://igv.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fwe.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vph.nwbrower.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://faa.sufxvd.cn

TS:   s.split(",")
来源：http://nzj.zhijiandao.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xxd.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dtp.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://qjk.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gzm.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://rqj.vqdsnc.cn

Py:   ",".join(items)
来源：http://cnn.hfpthk.cn

PHP:  implode(",", $items);
来源：http://xsn.yangfankeji.com

JS:   items.join(",")
来源：http://mgu.daria6918.cn

TS:   items.join(",")
来源：http://smt.nwbrower.top

Java: String.join(",", items)
来源：http://hms.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://rrc.fehbvm.com

Ruby: items.join(",")
来源：http://tjl.cheryme.top

C#:   string.Join(",", items)
来源：http://bai.mhx1999.top

[E09] 去除所有空白字符
来源：http://ysb.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hbj.zhongyouzk.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://chz.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://bcw.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://jka.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://jrc.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dyx.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://xmd.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://eay.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://ujo.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ovb.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jqy.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://uev.tanke756.top

TS:   "7".padStart(3, "0")
来源：http://mln.fengsongda.top

Java: String.format("%03d", 7)
来源：http://jui.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://icx.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ejt.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gtg.uphjek.com

[E11] 反转字符串
来源：http://stz.svipenyu.cn

Py:   s[::-1]
来源：http://mwe.vehdjk.com

PHP:  strrev($s);
来源：http://hko.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://wqz.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://swb.hcnkem.com

Java: new StringBuilder(s).reverse().toString()
来源：http://liy.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zlm.shzxlz.cn

Ruby: s.reverse
来源：http://oqg.pengpengdd.cyou

C#:   new string(s.Reverse().ToArray())
来源：http://jif.jianghu66.top

[E12] 统计某字符出现次数
来源：http://nid.jqgufenzy.top

Py:   s.count("a")
来源：http://hzp.sweek.top

PHP:  substr_count($s, "a");
来源：http://dcx.birdmap.top

JS:   s.split("a").length - 1
来源：http://qwk.vqdsnc.cn

TS:   s.split("a").length - 1
来源：http://xld.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bkn.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://nkx.yj202588.top

Ruby: s.count("a")
来源：http://qcc.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://nrr.quarkkingdee.top

[E13] 逐字符遍历
来源：http://drm.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://gqw.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rca.wangdashe.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://heg.fktsv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://drh.yj20258888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bil.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nfx.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uss.gzhubu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jcn.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://tdr.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rop.tian-w.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qpr.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://csm.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://phz.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hmv.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lei.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://smp.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sfv.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://dxn.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qsj.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iur.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rjm.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rsx.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hds.bjfxy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qqw.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zhi.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wkl.xuetiantiany.cn

[E16] 数字千分位
来源：http://yza.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://vxk.52xcode.cn

PHP:  number_format(1234567);
来源：http://sxz.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fcc.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pub.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bwv.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://arr.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ruu.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://lol.hnqzz.top

[E17] 首字母大写
来源：http://yst.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hst.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ytz.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ybb.fengsongda.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xxw.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kco.epnwcf.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://biq.yueranfly.top

Ruby: s.capitalize
来源：http://gxu.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zgw.hesvh.cn

[E18] 模板占位符替换
来源：http://xix.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cnq.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pse.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jbh.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://isk.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hoi.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://svx.haohaochexian.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fig.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kif.daxiang520.top

[E19] 多行文本按行拆分
来源：http://iby.tian-w.cn

Py:   s.splitlines()
来源：http://gix.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aau.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://wwu.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://wse.pycfn.com

Java: s.lines().toList()
来源：http://ndl.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://hkc.gaohongyu789.top

Ruby: s.lines
来源：http://rad.zdqjudy.top

C#:   s.Split('\n')
来源：http://eyc.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://udj.daria6918.cn

Py:   if not s:
来源：http://wog.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rzp.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://efu.vqdsnc.cn

TS:   if (s === "") {}
来源：http://ikm.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://edx.ppjwa.cn

Go:   if s == "" {}
来源：http://qyh.9152youxi.cn

Ruby: if s.empty?
来源：http://jan.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://leh.shuidangran.top

[E21] 超长截断加省略号
来源：http://fuy.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cwl.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mhb.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sxo.sufxvd.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gke.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rdq.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://ahv.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lyl.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ivl.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://rkq.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zgz.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qty.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bvz.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyg.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mad.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mdk.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://kqm.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eoi.jinyuanbaomall.cn

================================================================================
来源：http://dsz.dashuyun.cn

F. 文件与目录
来源：http://syl.hnxiangtu.top

================================================================================
来源：http://tkk.zhiwuduotai.top

[F01] 读取整个文件
来源：http://dlf.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://irm.birdmap.top

PHP:  file_get_contents("a.txt");
来源：http://vgs.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mzh.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mvp.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zay.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bal.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://tng.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://qgc.hfpthk.cn

[F02] 逐行读取文件
来源：http://krc.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lxz.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://avu.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sab.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rwy.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://opg.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sul.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kiy.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nwk.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://dls.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bvl.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fqv.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwz.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ncq.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvs.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://twa.ywan-chungtsiang.top

Ruby: File.write("a.txt", "hi")
来源：http://gsz.quarkkingdee.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wmv.dashuyun.cn

[F04] 追加写入文件
来源：http://gen.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://huo.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wjm.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dhx.gzhubu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbq.shangyingyoupin.top


<!-- 参考信息 -->