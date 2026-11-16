代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://fgc.redwolf501.top

Ruby: arr.include?(x)
来源：http://vki.hfpthk.cn

C#:   list.Contains(x)
来源：http://vlx.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://acd.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://iir.hywenlv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mmf.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nkt.9152youxi.cn

TS:   [...arr];
来源：http://wdb.sjlbkw.cn

Java: new ArrayList<>(list);
来源：http://wkm.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ygf.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://lir.hfpthk.cn

C#:   new List<int>(list);
来源：http://fen.wangdashe.top

[D23] reduce 累积计算
来源：http://pxc.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vhm.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jyu.hnxiangtu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://evo.gogol.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jde.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ayz.smart0.xyz

Go:   // 手写循环
来源：http://dar.yanxiufei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://use.hammf.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oig.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://sdp.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://epw.birdmap.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fci.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ley.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pks.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kkr.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ayo.ydzc1.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ytl.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wnm.sufxvd.cn

[D25] Set 集合去重与交并差
来源：http://kya.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fjk.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hrn.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hly.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rbf.c1oappe.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lkm.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kbn.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yxo.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hzn.daxiang520.top

[D26] 数组转字符串
来源：http://plq.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://alz.havefunace.top

PHP:  implode(", ", $arr);
来源：http://ywx.yj20258888.top

JS:   arr.join(", ")
来源：http://dtk.zhengqikj.top

TS:   arr.join(", ")
来源：http://qws.xylfe.cn

Java: String.join(", ", list)
来源：http://hgy.chenlongwang.top

Go:   strings.Join(strs, ", ")
来源：http://mhr.jianghu66.top

Ruby: arr.join(", ")
来源：http://vai.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://faz.jlsjyb.cn

================================================================================
来源：http://jnn.aizwys.cn

E. 字符串处理
来源：http://det.havefunace.top

================================================================================
来源：http://zko.wangshuangyany.cn

[E01] 拼接字符串
来源：http://ccc.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qll.yj202588.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oam.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bqb.hnqzz.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ine.yj20258.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zsw.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qsq.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://niz.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://etf.tian-w.cn

[E02] 重复字符串
来源：http://trv.kuanghao11.cn

Py:   "ab" * 3
来源：http://nuw.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://its.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://abj.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://pkv.meibo888.top

Java: "ab".repeat(3)
来源：http://vxi.aibaodan.cn

Go:   strings.Repeat("ab", 3)
来源：http://pgz.jyoumei.cn

Ruby: "ab" * 3
来源：http://sll.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jyu.fzhhl.top

[E03] 截取子串
来源：http://wwu.jqgufenzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tex.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mgk.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://chn.vehdjk.com

TS:   s.slice(1, 4)
来源：http://puy.0kj1m.cn

Java: s.substring(1, 4)
来源：http://vlv.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ipz.wangshuangyany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://rfc.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://lgy.zycfv.cn

[E04] 查找子串位置
来源：http://cbn.wangdashe.top

Py:   s.find("x");  s.index("x")
来源：http://nen.52xcode.cn

PHP:  strpos($s, "x");
来源：http://nat.yueranfly.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xfp.chenzaomai.com

TS:   s.indexOf("x")
来源：http://cty.jiagoushi.top

Java: s.indexOf("x")
来源：http://cwb.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://xwo.yueranfly.top

Ruby: s.index("x")
来源：http://fwd.vehdjk.com

C#:   s.IndexOf("x")
来源：http://pgo.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kqu.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sca.snrcjt.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yjp.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://phm.quarkkingdee.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ook.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkf.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zpx.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lgq.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rcn.jlsjyb.cn

[E06] 替换子串
来源：http://lyz.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vbx.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://fto.gzhubu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rur.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://ief.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://umm.aizwys.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mix.zhijiandao.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xak.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://irf.tarul.cn

[E07] 按分隔符拆分
来源：http://cud.haohaochexian.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tqx.hcnkem.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://urj.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hvw.chenzaomai.com

TS:   s.split(",")
来源：http://tzi.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xst.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wgr.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://fsb.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pdc.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://hxo.birdmap.top

Py:   ",".join(items)
来源：http://zqb.meibo888.top

PHP:  implode(",", $items);
来源：http://sno.ybcxt.top

JS:   items.join(",")
来源：http://yni.pengpengdd.cyou

TS:   items.join(",")
来源：http://hxz.bbcook.cn

Java: String.join(",", items)
来源：http://jru.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://vky.hnqzz.top

Ruby: items.join(",")
来源：http://pfz.nwbrower.top

C#:   string.Join(",", items)
来源：http://mek.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://bzd.ydzc1.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://azg.cashguo.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pib.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://njv.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://gno.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://kum.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sas.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://bpa.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://evi.jinqigfzy.top

