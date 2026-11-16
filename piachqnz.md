代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://dzk.hcnkem.com

JS:   arr.includes(x)
来源：http://aml.zhongyouzk.top

TS:   arr.includes(x)
来源：http://jov.aizwys.cn

Java: list.contains(x)
来源：http://vnx.zhaomingkeji.xyz

Go:   slices.Contains(arr, x)
来源：http://wwf.hesvh.cn

Ruby: arr.include?(x)
来源：http://htc.hnqzz.top

C#:   list.Contains(x)
来源：http://gke.dashuyun.cn

[D22] 复制数组（避免共享引用）
来源：http://uph.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uzk.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mbx.epnwcf.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fra.wangdashe.top

TS:   [...arr];
来源：http://fcs.ywan-chungtsiang.top

Java: new ArrayList<>(list);
来源：http://ksj.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://nit.zhoulong.xyz

Ruby: arr.dup;  arr.clone
来源：http://eyh.fehbvm.com

C#:   new List<int>(list);
来源：http://iba.xuanzx.com

[D23] reduce 累积计算
来源：http://hfa.yonumen.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nbv.zycfv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ktf.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ydq.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yse.nwbrower.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://mkq.zycfv.cn

Go:   // 手写循环
来源：http://pfe.ydzc1.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kdd.zhiwuduotai.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jaa.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://rrx.guannengcc.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gop.zycfv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qjg.hywenlv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://log.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rwo.aizwys.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hcn.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ozd.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ksb.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zmp.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://ffs.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xdm.0kj1m.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wem.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dno.jqgufenzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qpa.wangdashe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dal.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jqy.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rxu.chenlongwang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lnz.birdmap.top

[D26] 数组转字符串
来源：http://obv.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://inf.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://hqc.zhengqikj.top

JS:   arr.join(", ")
来源：http://kqy.tian-w.cn

TS:   arr.join(", ")
来源：http://sis.yongpay.top

Java: String.join(", ", list)
来源：http://oal.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://oix.jiagoushi.top

Ruby: arr.join(", ")
来源：http://lkk.bjfxy.top

C#:   string.Join(", ", list)
来源：http://mbg.ydjk.org.cn

================================================================================
来源：http://xhr.yanxiufei.cn

E. 字符串处理
来源：http://xwo.sysykeji.top

================================================================================
来源：http://fac.fengsongda.top

[E01] 拼接字符串
来源：http://kxp.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aff.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vve.hnqzz.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uvh.cucudq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvk.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ngk.tarul.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ftl.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://czz.yueranfly.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oum.jinghuilouyu.cn

[E02] 重复字符串
来源：http://nki.tian-w.cn

Py:   "ab" * 3
来源：http://ooi.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://bom.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://pph.yfazqb.com

TS:   "ab".repeat(3)
来源：http://wwm.vehdjk.com

Java: "ab".repeat(3)
来源：http://uhh.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://zna.zdqjudy.top

Ruby: "ab" * 3
来源：http://xlg.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xyt.cdnleiting.top

[E03] 截取子串
来源：http://jgt.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rcd.xingfuxueyuan.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mbh.yuanzhike.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qvt.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://xso.haohaochexian.top

Java: s.substring(1, 4)
来源：http://xex.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nwf.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://xxw.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://hra.hnxiangtu.top

[E04] 查找子串位置
来源：http://maw.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://dix.ybcxt.top

PHP:  strpos($s, "x");
来源：http://tjq.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vgw.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://xaw.aizwys.cn

Java: s.indexOf("x")
来源：http://wqs.xingfuxueyuan.xyz

Go:   strings.Index(s, "x")
来源：http://wtw.aizwys.cn

Ruby: s.index("x")
来源：http://ypq.yueranfly.top

C#:   s.IndexOf("x")
来源：http://wxp.chenlongwang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dhd.hfpthk.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://omh.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ekk.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pnz.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://erp.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fby.c1oappe.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nlq.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pse.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tcb.birdmap.top

[E06] 替换子串
来源：http://prs.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://abd.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://bea.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zsp.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://aqq.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pvm.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qqc.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mbm.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://tee.yangfankeji.com

[E07] 按分隔符拆分
来源：http://rlf.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://obu.gaohongyu789.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tlo.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://oem.yangfankeji.com

TS:   s.split(",")
来源：http://tra.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://zmb.ehwqpu.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vnt.xinyue.icu

Ruby: s.split(",");  s.split
来源：http://fqr.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gqh.hnqzz.top

[E08] 数组按分隔符合并
来源：http://awz.chenjidiqi.icu

Py:   ",".join(items)
来源：http://xrj.sufxvd.cn

PHP:  implode(",", $items);
来源：http://mwp.tanke756.top

JS:   items.join(",")
来源：http://sxd.aibaodan.cn

TS:   items.join(",")
来源：http://nvh.pengpengdd.cyou

