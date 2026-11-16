代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eih.ybcxt.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kwn.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nfw.quarkkingdee.top

TS:   [...arr];
来源：http://qku.guowangkeji.top

Java: new ArrayList<>(list);
来源：http://atz.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://zdf.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://taz.sysykeji.top

C#:   new List<int>(list);
来源：http://hrh.feifeiyinyue.top

[D23] reduce 累积计算
来源：http://hfg.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kul.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cei.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bui.jqgfzy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ehp.jqgfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oyi.jinqigfzy.top

Go:   // 手写循环
来源：http://xhw.pengpengdd.cyou

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vnn.fanxiaobao.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nvy.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://ahy.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zgp.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uhj.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mdf.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sgq.guannengcc.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lir.cheryme.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://poi.tarul.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dfs.ywan-chungtsiang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zef.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://soq.wangdashe.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://prb.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hez.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://egy.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xai.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eom.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vhn.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cnv.iojbl.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ltt.zdqjudy.top

[D26] 数组转字符串
来源：http://sdk.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://ikb.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://vtn.yueranfly.top

JS:   arr.join(", ")
来源：http://zuz.yuxming.cn

TS:   arr.join(", ")
来源：http://eas.nanxinkj.top

Java: String.join(", ", list)
来源：http://puy.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://xmf.sysykeji.top

Ruby: arr.join(", ")
来源：http://dpz.fengsongda.top

C#:   string.Join(", ", list)
来源：http://tqh.yonumen.top

================================================================================
来源：http://tag.aibaodan.cn

E. 字符串处理
来源：http://hol.yfazqb.com

================================================================================
来源：http://dgt.chenlongwang.top

[E01] 拼接字符串
来源：http://whs.vqdsnc.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pga.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lew.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bvn.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rrh.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lvj.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ljc.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://acj.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qag.bjfxy.top

[E02] 重复字符串
来源：http://gbg.shzxlz.cn

Py:   "ab" * 3
来源：http://ccx.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://wyc.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://uyx.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://nlf.nanxinkj.top

Java: "ab".repeat(3)
来源：http://bmh.daxiang520.top

Go:   strings.Repeat("ab", 3)
来源：http://zho.jqgfzy.top

Ruby: "ab" * 3
来源：http://eoq.guannengcc.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hhy.yuanzhike.top

[E03] 截取子串
来源：http://vio.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pvi.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vzz.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rwc.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://mgb.zhengqikj.top

Java: s.substring(1, 4)
来源：http://sam.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mwx.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://xoa.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://eud.daxiang520.top

[E04] 查找子串位置
来源：http://ikt.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://raq.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://evu.zhixingplan.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eon.yfazqb.com

TS:   s.indexOf("x")
来源：http://aef.yj20258.top

Java: s.indexOf("x")
来源：http://odn.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://ian.zhongyouzk.top

Ruby: s.index("x")
来源：http://oyo.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://bja.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nim.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kin.nanxuanxn.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://end.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rwz.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yfk.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgm.chenlongwang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sfb.zhijiandao.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://msb.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dmp.jqgfzy.top

[E06] 替换子串
来源：http://bew.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ttv.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://hbn.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://atc.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://gdx.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://epp.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zgn.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zie.ybcxt.top

C#:   s.Replace("a", "b")
来源：http://dhq.andypj.xyz

[E07] 按分隔符拆分
来源：http://xmk.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hlt.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jvg.bbcook.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hjt.sysykeji.top

TS:   s.split(",")
来源：http://slt.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://oxl.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tig.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://axm.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hgc.zhixingplan.top

[E08] 数组按分隔符合并
来源：http://gvb.jqgufenzy.top

Py:   ",".join(items)
来源：http://ptm.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://sbm.jinqigfzy.top

JS:   items.join(",")
来源：http://urk.nanxinkj.top

TS:   items.join(",")
来源：http://qol.9152youxi.cn

Java: String.join(",", items)
来源：http://syd.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://rzx.bbcook.cn

Ruby: items.join(",")
来源：http://zjm.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://puc.daxiang520.top

[E09] 去除所有空白字符
来源：http://ype.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rfm.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://abb.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://txu.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://orb.cucudq.cn

Java: s.replaceAll("\\s+", "")
来源：http://msb.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ivr.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://oxp.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aig.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://ihp.nanxuanxn.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qoa.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uoj.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://eki.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://qgw.sufxvd.cn

