代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://vsa.jqgfzy.top

Ruby: arr.include?(x)
来源：http://ocu.zhengqikj.top

C#:   list.Contains(x)
来源：http://jvy.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://nlv.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gbb.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tjg.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oaj.cdnleiting.top

TS:   [...arr];
来源：http://qow.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://tte.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://fax.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://rbs.dashuyun.cn

C#:   new List<int>(list);
来源：http://ave.hesvh.cn

[D23] reduce 累积计算
来源：http://hbb.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dzz.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hwx.xingfuxueyuan.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kni.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vdh.sufxvd.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rim.shuidangran.top

Go:   // 手写循环
来源：http://hpo.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fac.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hyv.ybcxt.top

[D24] 字典 / Map 基本操作
来源：http://rmq.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qzx.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wcg.yj20258888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iys.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ary.316326.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wws.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ksu.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://daj.zhoulong.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hyb.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://lzr.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyt.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gmh.sjlbkw.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zgi.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xai.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bfq.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://btf.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyl.ywan-chungtsiang.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kjp.xylfe.cn

[D26] 数组转字符串
来源：http://wgr.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://keq.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://rnp.hammf.cn

JS:   arr.join(", ")
来源：http://gdv.hesvh.cn

TS:   arr.join(", ")
来源：http://sth.tanke756.top

Java: String.join(", ", list)
来源：http://lbu.bjfxy.top

Go:   strings.Join(strs, ", ")
来源：http://jol.yonumen.top

Ruby: arr.join(", ")
来源：http://bju.shanyushiyangtech.top

C#:   string.Join(", ", list)
来源：http://ksr.bjfxy.top

================================================================================
来源：http://ntc.smart0.xyz

E. 字符串处理
来源：http://thx.jiagoushi.top

================================================================================
来源：http://sgj.chenjidiqi.icu

[E01] 拼接字符串
来源：http://xcw.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pax.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uew.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pax.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pau.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hks.yvedp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tio.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://guq.pycfn.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pnw.zhixingplan.top

[E02] 重复字符串
来源：http://dul.0kj1m.cn

Py:   "ab" * 3
来源：http://lff.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://ady.yvedp.cn

JS:   "ab".repeat(3)
来源：http://pfo.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://xln.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://ymo.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://frp.andypj.xyz

Ruby: "ab" * 3
来源：http://sik.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oms.jiagoushi.top

[E03] 截取子串
来源：http://lqu.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uws.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xjz.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cpy.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://asz.snrcjt.cn

Java: s.substring(1, 4)
来源：http://gwk.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://otj.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cnk.chenzaomai.com

C#:   s.Substring(1, 3)
来源：http://khy.hysaishi.cn

[E04] 查找子串位置
来源：http://mra.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://nkn.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://qrd.cucudq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qfq.ybcxt.top

TS:   s.indexOf("x")
来源：http://swv.zhijiandao.cn

Java: s.indexOf("x")
来源：http://gar.meibo888.top

Go:   strings.Index(s, "x")
来源：http://vik.zhiwuduotai.top

Ruby: s.index("x")
来源：http://fhb.aizwys.cn

C#:   s.IndexOf("x")
来源：http://vaq.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijz.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://idf.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wgy.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lhd.yj202588.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://isi.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://adm.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kyx.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jja.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yem.nanxuanxn.top

[E06] 替换子串
来源：http://dxu.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zkb.shanyushiyangkeji.top

PHP:  str_replace("a", "b", $s);
来源：http://srs.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dke.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://ifr.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zkv.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aad.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bel.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://srm.cqqwz.cn

[E07] 按分隔符拆分
来源：http://yed.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qox.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://roz.hammf.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://isp.nanxuanxn.top

TS:   s.split(",")
来源：http://oed.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://tsi.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pcg.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://wpc.hfpthk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://emm.uphjek.com

[E08] 数组按分隔符合并
来源：http://pyd.jyoumei.cn

Py:   ",".join(items)
来源：http://smy.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://zhv.zhiwuduotai.top

JS:   items.join(",")
来源：http://pmn.zycfv.cn

TS:   items.join(",")
来源：http://dcf.hnxiangtu.top

Java: String.join(",", items)
来源：http://fqd.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://sgw.havefunace.top

Ruby: items.join(",")
来源：http://vcz.zhengqikj.top

C#:   string.Join(",", items)
来源：http://wiz.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://gma.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kek.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nxs.kuanghao11.cn

JS:   s.replace(/\s+/g, "")
来源：http://jtl.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://xod.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://exo.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ffy.tian-w.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ssj.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xhz.hnxiangtu.top

