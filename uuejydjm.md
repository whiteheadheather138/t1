代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gsa.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://apf.andypj.xyz

Go:   // 手写循环
来源：http://naz.0kj1m.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://udk.shzxlz.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sly.zhengqikj.top

[D24] 字典 / Map 基本操作
来源：http://lix.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kjs.vehdjk.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ofm.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pjh.cucudq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yxq.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ove.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kqd.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qtv.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://don.fengsongda.top

[D25] Set 集合去重与交并差
来源：http://rxl.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rbe.9152youxi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wsb.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pvh.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hzk.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rjp.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qmj.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hap.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zoe.pengpengdd.cyou

[D26] 数组转字符串
来源：http://pen.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://foj.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://eay.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://iob.tarul.cn

TS:   arr.join(", ")
来源：http://bkw.yfazqb.com

Java: String.join(", ", list)
来源：http://pnc.fehbvm.com

Go:   strings.Join(strs, ", ")
来源：http://drd.zhengqikj.top

Ruby: arr.join(", ")
来源：http://xjg.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://uya.fzhhl.top

================================================================================
来源：http://sqa.cashguo.top

E. 字符串处理
来源：http://coy.fehbvm.com

================================================================================
来源：http://vro.c1oappe.top

[E01] 拼接字符串
来源：http://wkp.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gue.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zgt.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gui.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyc.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://syp.zycfv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zvk.hcnkem.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zlp.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mih.shangyingyoupin.top

[E02] 重复字符串
来源：http://aaa.jiagoushi.top

Py:   "ab" * 3
来源：http://ico.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://ksx.yj20258.top

JS:   "ab".repeat(3)
来源：http://sab.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://xyk.cheryme.top

Java: "ab".repeat(3)
来源：http://cnh.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://uad.sxryk.cn

Ruby: "ab" * 3
来源：http://rde.chenjidiqi.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pyw.nwbrower.top

[E03] 截取子串
来源：http://pff.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rnd.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://koa.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://frq.aizwys.cn

TS:   s.slice(1, 4)
来源：http://afn.zdbjq.cn

Java: s.substring(1, 4)
来源：http://kud.yuanzhike.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wca.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://lpc.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://oyc.daxiang520.top

[E04] 查找子串位置
来源：http://qbc.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://trt.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://brf.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wrx.cashguo.top

TS:   s.indexOf("x")
来源：http://fyo.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://iee.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://rzv.daria6918.cn

Ruby: s.index("x")
来源：http://rsn.andypj.xyz

C#:   s.IndexOf("x")
来源：http://efv.xylfe.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://aiy.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cwt.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dmt.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ige.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://eia.jlsjyb.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zlb.sjlbkw.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ruj.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rjb.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lte.smart0.xyz

[E06] 替换子串
来源：http://kxz.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sdc.sweek.top

PHP:  str_replace("a", "b", $s);
来源：http://lzg.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lyo.yongpay.top

TS:   s.replaceAll("a", "b")
来源：http://env.iojbl.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkm.zhaomingkeji.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xuy.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rcf.jinghuilouyu.cn

C#:   s.Replace("a", "b")
来源：http://wkz.cqqwz.cn

[E07] 按分隔符拆分
来源：http://gwq.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tmv.c1oappe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lbq.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://ccw.zhoulong.xyz

TS:   s.split(",")
来源：http://vbi.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://oku.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jrv.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://rpl.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xop.hcnkem.com

[E08] 数组按分隔符合并
来源：http://mlh.pycfn.com

Py:   ",".join(items)
来源：http://txc.jyoumei.cn

PHP:  implode(",", $items);
来源：http://jpv.quarkkingdee.top

JS:   items.join(",")
来源：http://iyg.fktsv.cn

TS:   items.join(",")
来源：http://fva.feifeiyinyue.top

Java: String.join(",", items)
来源：http://oic.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://pkh.vqdsnc.cn

Ruby: items.join(",")
来源：http://krf.c1oappe.top

C#:   string.Join(",", items)
来源：http://zpr.epnwcf.com

[E09] 去除所有空白字符
来源：http://yil.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://szs.ybcxt.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bch.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://poe.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://qem.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://qrt.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qtx.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://qll.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dxz.jinghuilouyu.cn

[E10] 左侧补零 / 定长填充
来源：http://gfa.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dgz.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ehc.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://grh.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://rqn.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://xcb.smart0.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://tpe.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rur.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jvw.sxryk.cn

[E11] 反转字符串
来源：http://hwz.ctjpmb.com

Py:   s[::-1]
来源：http://uri.gogol.net.cn

PHP:  strrev($s);
来源：http://upy.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://lzp.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://fqi.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://qmt.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://her.jiagoushi.top

