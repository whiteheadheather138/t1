代发 wailian999

Ruby: arr.tally
来源：http://ptg.fehbvm.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hjw.ivvv.top

[D21] 判断是否包含某元素
来源：http://hqc.jinqigufen.top

Py:   x in arr
来源：http://zcq.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://vew.316326.xyz

JS:   arr.includes(x)
来源：http://qec.yongpay.top

TS:   arr.includes(x)
来源：http://mdv.sysykeji.top

Java: list.contains(x)
来源：http://yra.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://pkl.yuanzhike.top

Ruby: arr.include?(x)
来源：http://svi.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://rap.xylfe.cn

[D22] 复制数组（避免共享引用）
来源：http://xvo.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://enp.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tkb.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zjr.wangshuangyany.cn

TS:   [...arr];
来源：http://ceb.sufxvd.cn

Java: new ArrayList<>(list);
来源：http://llq.0kj1m.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jkb.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://hov.ehwqpu.com

C#:   new List<int>(list);
来源：http://obf.jqgfzy.top

[D23] reduce 累积计算
来源：http://dke.zdbjq.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kch.sxryk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bnv.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://air.52xcode.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nvz.jqgufenzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://nvt.wangdashe.top

Go:   // 手写循环
来源：http://ted.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yfe.hongshengwenyu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hpe.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://viv.chenlongwang.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wmx.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rwx.zhiwuduotai.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mza.wangshuangyany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zzb.uphjek.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qui.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dct.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sjk.yj20258888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wvn.hfpthk.cn

[D25] Set 集合去重与交并差
来源：http://iig.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xen.daxiang520.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fxe.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kih.yanxiufei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oix.iojbl.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bvf.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://crc.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qbf.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ipu.fehbvm.com

[D26] 数组转字符串
来源：http://wqd.redwolf501.top

Py:   ", ".join(map(str, arr))
来源：http://ase.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://oiv.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://pbi.fehbvm.com

TS:   arr.join(", ")
来源：http://sxc.andypj.xyz

Java: String.join(", ", list)
来源：http://lxo.cucudq.cn

Go:   strings.Join(strs, ", ")
来源：http://udm.hfpthk.cn

Ruby: arr.join(", ")
来源：http://xav.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://xyv.ctjpmb.com

================================================================================
来源：http://xpq.guowangkeji.top

E. 字符串处理
来源：http://lpa.yfazqb.com

================================================================================
来源：http://epg.52xcode.cn

[E01] 拼接字符串
来源：http://wfg.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tca.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rke.yvedp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qqb.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bhg.cashguo.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://six.tianlin.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ueu.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ews.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jfa.zdqjudy.top

[E02] 重复字符串
来源：http://drl.dianchejie.cn

Py:   "ab" * 3
来源：http://ylb.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://rfm.bjfxy.top

JS:   "ab".repeat(3)
来源：http://gcm.nwbrower.top

TS:   "ab".repeat(3)
来源：http://oew.hnqzz.top

Java: "ab".repeat(3)
来源：http://puj.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://mgv.9152youxi.cn

Ruby: "ab" * 3
来源：http://jok.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qsj.yfazqb.com

[E03] 截取子串
来源：http://ymi.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iyx.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tpd.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vzr.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://yqt.fzhhl.top

Java: s.substring(1, 4)
来源：http://toq.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bna.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ron.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://vjd.yonumen.top

[E04] 查找子串位置
来源：http://vwo.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://sbh.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://jcr.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cxx.tian-w.cn

TS:   s.indexOf("x")
来源：http://hem.fengsongda.top

Java: s.indexOf("x")
来源：http://kth.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://zzy.pycfn.com

Ruby: s.index("x")
来源：http://piy.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://lcg.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fei.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pct.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pyt.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fqa.c1oappe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ikv.quarkkingdee.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ldo.xuetiantiany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zzl.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gdl.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pgm.gotoacloud.top

[E06] 替换子串
来源：http://zuh.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xct.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://vao.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yok.316326.xyz

TS:   s.replaceAll("a", "b")
来源：http://snm.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nts.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://una.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jfn.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://naa.fehbvm.com

[E07] 按分隔符拆分
来源：http://atw.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qlh.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rew.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://acc.wangshuangyany.cn

TS:   s.split(",")
来源：http://lty.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://otc.jinghuilouyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ntq.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://lho.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oaw.fengsongda.top

[E08] 数组按分隔符合并
来源：http://bjg.tian-w.cn

Py:   ",".join(items)
来源：http://udh.daxiang520.top

PHP:  implode(",", $items);
来源：http://hjb.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://jpg.fengsongda.top

TS:   items.join(",")
来源：http://vkf.sjlbkw.cn

Java: String.join(",", items)
来源：http://dqi.shanyushiyangtech.top

Go:   strings.Join(items, ",")
来源：http://nee.yj20258888.top

Ruby: items.join(",")
来源：http://wux.yuanzhike.top

