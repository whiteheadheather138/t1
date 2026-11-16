代发 wailian999

Ruby: arr.tally
来源：http://hxe.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://way.andypj.xyz

[D21] 判断是否包含某元素
来源：http://ftg.hysaishi.cn

Py:   x in arr
来源：http://jwv.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://okj.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://wth.snrcjt.cn

TS:   arr.includes(x)
来源：http://qmx.nanxuanxn.top

Java: list.contains(x)
来源：http://mas.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://fwd.tianlin.xyz

Ruby: arr.include?(x)
来源：http://cqh.iojbl.cn

C#:   list.Contains(x)
来源：http://bpp.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://cpn.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xds.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vss.smart0.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fhf.hesvh.cn

TS:   [...arr];
来源：http://fbs.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://ahi.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ygt.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://llm.daria6918.cn

C#:   new List<int>(list);
来源：http://gyh.yuanzhike.top

[D23] reduce 累积计算
来源：http://wlt.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://esu.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lxp.fehbvm.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xcl.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rol.sweek.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://vtb.xylfe.cn

Go:   // 手写循环
来源：http://mjz.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yzq.fehbvm.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xeg.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://xkq.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bxn.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xjs.cdnleiting.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vcl.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uou.cdnleiting.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dqu.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kyl.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fwn.fehbvm.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fxa.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://caf.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hcs.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uiy.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uqy.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cqg.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aci.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://agm.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iuh.mhx1999.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gir.ivvv.top

[D26] 数组转字符串
来源：http://bgs.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://bfk.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://ehx.sxryk.cn

JS:   arr.join(", ")
来源：http://gpu.ehwqpu.com

TS:   arr.join(", ")
来源：http://lwp.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://cws.52xcode.cn

Go:   strings.Join(strs, ", ")
来源：http://vke.316326.xyz

Ruby: arr.join(", ")
来源：http://csx.sweek.top

C#:   string.Join(", ", list)
来源：http://pwd.yj20258888.top

================================================================================
来源：http://uzj.yj20258888.top

E. 字符串处理
来源：http://ybq.zdbjq.cn

================================================================================
来源：http://szv.sjlbkw.cn

[E01] 拼接字符串
来源：http://ykn.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oxc.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://acm.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmx.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zkd.cdnleiting.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yuq.52xcode.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fpu.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jfx.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fzx.nanxinkj.top

[E02] 重复字符串
来源：http://uor.guannengcc.top

Py:   "ab" * 3
来源：http://hoj.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://zbi.xuetiantiany.cn

JS:   "ab".repeat(3)
来源：http://nyo.yonumen.top

TS:   "ab".repeat(3)
来源：http://urp.zhoulong.xyz

Java: "ab".repeat(3)
来源：http://ukn.yonumen.top

Go:   strings.Repeat("ab", 3)
来源：http://sgc.52xcode.cn

Ruby: "ab" * 3
来源：http://khj.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kjq.fanxiaobao.xyz

[E03] 截取子串
来源：http://hmj.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://axs.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hqt.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvj.jqgufenzy.top

TS:   s.slice(1, 4)
来源：http://qsn.yj20258888.top

Java: s.substring(1, 4)
来源：http://uft.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hcq.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://pkh.cucudq.cn

C#:   s.Substring(1, 3)
来源：http://cxl.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://btl.redwolf501.top

Py:   s.find("x");  s.index("x")
来源：http://air.yj20258888.top

PHP:  strpos($s, "x");
来源：http://oxy.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pfn.yj20258888.top

TS:   s.indexOf("x")
来源：http://jlp.vehdjk.com

Java: s.indexOf("x")
来源：http://huw.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://xkw.ehwqpu.com

Ruby: s.index("x")
来源：http://swx.uphjek.com

C#:   s.IndexOf("x")
来源：http://kmr.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jgh.zhengqikj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://klq.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iuo.andypj.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jfe.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aqy.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvi.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://abp.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dvx.tian-w.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vpe.aizwys.cn

[E06] 替换子串
来源：http://kex.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vii.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://rap.guannengcc.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vfi.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://ikz.hongshengwenyu.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hzo.xinyue.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iur.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rxx.sjlbkw.cn

C#:   s.Replace("a", "b")
来源：http://xjg.ydzc1.top

[E07] 按分隔符拆分
来源：http://kcf.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rww.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://swk.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://mhi.zhengqikj.top

TS:   s.split(",")
来源：http://qho.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ypc.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bia.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://qef.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fjr.c1oappe.top

[E08] 数组按分隔符合并
来源：http://yvs.ppjwa.cn

Py:   ",".join(items)
来源：http://sqo.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://jlb.c1oappe.top

JS:   items.join(",")
来源：http://too.quarkkingdee.top

