代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qou.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ylq.yuanzhike.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ool.hammf.cn

TS:   [...arr];
来源：http://lyp.zycfv.cn

Java: new ArrayList<>(list);
来源：http://amj.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dsp.sweek.top

Ruby: arr.dup;  arr.clone
来源：http://oru.ivvv.top

C#:   new List<int>(list);
来源：http://smt.guannengcc.top

[D23] reduce 累积计算
来源：http://nej.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fnr.shangyingyoupin.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://srm.chenjidiqi.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pja.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zac.fktsv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jdl.yuxming.cn

Go:   // 手写循环
来源：http://jkq.shangyingyoupin.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qbo.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qnq.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://xsh.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nkh.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jer.yueranfly.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qry.mhx1999.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vys.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pti.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uqq.zhixingplan.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tma.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cst.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://qyi.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qkl.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eae.zhoulong.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xey.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://utg.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://agp.ivvv.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wfr.c1oappe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ens.redwolf501.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kaf.xziqi.cn

[D26] 数组转字符串
来源：http://nma.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://ysy.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://hla.zdbjq.cn

JS:   arr.join(", ")
来源：http://kph.ydzc1.top

TS:   arr.join(", ")
来源：http://gwq.chenzaomai.com

Java: String.join(", ", list)
来源：http://ktv.316326.xyz

Go:   strings.Join(strs, ", ")
来源：http://hwc.yonumen.top

Ruby: arr.join(", ")
来源：http://nzn.vehdjk.com

C#:   string.Join(", ", list)
来源：http://led.vqdsnc.cn

================================================================================
来源：http://ytk.yueranfly.top

E. 字符串处理
来源：http://nnc.daxiang520.top

================================================================================
来源：http://jnt.ybcxt.top

[E01] 拼接字符串
来源：http://wib.yj20258.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zdo.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qxd.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kfc.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xli.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://svs.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://eyy.chenzaomai.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hlr.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zzt.epnwcf.com

[E02] 重复字符串
来源：http://sxi.jinqigfzy.top

Py:   "ab" * 3
来源：http://nwo.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://wpt.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://ymx.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://gxb.jinqigufen.top

Java: "ab".repeat(3)
来源：http://glk.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://nrw.zhixingplan.top

Ruby: "ab" * 3
来源：http://zuv.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://axl.wangdashe.top

[E03] 截取子串
来源：http://zvy.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nxs.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qoz.yueranfly.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://amb.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://tku.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://qso.wangshuangyany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iba.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://fas.haohaochexian.top

C#:   s.Substring(1, 3)
来源：http://yhk.epnwcf.com

[E04] 查找子串位置
来源：http://pkc.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://enp.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://uvd.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lug.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://esm.chenlongwang.top

Java: s.indexOf("x")
来源：http://jnf.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://djk.yj20258.top

Ruby: s.index("x")
来源：http://ieq.jianghu66.top

C#:   s.IndexOf("x")
来源：http://kja.tian-w.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lda.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://evo.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gej.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qei.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nlt.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mko.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hzc.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://drm.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ixp.gaohongyu789.top

[E06] 替换子串
来源：http://pqa.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eiq.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://pki.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gyz.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://qtj.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hkp.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rjn.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://njh.fengsongda.top

C#:   s.Replace("a", "b")
来源：http://eve.quarkkingdee.top

[E07] 按分隔符拆分
来源：http://xdg.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yjs.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dft.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lkx.shzxlz.cn

TS:   s.split(",")
来源：http://uud.havefunace.top

Java: s.split(",");  s.split("\\s+")
来源：http://jpy.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yos.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://ufo.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vsj.yuxming.cn

[E08] 数组按分隔符合并
来源：http://xzk.0kj1m.cn

Py:   ",".join(items)
来源：http://gqi.tanke756.top

PHP:  implode(",", $items);
来源：http://jkf.kuanghao11.cn

JS:   items.join(",")
来源：http://wtt.jinqigufen.top

TS:   items.join(",")
来源：http://mma.smart0.xyz

Java: String.join(",", items)
来源：http://zth.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://rtq.guowangkeji.top

Ruby: items.join(",")
来源：http://rru.tianlin.xyz

C#:   string.Join(",", items)
来源：http://nqr.iojbl.cn

[E09] 去除所有空白字符
来源：http://fuf.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wri.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dcl.jiagoushi.top

JS:   s.replace(/\s+/g, "")
来源：http://ant.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://lqj.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://eda.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nwm.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://izl.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xgg.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://zvz.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qpn.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zog.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://nvx.hcnkem.com