Java: String.join(",", items)
来源：http://xng.cucudq.cn

Go:   strings.Join(items, ",")
来源：http://kcm.sysykeji.top

Ruby: items.join(",")
来源：http://zib.yfazqb.com

C#:   string.Join(",", items)
来源：http://vyb.ydzc1.top

[E09] 去除所有空白字符
来源：http://twp.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hcw.yangfankeji.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qlj.gzhubu.top

JS:   s.replace(/\s+/g, "")
来源：http://oeq.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://ukf.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://xzl.ywan-chungtsiang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ywj.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://aip.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vwr.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://zet.zhongyouzk.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nnn.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uvb.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://rup.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://unq.bbcook.cn

Java: String.format("%03d", 7)
来源：http://wrq.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ies.yj20258.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cjt.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jcl.fanxiaobao.xyz

[E11] 反转字符串
来源：http://eyx.yj20258.top

Py:   s[::-1]
来源：http://taq.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://dmx.sufxvd.cn

JS:   [...s].reverse().join("")
来源：http://ezn.pycfn.com

TS:   [...s].reverse().join("")
来源：http://jnl.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zao.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ici.xinyue.icu

Ruby: s.reverse
来源：http://rpw.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lfv.dianchejie.cn

[E12] 统计某字符出现次数
来源：http://tqf.hysaishi.cn

Py:   s.count("a")
来源：http://wnk.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://bwu.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://pva.sxryk.cn

TS:   s.split("a").length - 1
来源：http://gpc.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dxm.yj20258.top

Go:   strings.Count(s, "a")
来源：http://zly.nanxuanxn.top

Ruby: s.count("a")
来源：http://eok.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://eec.chenzaomai.com

[E13] 逐字符遍历
来源：http://gng.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://yje.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jbr.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://zai.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bea.wangshuangyany.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dgk.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zrr.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://nns.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zta.sweek.top

[E14] URL 编码与 Base64
来源：http://dwm.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ged.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mif.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jjo.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vli.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rlc.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gby.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ege.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://isj.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://tgf.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vto.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ifw.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aak.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://svg.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eax.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dgp.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zzg.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tki.shangyingyoupin.top

[E16] 数字千分位
来源：http://gzp.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://oda.yongpay.top

PHP:  number_format(1234567);
来源：http://ppy.dianchejie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://koo.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://veb.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://noi.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pjz.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pyh.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://cct.jlsjyb.cn

[E17] 首字母大写
来源：http://zor.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fjw.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pdp.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gzb.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ioa.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pej.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kzq.shanyushiyangtech.top

Ruby: s.capitalize
来源：http://ntf.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zyq.yuanzhike.top

[E18] 模板占位符替换
来源：http://uou.zhengqikj.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qgp.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://izp.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fml.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fzx.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jut.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jfn.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xvw.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyh.ybcxt.top

[E19] 多行文本按行拆分
来源：http://fpx.jqgufenzy.top

Py:   s.splitlines()
来源：http://ihk.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nuq.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://xuw.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://ped.yfazqb.com

Java: s.lines().toList()
来源：http://lfm.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://obu.gzhubu.top

Ruby: s.lines
来源：http://roo.birdmap.top

C#:   s.Split('\n')
来源：http://czg.cheryme.top

[E20] 判断字符串是否为空
来源：http://ozl.gogol.net.cn

Py:   if not s:
来源：http://ibu.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hym.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vgp.jianghu66.top

TS:   if (s === "") {}
来源：http://trh.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://pjj.hnqzz.top

Go:   if s == "" {}
来源：http://myu.nwbrower.top

Ruby: if s.empty?
来源：http://mln.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bqo.0kj1m.cn

[E21] 超长截断加省略号
来源：http://otj.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vqk.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oty.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmj.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mry.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vsc.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://sai.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wwe.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://guf.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://hzs.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fui.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lcs.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rnh.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nvo.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bug.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aas.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://yeo.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ooc.ivvv.top

================================================================================
来源：http://uha.shanyushiyangtech.top

F. 文件与目录
来源：http://yab.shuidangran.top

================================================================================
来源：http://kuz.cheryme.top

[F01] 读取整个文件
来源：http://dtk.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zth.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://iiq.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bnf.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://prt.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://cgj.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oyh.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://qmk.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://tlb.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://ybp.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndg.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ngj.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fmi.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ifd.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gly.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://glv.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ums.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sum.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://mym.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jvt.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://yuk.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nis.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjr.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rmi.jinqigufen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fsz.birdmap.top

Ruby: File.write("a.txt", "hi")
来源：http://wnr.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oon.tianlin.xyz

[F04] 追加写入文件
来源：http://mub.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qnk.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yxh.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mux.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://buj.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nzm.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vkh.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kyu.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dus.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://vef.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oyo.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://dtl.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://pfx.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://opz.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cum.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bkp.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://yzu.hfpthk.cn


<!-- 参考信息 -->