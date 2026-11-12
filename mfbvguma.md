代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tws.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oeq.shanyushiyangkeji.top

Go:   // 手写循环
来源：http://zmm.yj202588.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://msl.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ose.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://ubq.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jzf.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kwa.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xrk.vqdsnc.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://npe.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kec.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uhf.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dsg.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xan.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://zub.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iko.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jjy.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tmg.chenlongwang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wzz.daxiang520.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://srg.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mxx.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://plc.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iuk.jlsjyb.cn

[D26] 数组转字符串
来源：http://dqt.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://rhp.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://wkq.gotoacloud.top

JS:   arr.join(", ")
来源：http://ylk.tian-w.cn

TS:   arr.join(", ")
来源：http://zzp.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://maw.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://pzk.hesvh.cn

Ruby: arr.join(", ")
来源：http://coa.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://tix.fehbvm.com

================================================================================
来源：http://xvc.guowangkeji.top

E. 字符串处理
来源：http://iwk.xuetiantiany.cn

================================================================================
来源：http://qnk.sweek.top

[E01] 拼接字符串
来源：http://ahh.fzhhl.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qio.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mqt.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gen.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxd.zhongyouzk.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://snr.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nfh.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xja.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rsq.fzhhl.top

[E02] 重复字符串
来源：http://tbh.ehwqpu.com

Py:   "ab" * 3
来源：http://tsj.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://edc.nanxuanxn.top

JS:   "ab".repeat(3)
来源：http://kpu.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://sig.snrcjt.cn

Java: "ab".repeat(3)
来源：http://hyl.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://wdb.fengsongda.top

Ruby: "ab" * 3
来源：http://rst.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qmz.iojbl.cn

[E03] 截取子串
来源：http://odp.sxryk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wll.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yvq.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jos.yvedp.cn

TS:   s.slice(1, 4)
来源：http://ulq.xylfe.cn

Java: s.substring(1, 4)
来源：http://pqa.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iur.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://vfx.vehdjk.com

C#:   s.Substring(1, 3)
来源：http://efy.jianghu66.top

[E04] 查找子串位置
来源：http://ucp.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://ena.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://pas.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wjy.sweek.top

TS:   s.indexOf("x")
来源：http://ipu.aizwys.cn

Java: s.indexOf("x")
来源：http://njw.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://soo.smart0.xyz

Ruby: s.index("x")
来源：http://hjt.gogol.net.cn

C#:   s.IndexOf("x")
来源：http://von.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ivk.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dik.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ujk.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rki.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ioh.fanxiaobao.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fck.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gni.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pxe.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cci.jqgufenzy.top

[E06] 替换子串
来源：http://rzn.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kgf.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://keg.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahj.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://don.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uzm.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jzy.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://okx.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://nqk.316326.xyz

[E07] 按分隔符拆分
来源：http://sad.sufxvd.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nkj.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ygo.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lvy.redwolf501.top

TS:   s.split(",")
来源：http://esw.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://uil.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iju.tarul.cn

Ruby: s.split(",");  s.split
来源：http://rjo.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iwn.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://rax.jinqigufen.top

Py:   ",".join(items)
来源：http://hns.sweek.top

PHP:  implode(",", $items);
来源：http://qhj.jinghuilouyu.cn

JS:   items.join(",")
来源：http://oyp.jqgfzy.top

TS:   items.join(",")
来源：http://fnt.feifeiyinyue.top

Java: String.join(",", items)
来源：http://bvx.yonumen.top

Go:   strings.Join(items, ",")
来源：http://ewp.hesvh.cn

Ruby: items.join(",")
来源：http://rxu.tianlin.xyz

C#:   string.Join(",", items)
来源：http://tpl.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://miw.chenjidiqi.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fhn.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://szo.yuxming.cn

JS:   s.replace(/\s+/g, "")
来源：http://qrg.gotoacloud.top

TS:   s.replace(/\s+/g, "")
来源：http://yiz.yonumen.top

Java: s.replaceAll("\\s+", "")
来源：http://dtt.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://urq.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://ely.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wwv.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://lgg.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dzp.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dvv.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://xfj.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://acn.yangfankeji.com

Java: String.format("%03d", 7)
来源：http://vro.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://aun.gotoacloud.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sde.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pwq.daria6918.cn

[E11] 反转字符串
来源：http://fpr.yongpay.top

Py:   s[::-1]
来源：http://cdn.gzhubu.top

PHP:  strrev($s);
来源：http://pud.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://wcw.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://xis.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nab.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tkv.quarkkingdee.top

Ruby: s.reverse
来源：http://ewh.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ksp.bjfxy.top

