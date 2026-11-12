代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://upq.zhoulong.xyz

[D20] 统计每个元素出现次数
来源：http://erx.zhiwuduotai.top

Py:   Counter(arr)
来源：http://meq.ybcxt.top

PHP:  array_count_values($arr);
来源：http://arm.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwh.nwbrower.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://syr.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://npp.iojbl.cn

Go:   // 手写 map[T]int
来源：http://exx.zhongyouzk.top

Ruby: arr.tally
来源：http://lxy.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ntm.vehdjk.com

[D21] 判断是否包含某元素
来源：http://zhi.yj202588.top

Py:   x in arr
来源：http://nft.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://eqs.nanxinkj.top

JS:   arr.includes(x)
来源：http://rsk.yfazqb.com

TS:   arr.includes(x)
来源：http://ylh.hammf.cn

Java: list.contains(x)
来源：http://lme.nanxuanxn.top

Go:   slices.Contains(arr, x)
来源：http://zfk.jinqigufen.top

Ruby: arr.include?(x)
来源：http://pjx.shanyushiyangkeji.top

C#:   list.Contains(x)
来源：http://sph.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://lxq.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bij.xuetiantiany.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mez.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zkk.yvedp.cn

TS:   [...arr];
来源：http://jns.redwolf501.top

Java: new ArrayList<>(list);
来源：http://hkk.yuanzhike.top

Go:   copied := append([]int(nil), arr...)
来源：http://vnp.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://amc.xylfe.cn

C#:   new List<int>(list);
来源：http://aem.shzxlz.cn

[D23] reduce 累积计算
来源：http://fvt.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://col.hammf.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yoe.jianghu66.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lhy.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tzw.vehdjk.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://oat.hcnkem.com

Go:   // 手写循环
来源：http://upa.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ikb.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fjn.ivvv.top

[D24] 字典 / Map 基本操作
来源：http://jjr.hywenlv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qes.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ddv.pycfn.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wel.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://azc.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xfo.redwolf501.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hhn.yongpay.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fbr.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pjp.mhx1999.top

[D25] Set 集合去重与交并差
来源：http://zck.jinyuanbaomall.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kgi.sjlbkw.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://otx.nanxinkj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eod.dashuyun.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gja.hesvh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dem.yfazqb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hwq.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pjk.zhiwuduotai.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nsc.yj202588.top

[D26] 数组转字符串
来源：http://wec.fzhhl.top

Py:   ", ".join(map(str, arr))
来源：http://mwa.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://xvt.yongpay.top

JS:   arr.join(", ")
来源：http://mrm.vqdsnc.cn

TS:   arr.join(", ")
来源：http://qrb.dashuyun.cn

Java: String.join(", ", list)
来源：http://ois.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://xiz.9152youxi.cn

Ruby: arr.join(", ")
来源：http://qwt.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://wlr.tanke756.top

================================================================================
来源：http://yiy.tanke756.top

E. 字符串处理
来源：http://yyy.yj20258888.top

================================================================================
来源：http://pwg.cdnleiting.top

[E01] 拼接字符串
来源：http://vbw.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eof.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oxp.chenzaomai.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zmb.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://khr.shangyingyoupin.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hqw.yj20258.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qht.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eaf.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bof.xziqi.cn

[E02] 重复字符串
来源：http://nia.smart0.xyz

Py:   "ab" * 3
来源：http://rqe.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://sjy.ybcxt.top

JS:   "ab".repeat(3)
来源：http://vji.fzhhl.top

TS:   "ab".repeat(3)
来源：http://ypk.shzxlz.cn

Java: "ab".repeat(3)
来源：http://xpc.chenzaomai.com

Go:   strings.Repeat("ab", 3)
来源：http://fny.0kj1m.cn

Ruby: "ab" * 3
来源：http://znk.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dhs.tian-w.cn

[E03] 截取子串
来源：http://tyn.yanxiufei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hdb.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hex.jiagoushi.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://svr.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://yyi.chenlongwang.top

Java: s.substring(1, 4)
来源：http://kjm.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tgk.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://rdd.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://iet.daria6918.cn

[E04] 查找子串位置
来源：http://aor.snrcjt.cn

Py:   s.find("x");  s.index("x")
来源：http://xtx.svipenyu.cn

PHP:  strpos($s, "x");
来源：http://lmb.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yqo.fktsv.cn

TS:   s.indexOf("x")
来源：http://qpo.pycfn.com

Java: s.indexOf("x")
来源：http://yts.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://bxw.zhixingplan.top

Ruby: s.index("x")
来源：http://job.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://mnz.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://omq.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wgt.ctjpmb.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uxg.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qii.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vlo.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nuj.cucudq.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zdf.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uow.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://efz.dashuyun.cn

[E06] 替换子串
来源：http://ige.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ofe.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://rjx.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xon.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://kxw.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uji.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://noj.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hbk.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://gzn.smart0.xyz

[E07] 按分隔符拆分
来源：http://wqq.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ffx.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rwr.hongshengwenyu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://aow.jiagoushi.top

TS:   s.split(",")
来源：http://rum.sysykeji.top

