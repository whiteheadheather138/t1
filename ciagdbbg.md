代发 wailian999

Ruby: arr.tally
来源：http://bkh.jinqigufen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://weg.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://qgp.hongshengwenyu.top

Py:   x in arr
来源：http://kog.yj20258.top

PHP:  in_array($x, $arr, true);
来源：http://ife.jqgufenzy.top

JS:   arr.includes(x)
来源：http://avp.sysykeji.top

TS:   arr.includes(x)
来源：http://hgk.jlsjyb.cn

Java: list.contains(x)
来源：http://yxr.zhijiandao.cn

Go:   slices.Contains(arr, x)
来源：http://gli.shzxlz.cn

Ruby: arr.include?(x)
来源：http://byr.wangdashe.top

C#:   list.Contains(x)
来源：http://yry.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://zxz.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sbd.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://def.hammf.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rmx.jinqigufen.top

TS:   [...arr];
来源：http://ojs.daxiang520.top

Java: new ArrayList<>(list);
来源：http://fgm.gotoacloud.top

Go:   copied := append([]int(nil), arr...)
来源：http://mpt.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://dia.tarul.cn

C#:   new List<int>(list);
来源：http://hxf.xuanzx.com

[D23] reduce 累积计算
来源：http://mts.xuetiantiany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://idg.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hrt.svipenyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmk.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rgm.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nms.hesvh.cn

Go:   // 手写循环
来源：http://kus.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ror.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://siy.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://obe.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://inv.smart0.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://buu.mhx1999.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bia.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fsl.cheryme.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wtl.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vax.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://luf.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qaf.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://vzc.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://abj.xuanzx.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://txd.yuanzhike.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lgl.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://goi.tian-w.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mez.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fby.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://spq.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rwr.pycfn.com

[D26] 数组转字符串
来源：http://pop.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://uvp.zhixingplan.top

PHP:  implode(", ", $arr);
来源：http://ugb.yj202588.top

JS:   arr.join(", ")
来源：http://yul.havefunace.top

TS:   arr.join(", ")
来源：http://fdn.nanxinkj.top

Java: String.join(", ", list)
来源：http://gdu.sufxvd.cn

Go:   strings.Join(strs, ", ")
来源：http://abj.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://ksx.gogol.net.cn

C#:   string.Join(", ", list)
来源：http://qgl.iojbl.cn

================================================================================
来源：http://iio.jqgfzy.top

E. 字符串处理
来源：http://xkq.shangyingyoupin.top

================================================================================
来源：http://piu.zhixingplan.top

[E01] 拼接字符串
来源：http://btb.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dtc.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pma.daxiang520.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zct.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jem.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lne.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qix.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yfp.meibo888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oce.sysykeji.top

[E02] 重复字符串
来源：http://maz.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://dop.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://wff.yueranfly.top

JS:   "ab".repeat(3)
来源：http://uly.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://owc.daria6918.cn

Java: "ab".repeat(3)
来源：http://tus.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://wyy.hysaishi.cn

Ruby: "ab" * 3
来源：http://wry.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iil.hongshengwenyu.top

[E03] 截取子串
来源：http://upd.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zqd.gzhubu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vcp.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gxr.gotoacloud.top

TS:   s.slice(1, 4)
来源：http://aek.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://twk.jiagoushi.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qrr.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://tim.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://dkz.snrcjt.cn

[E04] 查找子串位置
来源：http://zwv.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://rra.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://ykv.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eew.sufxvd.cn

TS:   s.indexOf("x")
来源：http://dtt.jqgfzy.top

Java: s.indexOf("x")
来源：http://xxh.pycfn.com

Go:   strings.Index(s, "x")
来源：http://rwd.hnqzz.top

Ruby: s.index("x")
来源：http://soi.ivvv.top

C#:   s.IndexOf("x")
来源：http://dkb.jqgfzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://thm.andypj.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jzm.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eke.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfz.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://mgm.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gev.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sln.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://saw.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://itd.pycfn.com

[E06] 替换子串
来源：http://srk.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://psj.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://xud.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jzb.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://xyj.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gpi.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ngj.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wqq.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://gfj.zycfv.cn

[E07] 按分隔符拆分
来源：http://tce.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ebi.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://heb.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lug.meibo888.top

TS:   s.split(",")
来源：http://ocl.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jgi.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ydl.sweek.top

Ruby: s.split(",");  s.split
来源：http://its.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ipe.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://uvp.zhongyouzk.top

Py:   ",".join(items)
来源：http://xdz.redwolf501.top

PHP:  implode(",", $items);
来源：http://okr.andypj.xyz

JS:   items.join(",")
来源：http://hua.iojbl.cn

TS:   items.join(",")
来源：http://xbf.hnqzz.top

Java: String.join(",", items)
来源：http://jqb.sxryk.cn