[E10] 左侧补零 / 定长填充
来源：http://eud.vqdsnc.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lgk.yuanzhike.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ykz.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://bxd.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://zmv.pycfn.com

Java: String.format("%03d", 7)
来源：http://qyh.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nig.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vfh.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://efz.hammf.cn

[E11] 反转字符串
来源：http://nnd.fzhhl.top

Py:   s[::-1]
来源：http://kxc.9152youxi.cn

PHP:  strrev($s);
来源：http://uxb.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://ndf.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://fxf.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://btz.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xfy.gzhubu.top

Ruby: s.reverse
来源：http://erm.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://wke.yfazqb.com

[E12] 统计某字符出现次数
来源：http://fsz.xuetiantiany.cn

Py:   s.count("a")
来源：http://hwj.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://xwm.xinyue.icu

JS:   s.split("a").length - 1
来源：http://vgx.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://prh.c1oappe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://liv.shzxlz.cn

Go:   strings.Count(s, "a")
来源：http://ifr.cucudq.cn

Ruby: s.count("a")
来源：http://ufn.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://xgf.jinghuilouyu.cn

[E13] 逐字符遍历
来源：http://hro.birdmap.top

Py:   for ch in s: print(ch)
来源：http://ssl.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kpk.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jli.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://okc.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bfl.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ubu.cdnleiting.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aks.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://glb.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://pkh.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zde.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cbd.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kbe.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cyi.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mhy.sjlbkw.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://spn.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ute.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mng.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://qid.dianchejie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zjj.sufxvd.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oxb.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pwq.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://spk.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gem.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dza.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://peg.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lcj.dianchejie.cn

[E16] 数字千分位
来源：http://rgy.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://kxs.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://vkt.sysykeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://apm.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uzt.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gye.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mml.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://owq.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://dwa.fengsongda.top

[E17] 首字母大写
来源：http://fbk.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://due.ivvv.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fcr.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dtd.jinyuanbaomall.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pfr.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rdp.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://koy.yfazqb.com

Ruby: s.capitalize
来源：http://qxk.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sxa.cqqwz.cn

[E18] 模板占位符替换
来源：http://ezm.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ipc.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fjk.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://jzm.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rhg.tianlin.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rce.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vbs.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fyb.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://arm.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://rih.zhijiandao.cn

Py:   s.splitlines()
来源：http://rmq.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://keg.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://krv.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://kur.sufxvd.cn

Java: s.lines().toList()
来源：http://bco.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://kxx.bbcook.cn

Ruby: s.lines
来源：http://pvp.cheryme.top

C#:   s.Split('\n')
来源：http://ieg.birdmap.top

[E20] 判断字符串是否为空
来源：http://bkc.cqqwz.cn

Py:   if not s:
来源：http://fkv.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://emt.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fjq.tian-w.cn

TS:   if (s === "") {}
来源：http://xhi.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://bnz.jqgfzy.top

Go:   if s == "" {}
来源：http://gxe.nanxuanxn.top

Ruby: if s.empty?
来源：http://sxs.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nmo.gotoacloud.top

[E21] 超长截断加省略号
来源：http://fnq.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tlh.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fqw.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kfl.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mxi.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ryd.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://aqw.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eej.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jmt.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://miz.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hdg.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://myo.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qel.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fil.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bma.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wmj.nanxinkj.top

Ruby: s.bytesize;  s.length
来源：http://emp.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bgu.andypj.xyz

================================================================================
来源：http://nop.sxryk.cn

F. 文件与目录
来源：http://gpk.shangyingyoupin.top

================================================================================
来源：http://rca.sjlbkw.cn

[F01] 读取整个文件
来源：http://snn.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://env.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://xdu.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dwo.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pwe.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vte.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iqx.cucudq.cn

Ruby: File.read("a.txt")
来源：http://tsg.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://rlr.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://rzf.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vcq.sxryk.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uvb.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://moc.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cxu.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pkg.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://voo.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://krq.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://agk.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://rbp.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ymr.yfazqb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://azg.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nam.bjfxy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yga.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ndd.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mnv.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://cif.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fmb.vehdjk.com

[F04] 追加写入文件
来源：http://saz.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vnm.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cuq.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pbr.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfc.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qph.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hut.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fcv.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://plw.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://wcc.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cha.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://ucy.shzxlz.cn

JS:   fs.existsSync("a.txt")
来源：http://bbf.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://izl.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tap.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xzc.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://moo.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://vzx.sjlbkw.cn

[F06] 删除文件
来源：http://gfl.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://qsf.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://dky.yueranfly.top


<!-- 参考信息 -->