[E12] 统计某字符出现次数
来源：http://mpb.aibaodan.cn

Py:   s.count("a")
来源：http://yeq.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://jbb.yueranfly.top

JS:   s.split("a").length - 1
来源：http://wum.fktsv.cn

TS:   s.split("a").length - 1
来源：http://een.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://exi.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://coc.sxryk.cn

Ruby: s.count("a")
来源：http://uvr.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://mlw.tianlin.xyz

[E13] 逐字符遍历
来源：http://zdc.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://rcn.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kxf.hammf.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cir.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nuu.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pmm.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wzu.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zjy.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wcb.smart0.xyz

[E14] URL 编码与 Base64
来源：http://nvf.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://atu.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://uoe.jinqigfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wyl.daxiang520.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jfy.mhx1999.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://own.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lvf.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://owp.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://she.zhiwuduotai.top

[E15] HTML 转义 / 反转义
来源：http://knz.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yak.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zbr.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hsu.zdbjq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yek.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kdo.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://scu.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://obo.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ohi.cqqwz.cn

[E16] 数字千分位
来源：http://agl.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://lim.yfazqb.com

PHP:  number_format(1234567);
来源：http://rli.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dcj.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lwh.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://emw.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://owg.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gkk.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://ods.birdmap.top

[E17] 首字母大写
来源：http://uxw.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ghh.jqgfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ahc.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://knf.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lrx.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yte.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ddy.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://tld.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nlp.gotoacloud.top

[E18] 模板占位符替换
来源：http://rdk.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aol.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cwj.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://jiv.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rer.fehbvm.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://avg.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qcv.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ofe.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ejv.andypj.xyz

[E19] 多行文本按行拆分
来源：http://pen.kuanghao11.cn

Py:   s.splitlines()
来源：http://tei.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ilc.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://mbx.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://rrz.shuidangran.top

Java: s.lines().toList()
来源：http://cqw.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://ely.feifeiyinyue.top

Ruby: s.lines
来源：http://eau.dianchejie.cn

C#:   s.Split('\n')
来源：http://dyt.havefunace.top

[E20] 判断字符串是否为空
来源：http://npu.hammf.cn

Py:   if not s:
来源：http://mad.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://abm.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cex.hongshengwenyu.top

TS:   if (s === "") {}
来源：http://jmr.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://efi.xylfe.cn

Go:   if s == "" {}
来源：http://lqr.xuetiantiany.cn

Ruby: if s.empty?
来源：http://bik.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jjp.zycfv.cn

[E21] 超长截断加省略号
来源：http://ass.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zkp.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bro.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oxm.shzxlz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cmc.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://flj.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://gtl.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lqb.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zgj.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://xna.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qsj.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hkj.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzw.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ubh.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vzo.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xeu.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://ivi.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kok.pengpengdd.cyou

================================================================================
来源：http://sjh.ywan-chungtsiang.top

F. 文件与目录
来源：http://hec.yj20258.top

================================================================================
来源：http://mvc.sjlbkw.cn

[F01] 读取整个文件
来源：http://wpt.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ulu.jinghuilouyu.cn

PHP:  file_get_contents("a.txt");
来源：http://auw.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cpn.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qze.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oox.zhijiandao.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kym.aizwys.cn

Ruby: File.read("a.txt")
来源：http://pva.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://ioq.ybcxt.top

[F02] 逐行读取文件
来源：http://nwv.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vrn.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kim.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bow.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ghx.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://atw.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mtr.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://est.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eqc.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://kuj.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nov.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zso.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://moq.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lav.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://goi.daria6918.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://txv.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ftb.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ioi.xziqi.cn

[F04] 追加写入文件
来源：http://esx.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qob.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://itc.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mat.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oif.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kix.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tzw.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zsd.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mof.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://jvf.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cbs.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://xhn.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://ait.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://uaf.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pcn.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fqk.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://wck.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://lef.ivvv.top

[F06] 删除文件
来源：http://bgr.bbcook.cn

Py:   os.remove("a.txt")
来源：http://vef.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://jux.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hgt.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lhp.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://par.xinyue.icu

Go:   os.Remove("a.txt")
来源：http://xqj.uphjek.com

Ruby: File.delete("a.txt")
来源：http://tbn.yongpay.top

C#:   File.Delete("a.txt");
来源：http://hld.cashguo.top

[F07] 创建目录（含多级）
来源：http://lrm.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hej.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kus.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nla.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aud.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vru.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://idb.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mil.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gae.sxryk.cn

[F08] 遍历目录
来源：http://hnz.fktsv.cn


<!-- 参考信息 -->