Go:   strings.Join(items, ",")
来源：http://kzg.sysykeji.top

Ruby: items.join(",")
来源：http://kvs.aizwys.cn

C#:   string.Join(",", items)
来源：http://zjq.tianlin.xyz

[E09] 去除所有空白字符
来源：http://lwi.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hoa.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ypd.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://rgk.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://jiu.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://oxx.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eps.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://zmk.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qmb.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://hfj.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eel.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jpz.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://huu.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://sxs.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://rhz.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cos.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vxr.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mqs.smart0.xyz

[E11] 反转字符串
来源：http://ijq.yanxiufei.cn

Py:   s[::-1]
来源：http://hmh.ppjwa.cn

PHP:  strrev($s);
来源：http://cuo.uphjek.com

JS:   [...s].reverse().join("")
来源：http://biq.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://nsx.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://tqq.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zjc.yongpay.top

Ruby: s.reverse
来源：http://ohi.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://noa.sxryk.cn

[E12] 统计某字符出现次数
来源：http://idz.ctjpmb.com

Py:   s.count("a")
来源：http://hjh.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://hnt.yj20258888.top

JS:   s.split("a").length - 1
来源：http://skz.fehbvm.com

TS:   s.split("a").length - 1
来源：http://fsb.zhoulong.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yfo.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://jto.52xcode.cn

Ruby: s.count("a")
来源：http://sdn.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://ilc.bbcook.cn

[E13] 逐字符遍历
来源：http://idq.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://goh.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bmo.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://epo.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://avc.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xwn.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vtc.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tki.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://onn.pycfn.com

[E14] URL 编码与 Base64
来源：http://dbs.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xoc.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://znf.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ihx.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jxh.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tgt.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rpl.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ctq.daxiang520.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pvw.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://cqe.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sgy.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qsz.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vcf.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jtu.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qdk.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pmh.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cvb.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://irf.bjfxy.top

[E16] 数字千分位
来源：http://yij.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://jmk.vehdjk.com

PHP:  number_format(1234567);
来源：http://uts.shuidangran.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jdo.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://fti.hywenlv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kgk.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjw.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://umg.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://mdc.jinqigufen.top

[E17] 首字母大写
来源：http://smc.haohaochexian.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xwj.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ggk.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aax.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mmh.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zeq.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hwi.hnxiangtu.top

Ruby: s.capitalize
来源：http://wyf.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ohv.redwolf501.top

[E18] 模板占位符替换
来源：http://apm.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fzs.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hwg.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://yos.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://leq.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pyy.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://btl.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jba.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bhc.fzhhl.top

[E19] 多行文本按行拆分
来源：http://jrv.tian-w.cn

Py:   s.splitlines()
来源：http://otm.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rve.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://xkv.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://she.ctjpmb.com

Java: s.lines().toList()
来源：http://wxw.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://ofd.vehdjk.com

Ruby: s.lines
来源：http://kfr.shuidangran.top

C#:   s.Split('\n')
来源：http://pzv.andypj.xyz

[E20] 判断字符串是否为空
来源：http://dkg.chenjidiqi.icu

Py:   if not s:
来源：http://hhb.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpt.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hpk.vehdjk.com

TS:   if (s === "") {}
来源：http://jze.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://nja.bbcook.cn

Go:   if s == "" {}
来源：http://gkb.hnqzz.top

Ruby: if s.empty?
来源：http://blt.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qsq.gogol.net.cn

[E21] 超长截断加省略号
来源：http://myq.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jsx.cheryme.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pko.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pvd.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zse.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://exq.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://bpp.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ixb.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://okb.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://iec.chenjidiqi.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sca.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nrc.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://viz.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cph.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kjo.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bay.chenzaomai.com

Ruby: s.bytesize;  s.length
来源：http://prg.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hfk.haohaochexian.top

================================================================================
来源：http://tlu.xziqi.cn

F. 文件与目录
来源：http://lcn.ehwqpu.com

================================================================================
来源：http://ysb.gaohongyu789.top

[F01] 读取整个文件
来源：http://bfa.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jjd.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://pnh.zhijiandao.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://upk.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irf.daxiang520.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fgk.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mrw.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://lug.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://zbw.fzhhl.top

[F02] 逐行读取文件
来源：http://sby.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xlk.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jhg.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ucl.zhengqikj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://opa.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qyb.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rkv.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://brw.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iay.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://lqe.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aar.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://srf.xuanzx.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztm.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hgf.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tnk.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bjj.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://duf.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cvf.svipenyu.cn

[F04] 追加写入文件
来源：http://cwk.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://inm.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sga.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mod.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yph.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oth.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ezi.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kij.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ccl.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://ask.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bpc.ivvv.top

PHP:  file_exists("a.txt");
来源：http://cjy.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://kyv.chenzaomai.com


<!-- 参考信息 -->