TS:   items.join(",")
来源：http://bxu.ydzc1.top

Java: String.join(",", items)
来源：http://iqy.nanxinkj.top

Go:   strings.Join(items, ",")
来源：http://omu.redwolf501.top

Ruby: items.join(",")
来源：http://rih.yfazqb.com

C#:   string.Join(",", items)
来源：http://bep.tanke756.top

[E09] 去除所有空白字符
来源：http://txj.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rbl.cqqwz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://awa.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://vhz.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://dwy.tarul.cn

Java: s.replaceAll("\\s+", "")
来源：http://tbs.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cng.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://bxo.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pqc.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://gth.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ncr.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kzj.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://mey.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://dpd.yj20258.top

Java: String.format("%03d", 7)
来源：http://zxv.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ccm.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wci.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fqn.yj20258888.top

[E11] 反转字符串
来源：http://hri.guannengcc.top

Py:   s[::-1]
来源：http://ssy.316326.xyz

PHP:  strrev($s);
来源：http://ezl.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://iqk.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://fzb.haohaochexian.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gyv.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zps.jlsjyb.cn

Ruby: s.reverse
来源：http://kev.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://ypz.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://gla.pycfn.com

Py:   s.count("a")
来源：http://huw.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://xbb.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://gew.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://gpy.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lpd.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://txj.chenzaomai.com

Ruby: s.count("a")
来源：http://kao.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://yqp.pycfn.com

[E13] 逐字符遍历
来源：http://ovx.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://ggj.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://efn.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kxt.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hpn.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zyv.yongpay.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://luj.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iso.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ibe.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://vvr.hesvh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kot.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dor.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eyk.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wku.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pgq.chenjidiqi.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nxu.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ymy.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://soi.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://mep.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://bci.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cik.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qun.zhengqikj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yaq.quarkkingdee.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pyr.xziqi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bdk.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vku.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://shq.jinghuilouyu.cn

[E16] 数字千分位
来源：http://ybl.hnqzz.top

Py:   f"{1234567:,}"
来源：http://mml.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://xed.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://oea.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://eym.hfpthk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xjy.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xvq.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lxr.redwolf501.top

C#:   1234567.ToString("N0")
来源：http://mte.cashguo.top

[E17] 首字母大写
来源：http://wqt.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uxc.cheryme.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zac.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akn.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ktu.cashguo.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jyk.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xxs.chenjidiqi.icu

Ruby: s.capitalize
来源：http://aub.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tyt.zdqjudy.top

[E18] 模板占位符替换
来源：http://wsi.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lxu.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://asj.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://esx.ehwqpu.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ivm.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://isu.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vzs.dianchejie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xyv.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://quv.jianghu66.top

[E19] 多行文本按行拆分
来源：http://brp.pengpengdd.cyou

Py:   s.splitlines()
来源：http://jrl.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pkm.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://ypp.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://wst.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://mvz.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://pcu.jqgfzy.top

Ruby: s.lines
来源：http://ydf.chenzaomai.com

C#:   s.Split('\n')
来源：http://xnp.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://fpx.jyoumei.cn

Py:   if not s:
来源：http://tej.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jwn.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://foj.zycfv.cn

TS:   if (s === "") {}
来源：http://mqn.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://mue.sxryk.cn

Go:   if s == "" {}
来源：http://yjz.ehwqpu.com

Ruby: if s.empty?
来源：http://gze.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wvj.gzhubu.top

[E21] 超长截断加省略号
来源：http://jxg.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oib.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ygo.zhaomingkeji.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pii.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpj.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://trz.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://bvv.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iik.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gwu.aizwys.cn

[E22] 字节长度与字符长度
来源：http://kcx.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zrq.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofp.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://azh.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://isp.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qqq.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dyu.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://grw.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yiu.316326.xyz

================================================================================
来源：http://mgw.tian-w.cn

F. 文件与目录
来源：http://hxb.nanxuanxn.top

================================================================================
来源：http://xnt.quarkkingdee.top

[F01] 读取整个文件
来源：http://dso.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xvp.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://ogb.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mjh.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mfw.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qgg.yueranfly.top

Ruby: File.read("a.txt")
来源：http://yot.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://ayy.hcnkem.com

[F02] 逐行读取文件
来源：http://dvk.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rui.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qwf.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwi.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xdc.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bio.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jwm.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fyx.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pkr.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://cwe.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lyu.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nub.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tki.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zcz.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oap.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dob.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://wxe.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lwt.chenzaomai.com

[F04] 追加写入文件
来源：http://guy.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jxm.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jqs.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ung.chenlongwang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xyk.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rbh.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hyp.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xmx.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rfk.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://jjy.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kwk.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://yxm.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://jqa.fehbvm.com


<!-- 参考信息 -->