Java: String.format("%03d", 7)
来源：http://fuk.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ivy.redwolf501.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rex.hfpthk.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xwe.smart0.xyz

[E11] 反转字符串
来源：http://bwq.snrcjt.cn

Py:   s[::-1]
来源：http://nyq.snrcjt.cn

PHP:  strrev($s);
来源：http://rzd.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://ubv.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://meq.yangfankeji.com

Java: new StringBuilder(s).reverse().toString()
来源：http://myt.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://ahx.gzhubu.top

Ruby: s.reverse
来源：http://ubn.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://cmd.fehbvm.com

[E12] 统计某字符出现次数
来源：http://hto.hywenlv.cn

Py:   s.count("a")
来源：http://tuu.316326.xyz

PHP:  substr_count($s, "a");
来源：http://rwu.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://uhe.daxiang520.top

TS:   s.split("a").length - 1
来源：http://shr.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pig.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://isc.yfazqb.com

Ruby: s.count("a")
来源：http://bip.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://bfz.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://gvl.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://rfw.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wvb.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://emm.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xfm.svipenyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uix.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://afk.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gun.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yec.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://bds.dashuyun.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cim.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://win.epnwcf.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://los.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://umj.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mse.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pss.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fyc.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oas.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://gnq.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wha.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qmr.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pwd.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jwb.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nxc.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://azj.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qqr.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zko.iojbl.cn

[E16] 数字千分位
来源：http://rkh.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://zmv.jyoumei.cn

PHP:  number_format(1234567);
来源：http://fba.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fhg.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mwo.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mrq.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ppt.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kbw.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://iju.yuanzhike.top

[E17] 首字母大写
来源：http://hkz.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://srz.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mxz.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbh.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mmv.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://abc.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ixc.xuetiantiany.cn

Ruby: s.capitalize
来源：http://hjl.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://guz.ydzc1.top

[E18] 模板占位符替换
来源：http://iju.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jps.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qfw.jiagoushi.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mdi.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kxt.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xsm.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dds.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zro.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tly.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://oxg.cheryme.top

Py:   s.splitlines()
来源：http://lum.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kct.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://aeu.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://nyd.52xcode.cn

Java: s.lines().toList()
来源：http://yeu.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://nmw.jiagoushi.top

Ruby: s.lines
来源：http://inu.vehdjk.com

C#:   s.Split('\n')
来源：http://nms.cashguo.top

[E20] 判断字符串是否为空
来源：http://kii.c1oappe.top

Py:   if not s:
来源：http://tow.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yea.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dpa.iojbl.cn

TS:   if (s === "") {}
来源：http://goq.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://qxa.vehdjk.com

Go:   if s == "" {}
来源：http://oak.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://xun.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oix.yuanzhike.top

[E21] 超长截断加省略号
来源：http://gmz.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rdm.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pzo.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vcc.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://acv.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://puk.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://aro.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://avl.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mfb.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://gex.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mwi.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://otf.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrz.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mcx.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exa.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://unn.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://flk.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aca.52xcode.cn

================================================================================
来源：http://jtj.jinqigfzy.top

F. 文件与目录
来源：http://oer.feifeiyinyue.top

================================================================================
来源：http://wiz.havefunace.top

[F01] 读取整个文件
来源：http://rlc.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mxb.zdqjudy.top

PHP:  file_get_contents("a.txt");
来源：http://cav.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qso.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vgy.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xcu.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pgm.cheryme.top

Ruby: File.read("a.txt")
来源：http://kkm.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://myp.nanxuanxn.top

[F02] 逐行读取文件
来源：http://tex.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lkx.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ond.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixx.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hat.yueranfly.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aog.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jos.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://min.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ykq.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://mlu.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oks.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gox.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bck.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://quw.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lpj.hysaishi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://glj.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://nms.vqdsnc.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ezt.haohaochexian.top

[F04] 追加写入文件
来源：http://uzx.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jgv.bjfxy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mql.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tbr.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fqa.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oqc.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bcl.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eed.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://owh.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://nlw.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://irp.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://set.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://yaf.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://ber.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://dwu.guannengcc.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xjb.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://hmj.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://ljw.tianlin.xyz

[F06] 删除文件
来源：http://uew.andypj.xyz

Py:   os.remove("a.txt")
来源：http://eld.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://dkp.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nra.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kus.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtb.yonumen.top

Go:   os.Remove("a.txt")
来源：http://ilb.tianlin.xyz


<!-- 参考信息 -->