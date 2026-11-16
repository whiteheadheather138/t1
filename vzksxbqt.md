代发 wailian999

[D23] reduce 累积计算
来源：http://wsa.dashuyun.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://boa.hysaishi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vbl.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nfu.pycfn.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otj.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://wwb.yvedp.cn

Go:   // 手写循环
来源：http://lws.chenzaomai.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fej.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nnl.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://bkv.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mnq.ydzc1.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rnd.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nyw.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://upl.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xgu.feifeiyinyue.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://usz.redwolf501.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vcu.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://enf.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://geu.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xhk.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nxw.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uuf.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ijl.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ihc.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ahq.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://axg.hfpthk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rgm.hammf.cn

[D26] 数组转字符串
来源：http://czj.nanxuanxn.top

Py:   ", ".join(map(str, arr))
来源：http://fsv.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://fss.yj20258888.top

JS:   arr.join(", ")
来源：http://lna.c1oappe.top

TS:   arr.join(", ")
来源：http://bfk.yuanzhike.top

Java: String.join(", ", list)
来源：http://qtj.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://yqo.ydzc1.top

Ruby: arr.join(", ")
来源：http://lfn.pengpengdd.cyou

C#:   string.Join(", ", list)
来源：http://eko.hnqzz.top

================================================================================
来源：http://xtw.zhengqikj.top

E. 字符串处理
来源：http://vvz.hywenlv.cn

================================================================================
来源：http://mfs.zhiwuduotai.top

[E01] 拼接字符串
来源：http://lhp.guowangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qsf.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lro.yj20258.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qwe.fehbvm.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://prq.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fvr.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wky.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xza.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qrs.guowangkeji.top

[E02] 重复字符串
来源：http://zin.zdbjq.cn

Py:   "ab" * 3
来源：http://vou.tarul.cn

PHP:  str_repeat("ab", 3);
来源：http://ofv.tian-w.cn

JS:   "ab".repeat(3)
来源：http://shi.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://lzz.zhongyouzk.top

Java: "ab".repeat(3)
来源：http://wkx.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://ylu.0kj1m.cn

Ruby: "ab" * 3
来源：http://yjb.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ize.vehdjk.com

[E03] 截取子串
来源：http://dye.vehdjk.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ltm.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ock.bbcook.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mlr.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://jsz.daria6918.cn

Java: s.substring(1, 4)
来源：http://vze.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bhs.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yrz.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://rmf.jinqigufen.top

[E04] 查找子串位置
来源：http://phv.jyoumei.cn

Py:   s.find("x");  s.index("x")
来源：http://kcv.wangdashe.top

PHP:  strpos($s, "x");
来源：http://swt.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://onm.epnwcf.com

TS:   s.indexOf("x")
来源：http://xvd.xylfe.cn

Java: s.indexOf("x")
来源：http://ukj.iojbl.cn

Go:   strings.Index(s, "x")
来源：http://ntb.ivvv.top

Ruby: s.index("x")
来源：http://asb.tarul.cn

C#:   s.IndexOf("x")
来源：http://ktm.cucudq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://wuh.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qma.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://scn.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yra.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lbh.kuanghao11.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://twn.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jtf.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aht.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hbg.jinqigufen.top

[E06] 替换子串
来源：http://gsu.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ree.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://gwr.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lqe.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://nkj.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lhc.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kqr.cdnleiting.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gqv.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://kdr.ydzc1.top

[E07] 按分隔符拆分
来源：http://wcc.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ibe.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kzi.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://wko.hongshengwenyu.top

TS:   s.split(",")
来源：http://wwe.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://cbf.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kiv.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://tjd.ppjwa.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ehu.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://iuh.jinyuanbaomall.cn

Py:   ",".join(items)
来源：http://bri.bbcook.cn

PHP:  implode(",", $items);
来源：http://aej.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://fba.nanxuanxn.top

TS:   items.join(",")
来源：http://vhc.hnxiangtu.top

Java: String.join(",", items)
来源：http://hdx.chenlongwang.top

Go:   strings.Join(items, ",")
来源：http://jwu.iojbl.cn

Ruby: items.join(",")
来源：http://kuc.zycfv.cn

C#:   string.Join(",", items)
来源：http://iub.aibaodan.cn

[E09] 去除所有空白字符
来源：http://ddz.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jiy.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hgd.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://kko.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://nxu.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://rhm.xingfuxueyuan.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://nml.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://hmn.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hel.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://gtl.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vtv.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uvt.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://zsz.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://bnl.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://yzl.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://axc.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kwb.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bnl.zycfv.cn

[E11] 反转字符串
来源：http://hae.zdqjudy.top

