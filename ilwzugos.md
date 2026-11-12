代发 wailian999

Ruby: arr.tally
来源：http://nsi.wangshuangyany.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ulu.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://vfk.haohaochexian.top

Py:   x in arr
来源：http://ply.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://lra.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://kst.9152youxi.cn

TS:   arr.includes(x)
来源：http://oqu.feifeiyinyue.top

Java: list.contains(x)
来源：http://snh.andypj.xyz

Go:   slices.Contains(arr, x)
来源：http://edb.c1oappe.top

Ruby: arr.include?(x)
来源：http://xsl.xinyue.icu

C#:   list.Contains(x)
来源：http://pxb.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://bdw.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eoi.yongpay.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nof.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bjt.sweek.top

TS:   [...arr];
来源：http://pzg.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://xxp.zhoulong.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://vql.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://sxa.316326.xyz

C#:   new List<int>(list);
来源：http://aue.kuanghao11.cn

[D23] reduce 累积计算
来源：http://ndr.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gei.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dbe.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sgw.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lsk.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mfv.hfpthk.cn

Go:   // 手写循环
来源：http://vmb.tanke756.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dog.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tiv.ydzc1.top

[D24] 字典 / Map 基本操作
来源：http://tos.c1oappe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ywg.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nyi.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://akk.jqgufenzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dhy.wangshuangyany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vkn.hammf.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ggg.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mld.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ujv.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://fpf.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://avl.pycfn.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aoj.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kwb.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jvu.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eyc.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ddi.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://snh.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lot.hammf.cn

[D26] 数组转字符串
来源：http://pej.vqdsnc.cn

Py:   ", ".join(map(str, arr))
来源：http://bhk.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://avm.jyoumei.cn

JS:   arr.join(", ")
来源：http://htf.shanyushiyangtech.top

TS:   arr.join(", ")
来源：http://wsd.xziqi.cn

Java: String.join(", ", list)
来源：http://rro.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://euh.hesvh.cn

Ruby: arr.join(", ")
来源：http://dly.hesvh.cn

C#:   string.Join(", ", list)
来源：http://ypq.bbcook.cn

================================================================================
来源：http://bda.ybcxt.top

E. 字符串处理
来源：http://odv.yj20258888.top

================================================================================
来源：http://ayy.yuanzhike.top

[E01] 拼接字符串
来源：http://fac.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ica.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vdd.yonumen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qtl.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mbl.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zas.jinghuilouyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cvj.jinghuilouyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uoq.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nlk.andypj.xyz

[E02] 重复字符串
来源：http://ytv.vehdjk.com

Py:   "ab" * 3
来源：http://cjs.ybcxt.top

PHP:  str_repeat("ab", 3);
来源：http://giw.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://zso.316326.xyz

TS:   "ab".repeat(3)
来源：http://nfq.jinghuilouyu.cn

Java: "ab".repeat(3)
来源：http://jsn.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://mon.hnqzz.top

Ruby: "ab" * 3
来源：http://fuf.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cyp.zhengqikj.top

[E03] 截取子串
来源：http://xze.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dqz.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lgc.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lwn.yfazqb.com

TS:   s.slice(1, 4)
来源：http://qyv.sweek.top

Java: s.substring(1, 4)
来源：http://cqb.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jbj.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qel.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://acw.svipenyu.cn

[E04] 查找子串位置
来源：http://iyk.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://uja.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://dra.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gnz.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://lxz.fktsv.cn

Java: s.indexOf("x")
来源：http://pxx.wangdashe.top

Go:   strings.Index(s, "x")
来源：http://zxr.guowangkeji.top

Ruby: s.index("x")
来源：http://vtu.yongpay.top

C#:   s.IndexOf("x")
来源：http://bnq.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://iyl.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://daa.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vup.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vjs.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vha.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ljt.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wdx.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njz.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://egb.ybcxt.top

[E06] 替换子串
来源：http://vsc.chenzaomai.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://etb.jiagoushi.top

PHP:  str_replace("a", "b", $s);
来源：http://hpm.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nzu.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://vdo.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pyt.vehdjk.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bvl.cucudq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hhz.gaohongyu789.top

C#:   s.Replace("a", "b")
来源：http://zcr.meibo888.top

[E07] 按分隔符拆分
来源：http://gma.yj20258.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ulk.redwolf501.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iib.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://epz.zycfv.cn

TS:   s.split(",")
来源：http://sax.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://ufm.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qcl.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://rwf.jinyuanbaomall.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rml.aizwys.cn

[E08] 数组按分隔符合并
来源：http://dcu.zdqjudy.top

Py:   ",".join(items)
来源：http://ibc.sweek.top

PHP:  implode(",", $items);
来源：http://yzg.hongshengwenyu.top

