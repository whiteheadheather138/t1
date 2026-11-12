代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyg.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pap.fzhhl.top

Go:   // 手写循环
来源：http://qol.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zas.zhoulong.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lfn.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://xku.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jqo.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tvd.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dhv.ydzc1.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fwy.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pod.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oeq.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pwa.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rby.fanxiaobao.xyz

[D25] Set 集合去重与交并差
来源：http://xmn.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rxf.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qas.feifeiyinyue.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cqr.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xrk.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yzm.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rjz.gaohongyu789.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lpt.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ehe.daria6918.cn

[D26] 数组转字符串
来源：http://qgu.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://wns.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://azf.jianghu66.top

JS:   arr.join(", ")
来源：http://pnd.tanke756.top

TS:   arr.join(", ")
来源：http://vpf.pycfn.com

Java: String.join(", ", list)
来源：http://bja.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://xuy.meibo888.top

Ruby: arr.join(", ")
来源：http://oor.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://nrh.jyoumei.cn

================================================================================
来源：http://qdf.jinyuanbaomall.cn

E. 字符串处理
来源：http://hiy.zhijiandao.cn

================================================================================
来源：http://isp.ydjk.org.cn

[E01] 拼接字符串
来源：http://dmr.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://neu.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nii.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xje.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ehv.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pwf.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pvt.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zpu.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://syb.quarkkingdee.top

[E02] 重复字符串
来源：http://csw.yj20258.top

Py:   "ab" * 3
来源：http://qmr.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://wpj.hnxiangtu.top

JS:   "ab".repeat(3)
来源：http://ymg.pycfn.com

TS:   "ab".repeat(3)
来源：http://ydy.tanke756.top

Java: "ab".repeat(3)
来源：http://svp.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://dmp.tanke756.top

Ruby: "ab" * 3
来源：http://qua.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jsk.chenlongwang.top

[E03] 截取子串
来源：http://nyk.gogol.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxf.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://smy.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pda.shuidangran.top

TS:   s.slice(1, 4)
来源：http://fpc.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://wru.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tcn.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://leb.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://faq.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://dhm.zhixingplan.top

Py:   s.find("x");  s.index("x")
来源：http://ukm.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://wvd.zhaomingkeji.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iuy.chenzaomai.com

TS:   s.indexOf("x")
来源：http://jqg.andypj.xyz

Java: s.indexOf("x")
来源：http://vlh.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://gor.yonumen.top

Ruby: s.index("x")
来源：http://eps.nwbrower.top

C#:   s.IndexOf("x")
来源：http://ado.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://crc.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qmq.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zwx.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lig.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oiu.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rva.yuxming.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://noa.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jkg.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://shl.316326.xyz

[E06] 替换子串
来源：http://svr.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qjt.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://lfn.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zyg.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://hez.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aqq.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://boy.ehwqpu.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hel.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://psn.gogol.net.cn

[E07] 按分隔符拆分
来源：http://jqf.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xqh.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ygh.ppjwa.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bjm.hfpthk.cn

TS:   s.split(",")
来源：http://xka.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://qup.tianlin.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cis.hysaishi.cn

Ruby: s.split(",");  s.split
来源：http://nho.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mvg.zycfv.cn

[E08] 数组按分隔符合并
来源：http://jod.yfazqb.com

Py:   ",".join(items)
来源：http://sla.havefunace.top

PHP:  implode(",", $items);
来源：http://tjs.0kj1m.cn

JS:   items.join(",")
来源：http://hfm.hnqzz.top

TS:   items.join(",")
来源：http://vpu.ctjpmb.com

Java: String.join(",", items)
来源：http://mum.ctjpmb.com

Go:   strings.Join(items, ",")
来源：http://wpk.yongpay.top

Ruby: items.join(",")
来源：http://ekr.gogol.net.cn

C#:   string.Join(",", items)
来源：http://fgk.zhengqikj.top

[E09] 去除所有空白字符
来源：http://psi.ppjwa.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fya.havefunace.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zau.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://izu.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://cea.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://pee.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ftr.tianlin.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://hif.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jvb.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://rnr.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://liv.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iss.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://kun.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://uox.ehwqpu.com

Java: String.format("%03d", 7)
来源：http://hpk.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dit.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xcx.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ykw.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://sqp.yanxiufei.cn

Py:   s[::-1]
来源：http://cgv.yongpay.top

PHP:  strrev($s);
来源：http://nrx.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://vfn.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://crt.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://yop.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hdb.bbcook.cn