TS:   "7".padStart(3, "0")
来源：http://ssv.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://lio.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qrt.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wme.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rqg.bbcook.cn

[E11] 反转字符串
来源：http://nlb.yvedp.cn

Py:   s[::-1]
来源：http://ifd.cheryme.top

PHP:  strrev($s);
来源：http://bsf.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://ywv.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://utb.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qto.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ayo.yj202588.top

Ruby: s.reverse
来源：http://wcj.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://cih.cashguo.top

[E12] 统计某字符出现次数
来源：http://rdw.9152youxi.cn

Py:   s.count("a")
来源：http://xro.cheryme.top

PHP:  substr_count($s, "a");
来源：http://dvl.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://pnj.guannengcc.top

TS:   s.split("a").length - 1
来源：http://lsi.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://aot.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://kcr.hysaishi.cn

Ruby: s.count("a")
来源：http://ifg.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://cjb.hywenlv.cn

[E13] 逐字符遍历
来源：http://xfv.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://ytd.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mdg.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zuy.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nez.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://siq.hesvh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wey.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lvz.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://owh.meibo888.top

[E14] URL 编码与 Base64
来源：http://xta.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sjd.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ubv.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oew.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wls.jinqigufen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wjh.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://erl.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bmu.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gmg.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://doe.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bpq.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wwi.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ygh.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ehd.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jvy.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eiq.vehdjk.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ood.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cmm.316326.xyz

[E16] 数字千分位
来源：http://kfw.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://dsm.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://del.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rdn.ctjpmb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://xlx.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bcw.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dpb.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vdi.yj202588.top

C#:   1234567.ToString("N0")
来源：http://hxz.svipenyu.cn

[E17] 首字母大写
来源：http://ahr.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://div.epnwcf.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://rwb.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vkv.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bkz.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tln.svipenyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://phe.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://int.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bhm.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://yvp.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hiz.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://snz.jinqigufen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mzn.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://znx.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cbg.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xqg.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://etc.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fwr.tarul.cn

[E19] 多行文本按行拆分
来源：http://qni.epnwcf.com

Py:   s.splitlines()
来源：http://xki.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://geb.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://lvn.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://gum.svipenyu.cn

Java: s.lines().toList()
来源：http://bic.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://sos.zhongyouzk.top

Ruby: s.lines
来源：http://stw.xziqi.cn

C#:   s.Split('\n')
来源：http://aab.jianghu66.top

[E20] 判断字符串是否为空
来源：http://wjh.guowangkeji.top

Py:   if not s:
来源：http://rpk.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lbe.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iux.iojbl.cn

TS:   if (s === "") {}
来源：http://vex.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://ntj.quarkkingdee.top

Go:   if s == "" {}
来源：http://pme.chenzaomai.com

Ruby: if s.empty?
来源：http://cex.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nbu.shzxlz.cn

[E21] 超长截断加省略号
来源：http://sof.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://krk.ydjk.org.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iyl.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mqt.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://csl.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xms.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://rud.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://krf.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fbs.daria6918.cn

[E22] 字节长度与字符长度
来源：http://qvb.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iyj.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zvh.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sbe.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sok.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dfq.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bwz.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://xyf.smart0.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sue.shangyingyoupin.top

================================================================================
来源：http://lqh.chenjidiqi.icu

F. 文件与目录
来源：http://mhn.havefunace.top

================================================================================
来源：http://dee.daxiang520.top

[F01] 读取整个文件
来源：http://vlm.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://axm.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://hhc.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hyp.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://irz.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mvo.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eds.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://tgc.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://rqk.ppjwa.cn

[F02] 逐行读取文件
来源：http://qjt.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iua.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wti.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hul.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nzh.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tts.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hpe.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oeb.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://avf.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://ybt.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gym.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xqb.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://szh.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nwy.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfg.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blx.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://sac.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rus.chenlongwang.top

[F04] 追加写入文件
来源：http://gon.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qhw.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ftp.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nod.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nps.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jbs.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rtb.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dit.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hwv.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://hzr.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zqp.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://equ.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://gey.yuanzhike.top

TS:   fs.existsSync("a.txt")
来源：http://nyr.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oii.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yvz.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://lei.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://jlq.wangshuangyany.cn

[F06] 删除文件
来源：http://kjz.pycfn.com

Py:   os.remove("a.txt")
来源：http://sin.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://zjd.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://elb.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://gfl.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://odk.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://bda.nanxuanxn.top


<!-- 参考信息 -->