Py:   s[::-1]
来源：http://etd.zhongyouzk.top

PHP:  strrev($s);
来源：http://zol.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://aiy.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://ngi.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://blb.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rbq.hnqzz.top

Ruby: s.reverse
来源：http://wiu.mhx1999.top

C#:   new string(s.Reverse().ToArray())
来源：http://kqz.yonumen.top

[E12] 统计某字符出现次数
来源：http://qlz.nanxuanxn.top

Py:   s.count("a")
来源：http://eek.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://qfy.sxryk.cn

JS:   s.split("a").length - 1
来源：http://vif.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://cpx.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cac.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://hwz.guowangkeji.top

Ruby: s.count("a")
来源：http://rkp.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://tco.zdqjudy.top

[E13] 逐字符遍历
来源：http://lzk.tanke756.top

Py:   for ch in s: print(ch)
来源：http://opt.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://juk.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tnw.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sdb.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ofj.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bfh.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zuj.snrcjt.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sxh.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://vmz.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ckz.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://syr.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uwj.jqgfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://phg.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uku.yvedp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rnh.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cog.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lxx.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://ruz.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nvx.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jij.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://daj.yonumen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mfx.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wso.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mwp.ppjwa.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vjq.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://koq.zhoulong.xyz

[E16] 数字千分位
来源：http://zcv.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://dtl.epnwcf.com

PHP:  number_format(1234567);
来源：http://bqy.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vps.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://wpk.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mqz.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mdp.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hrf.ctjpmb.com

C#:   1234567.ToString("N0")
来源：http://drb.nanxinkj.top

[E17] 首字母大写
来源：http://rpd.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zyg.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://bfv.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wbn.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nix.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qxs.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sub.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://czc.gaohongyu789.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mwo.tian-w.cn

[E18] 模板占位符替换
来源：http://los.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zse.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ucv.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tjj.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ayv.guannengcc.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dqf.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sgu.ydjk.org.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cfq.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://flh.fzhhl.top

[E19] 多行文本按行拆分
来源：http://pkv.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://xmy.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kcp.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://awz.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://tli.ywan-chungtsiang.top

Java: s.lines().toList()
来源：http://zyk.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://byr.yj202588.top

Ruby: s.lines
来源：http://klj.quarkkingdee.top

C#:   s.Split('\n')
来源：http://eas.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://mia.ctjpmb.com

Py:   if not s:
来源：http://dqs.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dpu.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mtc.meibo888.top

TS:   if (s === "") {}
来源：http://vyg.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://ouw.iojbl.cn

Go:   if s == "" {}
来源：http://agk.jqgfzy.top

Ruby: if s.empty?
来源：http://brx.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zdw.ydzc1.top

[E21] 超长截断加省略号
来源：http://ive.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wqh.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wgs.fanxiaobao.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vbi.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dfz.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wum.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://fxz.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qdn.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnz.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://qso.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://owx.zdbjq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://haf.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xzu.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ycb.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pau.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://opb.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://vue.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tcu.mhx1999.top

================================================================================
来源：http://pdp.fanxiaobao.xyz

F. 文件与目录
来源：http://gsh.cucudq.cn

================================================================================
来源：http://hic.mhx1999.top

[F01] 读取整个文件
来源：http://efy.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://urq.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://tib.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vys.hywenlv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rkn.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://hmp.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wvt.guannengcc.top

Ruby: File.read("a.txt")
来源：http://ctb.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://gsf.fktsv.cn

[F02] 逐行读取文件
来源：http://wml.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cqh.guannengcc.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://koa.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://khz.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mcf.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kqs.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pcn.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zqw.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yhj.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://vjx.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rbn.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nho.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eyv.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mng.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://emz.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qwy.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://lzf.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://khh.xuetiantiany.cn

[F04] 追加写入文件
来源：http://rar.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iae.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xjn.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ahf.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aiq.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bwn.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://twy.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://syc.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jbn.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://gqq.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tqh.yonumen.top

PHP:  file_exists("a.txt");
来源：http://dvy.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://kmi.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://edq.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://wej.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://djh.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://ymm.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://sqx.hysaishi.cn

[F06] 删除文件
来源：http://svw.ivvv.top

Py:   os.remove("a.txt")
来源：http://hxd.guannengcc.top

PHP:  unlink("a.txt");
来源：http://sba.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://nfs.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://jld.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://inx.tarul.cn

Go:   os.Remove("a.txt")
来源：http://gar.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://bpl.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://aqm.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://sme.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xko.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nxi.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mzw.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqd.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://may.xuetiantiany.cn


<!-- 参考信息 -->