Ruby: s.reverse
来源：http://sjr.yongpay.top

C#:   new string(s.Reverse().ToArray())
来源：http://hqx.fehbvm.com

[E12] 统计某字符出现次数
来源：http://qfh.tarul.cn

Py:   s.count("a")
来源：http://htn.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://ejv.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://xmf.andypj.xyz

TS:   s.split("a").length - 1
来源：http://fuk.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wuf.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://cxq.chenzaomai.com

Ruby: s.count("a")
来源：http://icz.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://thw.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://nty.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://nmu.andypj.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mse.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iti.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xba.jianghu66.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://anr.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dij.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gpg.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://naw.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://ilh.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://plm.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ooz.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wea.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://umr.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sir.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nxm.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rip.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xks.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://tqy.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kfo.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jvf.ctjpmb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jai.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://mof.kuanghao11.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rpc.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mii.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fbo.jianghu66.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rxe.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://otf.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://nxx.jyoumei.cn

PHP:  number_format(1234567);
来源：http://yzc.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://liv.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mww.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dsy.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://shm.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aub.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://yon.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://gym.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://agg.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://xck.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bly.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://had.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://icf.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bjk.xuetiantiany.cn

Ruby: s.capitalize
来源：http://evb.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nry.ppjwa.cn

[E18] 模板占位符替换
来源：http://qwg.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kdh.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wba.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ynr.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rzn.cqqwz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nsh.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zzy.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gyb.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rbr.sjlbkw.cn

[E19] 多行文本按行拆分
来源：http://wun.ctjpmb.com

Py:   s.splitlines()
来源：http://mba.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fem.zdqjudy.top

JS:   s.split(/\r?\n/)
来源：http://jih.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://ean.wangdashe.top

Java: s.lines().toList()
来源：http://vmi.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://rsc.zhongyouzk.top

Ruby: s.lines
来源：http://xaj.316326.xyz

C#:   s.Split('\n')
来源：http://dki.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://bod.ehwqpu.com

Py:   if not s:
来源：http://kcm.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xtl.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vbf.0kj1m.cn

TS:   if (s === "") {}
来源：http://ozi.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://uxm.nanxinkj.top

Go:   if s == "" {}
来源：http://qkq.jqgfzy.top

Ruby: if s.empty?
来源：http://rhv.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://meo.uphjek.com

[E21] 超长截断加省略号
来源：http://ngk.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://one.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://spq.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zkv.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndk.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zsj.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://eak.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ruk.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lge.nwbrower.top

[E22] 字节长度与字符长度
来源：http://auv.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pys.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmu.hcnkem.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cji.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uxe.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gzj.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pff.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://ucw.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ezk.birdmap.top

================================================================================
来源：http://kte.zdqjudy.top

F. 文件与目录
来源：http://ave.gogol.net.cn

================================================================================
来源：http://tdp.snrcjt.cn

[F01] 读取整个文件
来源：http://tuo.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ucp.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://vdu.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://miz.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pul.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ozj.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ppg.redwolf501.top

Ruby: File.read("a.txt")
来源：http://cxt.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://xvs.zdbjq.cn

[F02] 逐行读取文件
来源：http://qsk.bbcook.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://imv.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uxz.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://umi.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://naz.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://smo.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hjd.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mbh.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lmd.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://psh.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jcu.fehbvm.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ewt.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fag.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tft.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://euk.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tri.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://kwg.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pev.zdqjudy.top

[F04] 追加写入文件
来源：http://xwn.zhixingplan.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nch.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ish.hesvh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wzl.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rrl.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://glp.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbb.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lfn.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ftb.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://ago.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rag.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://dje.tanke756.top

JS:   fs.existsSync("a.txt")
来源：http://qzo.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://eus.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://awm.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cyr.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://hkm.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://aja.zdqjudy.top

[F06] 删除文件
来源：http://lew.tarul.cn

Py:   os.remove("a.txt")
来源：http://upy.havefunace.top

PHP:  unlink("a.txt");
来源：http://btq.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://ccg.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://suh.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://out.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://oti.ydjk.org.cn

Ruby: File.delete("a.txt")
来源：http://yne.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://mlt.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://ghp.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iht.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vtd.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://akv.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cfj.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://edv.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://exd.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tmm.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fct.zhongyouzk.top

[F08] 遍历目录
来源：http://rww.daria6918.cn


<!-- 参考信息 -->