Ruby: s.reverse
来源：http://gpu.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hrg.zycfv.cn

[E12] 统计某字符出现次数
来源：http://bgj.aibaodan.cn

Py:   s.count("a")
来源：http://dzl.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://ssh.cdnleiting.top

JS:   s.split("a").length - 1
来源：http://ftm.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://vjm.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pog.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://hbw.meibo888.top

Ruby: s.count("a")
来源：http://ikg.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://sol.jlsjyb.cn

[E13] 逐字符遍历
来源：http://dns.ybcxt.top

Py:   for ch in s: print(ch)
来源：http://xii.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ofh.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ugg.ydzc1.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nba.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zef.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jlb.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://dht.jlsjyb.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wga.xuanzx.com

[E14] URL 编码与 Base64
来源：http://itj.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lti.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hjv.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bhe.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wyi.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pch.chenlongwang.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bei.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://daj.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ifu.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://gzc.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fdd.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ana.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rgt.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lwh.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mza.tianlin.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yid.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vnq.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lya.dianchejie.cn

[E16] 数字千分位
来源：http://fgk.chenlongwang.top

Py:   f"{1234567:,}"
来源：http://fpr.cucudq.cn

PHP:  number_format(1234567);
来源：http://ssu.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://bll.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://cdq.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vau.fengsongda.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hor.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lay.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://eee.zhiwuduotai.top

[E17] 首字母大写
来源：http://nam.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ncx.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hqe.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hvj.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ari.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lgy.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zna.zhixingplan.top

Ruby: s.capitalize
来源：http://akd.yueranfly.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ceh.zhongyouzk.top

[E18] 模板占位符替换
来源：http://hwh.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qxl.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ekl.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rac.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ynf.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://max.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qel.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kgr.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fad.epnwcf.com

[E19] 多行文本按行拆分
来源：http://ptd.uphjek.com

Py:   s.splitlines()
来源：http://vnz.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://prh.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://yfp.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://fmu.zhengqikj.top

Java: s.lines().toList()
来源：http://ntr.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://lrl.shzxlz.cn

Ruby: s.lines
来源：http://vbn.smart0.xyz

C#:   s.Split('\n')
来源：http://jfg.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://ocv.fengsongda.top

Py:   if not s:
来源：http://srv.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://imn.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qoy.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://pol.andypj.xyz

Java: if (s.isEmpty()) {}
来源：http://adi.andypj.xyz

Go:   if s == "" {}
来源：http://ymy.guowangkeji.top

Ruby: if s.empty?
来源：http://bmx.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hry.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://dff.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ako.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pnc.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lis.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vbc.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ala.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://rss.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fut.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wcb.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://vmz.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lif.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cmx.ehwqpu.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tzf.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mbd.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://keo.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rvf.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://und.fanxiaobao.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zkc.havefunace.top

================================================================================
来源：http://wcu.andypj.xyz

F. 文件与目录
来源：http://vbg.jinqigufen.top

================================================================================
来源：http://hiv.kuanghao11.cn

[F01] 读取整个文件
来源：http://nbe.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wjv.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://wwu.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tyu.cashguo.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vtd.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://gna.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ulw.tian-w.cn

Ruby: File.read("a.txt")
来源：http://wyf.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://nwo.jqgufenzy.top

[F02] 逐行读取文件
来源：http://cqt.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qrk.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bfp.jianghu66.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wld.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uae.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ooe.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ewn.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pbi.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fab.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://otd.yueranfly.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jds.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mvq.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iju.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dtc.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fwn.nwbrower.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fsu.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://zzx.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wjj.9152youxi.cn

[F04] 追加写入文件
来源：http://exz.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cav.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nka.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pau.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyn.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ilw.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://aae.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vyg.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ssl.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://jfs.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xht.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://taq.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://blj.smart0.xyz

TS:   fs.existsSync("a.txt")
来源：http://ecq.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tbs.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hoz.fengsongda.top

Ruby: File.exist?("a.txt")
来源：http://txe.quarkkingdee.top

C#:   File.Exists("a.txt")
来源：http://swy.haohaochexian.top

[F06] 删除文件
来源：http://wtj.fzhhl.top

Py:   os.remove("a.txt")
来源：http://qij.daria6918.cn

PHP:  unlink("a.txt");
来源：http://uvg.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://avd.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://wnk.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://siq.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://abq.ivvv.top

Ruby: File.delete("a.txt")
来源：http://aml.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://ebi.sweek.top

[F07] 创建目录（含多级）
来源：http://jcw.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hix.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wnb.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gdd.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tqn.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yhv.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rff.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tvu.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ffg.yuanzhike.top

[F08] 遍历目录
来源：http://dsx.xingfuxueyuan.xyz


<!-- 参考信息 -->