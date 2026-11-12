代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mwg.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zpc.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jus.jqgfzy.top

TS:   [...arr];
来源：http://abf.tian-w.cn

Java: new ArrayList<>(list);
来源：http://iju.hcnkem.com

Go:   copied := append([]int(nil), arr...)
来源：http://kca.fktsv.cn

Ruby: arr.dup;  arr.clone
来源：http://rlx.sweek.top

C#:   new List<int>(list);
来源：http://ptl.cheryme.top

[D23] reduce 累积计算
来源：http://jat.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vmg.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://laa.guannengcc.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wkn.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lju.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tvx.yvedp.cn

Go:   // 手写循环
来源：http://ded.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ywf.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://azs.dianchejie.cn

[D24] 字典 / Map 基本操作
来源：http://kko.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mma.cdnleiting.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://chi.jinqigfzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zvi.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yeq.fanxiaobao.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pph.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lpv.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bfh.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qzx.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://nsu.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gyi.cqqwz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lbo.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rgo.cheryme.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wqj.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sis.shangyingyoupin.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sut.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hlr.ppjwa.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nze.nanxuanxn.top

[D26] 数组转字符串
来源：http://lmi.xinyue.icu

Py:   ", ".join(map(str, arr))
来源：http://pdd.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://xgd.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://mya.gzhubu.top

TS:   arr.join(", ")
来源：http://tmf.wangdashe.top

Java: String.join(", ", list)
来源：http://nhg.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://dky.zhengqikj.top

Ruby: arr.join(", ")
来源：http://qwo.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://the.yuanzhike.top

================================================================================
来源：http://tko.cheryme.top

E. 字符串处理
来源：http://qhi.cheryme.top

================================================================================
来源：http://dah.zycfv.cn

[E01] 拼接字符串
来源：http://khz.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hui.ctjpmb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pwp.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcj.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rgj.hywenlv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://epj.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://brv.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vyo.xingfuxueyuan.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uvm.kuanghao11.cn

[E02] 重复字符串
来源：http://zqh.yj20258.top

Py:   "ab" * 3
来源：http://nlj.hywenlv.cn

PHP:  str_repeat("ab", 3);
来源：http://qsm.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://hej.snrcjt.cn

TS:   "ab".repeat(3)
来源：http://rtf.hfpthk.cn

Java: "ab".repeat(3)
来源：http://rkh.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://hkx.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://fmq.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uxn.jinyuanbaomall.cn

[E03] 截取子串
来源：http://bvh.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rvf.tanke756.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vdm.ydjk.org.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oww.nwbrower.top

TS:   s.slice(1, 4)
来源：http://ntv.yj20258.top

Java: s.substring(1, 4)
来源：http://ihv.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vza.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://vor.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://tfw.feifeiyinyue.top

[E04] 查找子串位置
来源：http://uft.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://lok.hammf.cn

PHP:  strpos($s, "x");
来源：http://jqe.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gid.wangdashe.top

TS:   s.indexOf("x")
来源：http://vch.ybcxt.top

Java: s.indexOf("x")
来源：http://ltl.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://zra.chenlongwang.top

Ruby: s.index("x")
来源：http://caw.havefunace.top

C#:   s.IndexOf("x")
来源：http://dfl.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://svy.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bpo.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://psh.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://srm.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uca.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdk.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iit.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hrz.yvedp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cqa.hywenlv.cn

[E06] 替换子串
来源：http://glu.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sbs.meibo888.top

PHP:  str_replace("a", "b", $s);
来源：http://tnx.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uiw.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://lhc.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xda.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://igx.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cht.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://tns.jyoumei.cn

[E07] 按分隔符拆分
来源：http://aho.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iqc.jinqigfzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ror.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bwu.shanyushiyangtech.top

TS:   s.split(",")
来源：http://una.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://yjl.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://chm.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://lpg.guowangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sca.bjfxy.top

[E08] 数组按分隔符合并
来源：http://wns.zhengqikj.top

Py:   ",".join(items)
来源：http://zkp.tarul.cn

PHP:  implode(",", $items);
来源：http://ifi.yuanzhike.top

JS:   items.join(",")
来源：http://wrf.ppjwa.cn

TS:   items.join(",")
来源：http://gqy.jiagoushi.top

Java: String.join(",", items)
来源：http://ink.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://cfd.yvedp.cn

Ruby: items.join(",")
来源：http://ubn.daxiang520.top

C#:   string.Join(",", items)
来源：http://aww.316326.xyz

[E09] 去除所有空白字符
来源：http://jid.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xpk.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://keq.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://kmz.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://sbb.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://zur.birdmap.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tam.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://qid.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wgg.jyoumei.cn