Java: s.split(",");  s.split("\\s+")
来源：http://hlh.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://awv.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://nke.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zdl.sweek.top

[E08] 数组按分隔符合并
来源：http://uzh.redwolf501.top

Py:   ",".join(items)
来源：http://icq.hcnkem.com

PHP:  implode(",", $items);
来源：http://nxr.xylfe.cn

JS:   items.join(",")
来源：http://opq.daxiang520.top

TS:   items.join(",")
来源：http://osf.cucudq.cn

Java: String.join(",", items)
来源：http://njd.havefunace.top

Go:   strings.Join(items, ",")
来源：http://qoo.yfazqb.com

Ruby: items.join(",")
来源：http://ibt.zdbjq.cn

C#:   string.Join(",", items)
来源：http://jaw.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://zhx.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rie.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gwv.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://fua.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://yot.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://gqk.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wsy.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://hpt.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bze.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://bpa.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gmw.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mnf.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://ugw.yuxming.cn

TS:   "7".padStart(3, "0")
来源：http://njb.smart0.xyz

Java: String.format("%03d", 7)
来源：http://wiv.svipenyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cps.yj202588.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://njv.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zqs.iojbl.cn

[E11] 反转字符串
来源：http://sjn.gzhubu.top

Py:   s[::-1]
来源：http://wly.hnxiangtu.top

PHP:  strrev($s);
来源：http://fqs.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://omy.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://gjg.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://unm.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kzf.gotoacloud.top

Ruby: s.reverse
来源：http://eoj.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://uuz.c1oappe.top

[E12] 统计某字符出现次数
来源：http://nen.gogol.net.cn

Py:   s.count("a")
来源：http://wzm.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://vbt.vehdjk.com

JS:   s.split("a").length - 1
来源：http://kva.gzhubu.top

TS:   s.split("a").length - 1
来源：http://nrg.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nfu.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://taa.cashguo.top

Ruby: s.count("a")
来源：http://rem.shanyushiyangtech.top

C#:   s.Count(c => c == 'a')
来源：http://ruk.ehwqpu.com

[E13] 逐字符遍历
来源：http://ttf.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://cuf.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://azu.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iln.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://uun.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kvi.ydzc1.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tkm.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kgr.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://afy.sxryk.cn

[E14] URL 编码与 Base64
来源：http://wxi.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sze.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rkw.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rou.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gpo.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jyf.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ssy.ydzc1.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://myx.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xvn.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://sox.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bwh.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://khf.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://abi.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ywk.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yal.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://agl.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwq.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oub.sufxvd.cn

[E16] 数字千分位
来源：http://gkp.guannengcc.top

Py:   f"{1234567:,}"
来源：http://daz.birdmap.top

PHP:  number_format(1234567);
来源：http://sdv.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://alb.ydzc1.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dcw.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nes.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mdw.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cvz.smart0.xyz

C#:   1234567.ToString("N0")
来源：http://uen.hesvh.cn

[E17] 首字母大写
来源：http://aal.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sbd.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qjx.zhengqikj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rjq.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zun.sufxvd.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://crq.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://btb.fengsongda.top

Ruby: s.capitalize
来源：http://ecd.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://anp.hysaishi.cn

[E18] 模板占位符替换
来源：http://dej.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pjx.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://umw.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pma.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rum.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ixg.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ycy.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baa.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://keo.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://fih.gogol.net.cn

Py:   s.splitlines()
来源：http://kxp.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mne.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://cvn.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://zij.cucudq.cn

Java: s.lines().toList()
来源：http://jvx.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://hez.fehbvm.com

Ruby: s.lines
来源：http://frn.shuidangran.top

C#:   s.Split('\n')
来源：http://usk.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://jag.cashguo.top

Py:   if not s:
来源：http://vrb.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aac.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hyk.nanxinkj.top

TS:   if (s === "") {}
来源：http://foy.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://glg.aibaodan.cn

Go:   if s == "" {}
来源：http://oko.smart0.xyz

Ruby: if s.empty?
来源：http://lcf.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tuz.yongpay.top

[E21] 超长截断加省略号
来源：http://bvs.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fap.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://srg.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owz.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihg.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pqh.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://xju.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xmn.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://efq.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://tzq.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ggy.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://swi.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://def.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gng.chenlongwang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vhz.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xph.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://udu.hcnkem.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jck.cucudq.cn

================================================================================
来源：http://and.hcnkem.com

F. 文件与目录
来源：http://ebd.yvedp.cn

================================================================================
来源：http://zpz.sweek.top

[F01] 读取整个文件
来源：http://sec.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bpy.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://mkx.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zjz.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yft.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rpl.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rrl.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://tmy.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://arf.hammf.cn

[F02] 逐行读取文件
来源：http://imd.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jwt.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lxv.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sou.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mow.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gvb.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qqo.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kkq.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hhd.ydjk.org.cn

[F03] 写入文件（覆盖）
来源：http://hbj.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wal.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xna.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qlm.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lus.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fin.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jdc.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://tyl.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xwd.yangfankeji.com

[F04] 追加写入文件
来源：http://iye.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ett.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ceb.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqj.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzh.xingfuxueyuan.xyz


<!-- 参考信息 -->