JS:   items.join(",")
来源：http://guj.ctjpmb.com

TS:   items.join(",")
来源：http://uuu.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://kxy.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://wxa.jinqigfzy.top

Ruby: items.join(",")
来源：http://fhn.chenlongwang.top

C#:   string.Join(",", items)
来源：http://zkq.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://nti.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vye.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://phg.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://qsr.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://lnp.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://dlu.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://asx.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://sbl.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fdf.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://ess.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iri.snrcjt.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yig.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://hgm.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://xat.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://qdg.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://bxr.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bob.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qda.yfazqb.com

[E11] 反转字符串
来源：http://igv.andypj.xyz

Py:   s[::-1]
来源：http://rkz.shangyingyoupin.top

PHP:  strrev($s);
来源：http://xrb.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://dwj.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://alo.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kpo.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cvv.tarul.cn

Ruby: s.reverse
来源：http://hmj.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kqo.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://dro.316326.xyz

Py:   s.count("a")
来源：http://zno.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://sub.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://ydy.fzhhl.top

TS:   s.split("a").length - 1
来源：http://kvj.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wmx.uphjek.com

Go:   strings.Count(s, "a")
来源：http://sol.0kj1m.cn

Ruby: s.count("a")
来源：http://apm.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://cyf.wangshuangyany.cn

[E13] 逐字符遍历
来源：http://bsz.yonumen.top

Py:   for ch in s: print(ch)
来源：http://ggm.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://plz.yanxiufei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ngw.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kei.yueranfly.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lst.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rcb.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xwa.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dfk.sweek.top

[E14] URL 编码与 Base64
来源：http://kxd.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://svv.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lrl.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ujf.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gfg.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pxt.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gtd.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vta.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sco.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://mtg.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pju.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qnh.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://szr.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sfo.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pep.yj20258.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zyh.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gwq.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dmi.fzhhl.top

[E16] 数字千分位
来源：http://fes.yuxming.cn

Py:   f"{1234567:,}"
来源：http://frp.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://fvk.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://pig.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nuh.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vyp.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tds.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yqb.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://jtq.zhijiandao.cn

[E17] 首字母大写
来源：http://kkt.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ovj.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ajm.zhaomingkeji.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://htu.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ive.jinyuanbaomall.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://isr.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xue.chenzaomai.com

Ruby: s.capitalize
来源：http://zmj.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vrh.hesvh.cn

[E18] 模板占位符替换
来源：http://lfd.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mcm.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://apj.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nah.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://jpm.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ikp.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ttr.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aqy.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ehl.shuidangran.top

[E19] 多行文本按行拆分
来源：http://jck.yuxming.cn

Py:   s.splitlines()
来源：http://jtb.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kjj.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://nks.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://eqi.yj20258.top

Java: s.lines().toList()
来源：http://cgs.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://vmu.sysykeji.top

Ruby: s.lines
来源：http://jts.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://qan.yvedp.cn

[E20] 判断字符串是否为空
来源：http://dfq.aibaodan.cn

Py:   if not s:
来源：http://xxr.daxiang520.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ezv.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vhv.zhixingplan.top

TS:   if (s === "") {}
来源：http://abt.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://gsi.fzhhl.top

Go:   if s == "" {}
来源：http://qlk.chenjidiqi.icu

Ruby: if s.empty?
来源：http://xof.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tcr.hfpthk.cn

[E21] 超长截断加省略号
来源：http://rrx.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sjq.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tmc.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsp.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://con.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbw.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://rmt.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jne.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ztr.meibo888.top

[E22] 字节长度与字符长度
来源：http://qxx.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://srl.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vdm.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ldk.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dkb.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fyc.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mrk.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://xnk.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://onp.zdqjudy.top

================================================================================
来源：http://odw.xziqi.cn

F. 文件与目录
来源：http://hrw.hcnkem.com

================================================================================
来源：http://uoc.xinyue.icu

[F01] 读取整个文件
来源：http://mrt.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nxp.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://arb.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sqm.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://huh.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ncz.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zgh.nwbrower.top

Ruby: File.read("a.txt")
来源：http://xbg.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://koo.hammf.cn

[F02] 逐行读取文件
来源：http://tcu.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ifn.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mdg.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pec.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gmn.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://txb.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rxv.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bba.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kol.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://xyo.cheryme.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sli.zhixingplan.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wku.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsa.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nub.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rwp.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aju.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://ohs.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://afu.quarkkingdee.top

[F04] 追加写入文件
来源：http://lml.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://owe.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://czi.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://czm.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dll.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wir.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xum.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ukv.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hrq.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://mvi.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tfu.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://awb.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://lfc.jinqigfzy.top


<!-- 参考信息 -->