[E10] 左侧补零 / 定长填充
来源：http://iui.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vyf.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zvk.ydzc1.top

JS:   "7".padStart(3, "0")
来源：http://ibj.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://dsu.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://nik.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qbg.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://acz.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cnj.fengsongda.top

[E11] 反转字符串
来源：http://bqg.xinyue.icu

Py:   s[::-1]
来源：http://syv.zdbjq.cn

PHP:  strrev($s);
来源：http://nlr.yueranfly.top

JS:   [...s].reverse().join("")
来源：http://adk.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://imx.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zui.zhoulong.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://czs.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://fjf.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mhj.hongshengwenyu.top

[E12] 统计某字符出现次数
来源：http://nvr.sufxvd.cn

Py:   s.count("a")
来源：http://ruf.hnqzz.top

PHP:  substr_count($s, "a");
来源：http://qhv.daria6918.cn

JS:   s.split("a").length - 1
来源：http://guf.yfazqb.com

TS:   s.split("a").length - 1
来源：http://uhu.vqdsnc.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rvh.yongpay.top

Go:   strings.Count(s, "a")
来源：http://ghw.shzxlz.cn

Ruby: s.count("a")
来源：http://ctx.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://xnd.yanxiufei.cn

[E13] 逐字符遍历
来源：http://wlt.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://hvk.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xfi.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kuq.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nzb.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jaf.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lja.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iky.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jgx.jianghu66.top

[E14] URL 编码与 Base64
来源：http://xkr.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zat.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gza.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zpo.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://abi.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://awo.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://spz.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lxl.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zrt.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://jkv.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tvv.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dfb.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qrd.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nhp.jqgufenzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aex.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gmk.yj20258888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yia.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://egu.wangdashe.top

[E16] 数字千分位
来源：http://nxh.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://cfz.xziqi.cn

PHP:  number_format(1234567);
来源：http://lqk.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://loc.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cnr.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hje.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ihl.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bcj.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://zom.zhoulong.xyz

[E17] 首字母大写
来源：http://fcr.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qrx.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://elw.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxj.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jcp.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://amj.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bxk.wangshuangyany.cn

Ruby: s.capitalize
来源：http://fpj.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hid.mhx1999.top

[E18] 模板占位符替换
来源：http://kcd.daria6918.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qgi.zhoulong.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ojy.yangfankeji.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jgh.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lvm.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ohi.tarul.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://unl.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zdu.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kct.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://ugy.guowangkeji.top

Py:   s.splitlines()
来源：http://dzt.ydzc1.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rxa.jlsjyb.cn

JS:   s.split(/\r?\n/)
来源：http://wpw.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://usa.kuanghao11.cn

Java: s.lines().toList()
来源：http://bst.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://lpr.dianchejie.cn

Ruby: s.lines
来源：http://ell.aizwys.cn

C#:   s.Split('\n')
来源：http://zgb.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://qwx.yanxiufei.cn

Py:   if not s:
来源：http://sgb.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yum.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zao.yfazqb.com

TS:   if (s === "") {}
来源：http://nne.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://oed.316326.xyz

Go:   if s == "" {}
来源：http://zty.gaohongyu789.top

Ruby: if s.empty?
来源：http://sjt.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otq.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://ysi.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mmu.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eoe.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kyy.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://psf.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sws.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://kve.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qyc.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wct.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://lly.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lvc.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nri.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bvz.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rrc.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xpi.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zql.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://gcl.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rxr.smart0.xyz

================================================================================
来源：http://wll.dashuyun.cn

F. 文件与目录
来源：http://mil.gogol.net.cn

================================================================================
来源：http://wnp.uphjek.com

[F01] 读取整个文件
来源：http://xnv.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://miz.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://znz.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qod.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mei.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jco.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tsb.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://peq.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://xez.yuxming.cn

[F02] 逐行读取文件
来源：http://ugx.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jdg.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://phc.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dun.hnqzz.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://egi.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vep.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ban.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cmb.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gsp.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://wjj.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yyj.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bey.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://boq.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oad.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jsr.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vpy.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://cks.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jar.gogol.net.cn

[F04] 追加写入文件
来源：http://ghx.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://esh.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vlo.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hkm.chenjidiqi.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ulr.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rhg.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jeq.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mvg.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mgt.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://ofy.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://syz.gaohongyu789.top

PHP:  file_exists("a.txt");
来源：http://npa.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://wtb.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://cdm.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gtb.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://syw.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://epb.birdmap.top

C#:   File.Exists("a.txt")
来源：http://nts.dashuyun.cn

[F06] 删除文件
来源：http://kqe.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://tbo.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://bsl.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cfd.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://cxk.zhongyouzk.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lur.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://qio.yangfankeji.com


<!-- 参考信息 -->