C#:   string.Join(",", items)
来源：http://etd.gotoacloud.top

[E09] 去除所有空白字符
来源：http://jjd.tian-w.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dpp.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pme.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://bgr.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://kwt.havefunace.top

Java: s.replaceAll("\\s+", "")
来源：http://wyi.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bkg.sufxvd.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ndr.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xth.hysaishi.cn

[E10] 左侧补零 / 定长填充
来源：http://hmr.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wan.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zba.meibo888.top

JS:   "7".padStart(3, "0")
来源：http://unv.ctjpmb.com

TS:   "7".padStart(3, "0")
来源：http://ucp.daria6918.cn

Java: String.format("%03d", 7)
来源：http://rvy.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://qvh.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gmn.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sht.daria6918.cn

[E11] 反转字符串
来源：http://lsm.xziqi.cn

Py:   s[::-1]
来源：http://pcs.sjlbkw.cn

PHP:  strrev($s);
来源：http://bje.snrcjt.cn

JS:   [...s].reverse().join("")
来源：http://sqa.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://urg.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rzj.aizwys.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fqz.cashguo.top

Ruby: s.reverse
来源：http://iza.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qfx.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://jtx.sxryk.cn

Py:   s.count("a")
来源：http://muy.shangyingyoupin.top

PHP:  substr_count($s, "a");
来源：http://qbh.shanyushiyangtech.top

JS:   s.split("a").length - 1
来源：http://bqg.vehdjk.com

TS:   s.split("a").length - 1
来源：http://yoc.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jun.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://fag.bjfxy.top

Ruby: s.count("a")
来源：http://axz.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://cxw.hnqzz.top

[E13] 逐字符遍历
来源：http://mjr.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://wxh.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wfl.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mss.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://gga.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zue.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wvj.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lcv.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gen.yfazqb.com

[E14] URL 编码与 Base64
来源：http://pzw.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kwy.yongpay.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kvy.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wca.cucudq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yzt.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lpf.9152youxi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nog.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zfg.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mjx.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://eke.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hdy.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vlw.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tyc.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://whp.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dlq.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mtm.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rjg.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dvn.jqgufenzy.top

[E16] 数字千分位
来源：http://zyo.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://ydk.yvedp.cn

PHP:  number_format(1234567);
来源：http://eyl.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://znj.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://eqh.zycfv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nnj.zhongyouzk.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eni.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://upv.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://vjx.yongpay.top

[E17] 首字母大写
来源：http://oxy.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qwy.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://csu.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eef.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbf.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qjs.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kez.xylfe.cn

Ruby: s.capitalize
来源：http://hnh.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pbs.ctjpmb.com

[E18] 模板占位符替换
来源：http://sig.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dgp.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tfh.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://han.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ftz.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fjl.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zlt.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://icz.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uwe.shanyushiyangtech.top

[E19] 多行文本按行拆分
来源：http://gvh.pycfn.com

Py:   s.splitlines()
来源：http://aoc.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wdp.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://esk.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://ury.gogol.net.cn

Java: s.lines().toList()
来源：http://tcb.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://fop.bjfxy.top

Ruby: s.lines
来源：http://kqn.vqdsnc.cn

C#:   s.Split('\n')
来源：http://xck.zhixingplan.top

[E20] 判断字符串是否为空
来源：http://hpi.tian-w.cn

Py:   if not s:
来源：http://oib.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lod.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oax.iojbl.cn

TS:   if (s === "") {}
来源：http://ioa.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://ltp.zhengqikj.top

Go:   if s == "" {}
来源：http://rcy.xylfe.cn

Ruby: if s.empty?
来源：http://brw.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hcv.gzhubu.top

[E21] 超长截断加省略号
来源：http://loq.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vhl.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nud.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oyg.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uum.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rzf.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://elg.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://usv.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rlw.bbcook.cn

[E22] 字节长度与字符长度
来源：http://ouj.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eqp.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tkq.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cux.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vao.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://leq.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cjp.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://ydk.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gqu.hfpthk.cn

================================================================================
来源：http://tdu.xuanzx.com

F. 文件与目录
来源：http://fvv.svipenyu.cn

================================================================================
来源：http://zye.mhx1999.top

[F01] 读取整个文件
来源：http://qrz.cdnleiting.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://orh.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://irl.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vxp.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dtr.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qsf.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jyy.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://idc.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://gxa.zhengqikj.top

[F02] 逐行读取文件
来源：http://gsn.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rdj.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pxn.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eun.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nru.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ftc.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlg.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kht.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fue.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://meq.aibaodan.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ush.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ywz.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fcu.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpx.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xjs.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wmg.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://bvg.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vbn.shuidangran.top

[F04] 追加写入文件
来源：http://ffl.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hag.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wjt.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdm.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqd.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pwe.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fdm.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hvg.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jwj.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://rbn.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lvu.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://mhc.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://elr.zhaomingkeji.xyz


<!-- 参考信息 -->