[E10] 左侧补零 / 定长填充
来源：http://smf.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://icl.pengpengdd.cyou

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wnf.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://psw.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://wwb.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://vrk.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ywk.yanxiufei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iwo.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tin.epnwcf.com

[E11] 反转字符串
来源：http://ltr.fehbvm.com

Py:   s[::-1]
来源：http://plf.yj20258.top

PHP:  strrev($s);
来源：http://rjp.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://nar.ctjpmb.com

TS:   [...s].reverse().join("")
来源：http://fmz.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hpa.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://eyt.mhx1999.top

Ruby: s.reverse
来源：http://vxm.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://raw.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://cdp.zhiwuduotai.top

Py:   s.count("a")
来源：http://vnt.hammf.cn

PHP:  substr_count($s, "a");
来源：http://tbg.hcnkem.com

JS:   s.split("a").length - 1
来源：http://ihm.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://evj.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vnk.ppjwa.cn

Go:   strings.Count(s, "a")
来源：http://gsq.ehwqpu.com

Ruby: s.count("a")
来源：http://uyl.ehwqpu.com

C#:   s.Count(c => c == 'a')
来源：http://gek.mhx1999.top

[E13] 逐字符遍历
来源：http://zse.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://gsi.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fzd.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ifd.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ixz.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://beo.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wil.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://eoa.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xqu.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://lbj.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pct.yangfankeji.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://tgj.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://msp.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://axx.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://aer.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jxo.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://twh.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zvl.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://lkc.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://qgp.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://msz.andypj.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mes.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iyf.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cyo.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lvi.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jgx.hfpthk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qat.daria6918.cn

[E16] 数字千分位
来源：http://vrn.52xcode.cn

Py:   f"{1234567:,}"
来源：http://uhw.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://hwv.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hkb.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mlk.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fud.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hgr.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vge.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://jzj.bjfxy.top

[E17] 首字母大写
来源：http://ljt.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zkd.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tzj.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gro.dianchejie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qdu.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vam.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tyr.hfpthk.cn

Ruby: s.capitalize
来源：http://kjy.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bun.ydzc1.top

[E18] 模板占位符替换
来源：http://qeq.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wlo.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mao.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://moh.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vqk.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mlu.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uud.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ava.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hyl.bbcook.cn

[E19] 多行文本按行拆分
来源：http://nqo.tianlin.xyz

Py:   s.splitlines()
来源：http://btu.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qlt.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://yua.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://ize.cucudq.cn

Java: s.lines().toList()
来源：http://phi.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://whh.epnwcf.com

Ruby: s.lines
来源：http://qpb.dianchejie.cn

C#:   s.Split('\n')
来源：http://hkj.daria6918.cn

[E20] 判断字符串是否为空
来源：http://qeo.redwolf501.top

Py:   if not s:
来源：http://osh.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nss.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xzf.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://eau.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://qna.tanke756.top

Go:   if s == "" {}
来源：http://qfv.fengsongda.top

Ruby: if s.empty?
来源：http://kxz.guannengcc.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fnc.bjfxy.top

[E21] 超长截断加省略号
来源：http://lag.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cla.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xkj.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bmc.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yxa.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rxn.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://ics.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oah.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qbq.svipenyu.cn

[E22] 字节长度与字符长度
来源：http://siu.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ega.pycfn.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://shf.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ttl.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lyb.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zsb.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://alg.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://pqb.vqdsnc.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pzs.nanxinkj.top

================================================================================
来源：http://nwq.snrcjt.cn

F. 文件与目录
来源：http://rnb.zhixingplan.top

================================================================================
来源：http://eto.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://qmj.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://psw.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://ahx.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://onc.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lwy.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vga.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lwd.nwbrower.top

Ruby: File.read("a.txt")
来源：http://uku.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://ugy.birdmap.top

[F02] 逐行读取文件
来源：http://fcq.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lwj.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mtc.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://emr.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grw.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://srw.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cfs.zhixingplan.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tyx.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nzg.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://bxt.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oks.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hsm.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ukb.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ddb.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wzz.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sdm.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://jyo.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://arf.redwolf501.top

[F04] 追加写入文件
来源：http://rdv.yongpay.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bwk.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lyv.gotoacloud.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvq.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tzg.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://efp.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jdc.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fmf.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dwd.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://agt.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aai.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://wko.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://mra.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://hxx.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zrr.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://avb.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://fam.ivvv.top

C#:   File.Exists("a.txt")
来源：http://uom.ivvv.top

[F06] 删除文件
来源：http://nnt.epnwcf.com

Py:   os.remove("a.txt")
来源：http://yue.daria6918.cn

PHP:  unlink("a.txt");
来源：http://mzi.hfpthk.cn


<!-- 参考信息 -->