代发 wailian999

[D23] reduce 累积计算
来源：http://fzq.sysykeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://paz.hywenlv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tgn.jinqigfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fsf.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qyz.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://aba.jinghuilouyu.cn

Go:   // 手写循环
来源：http://blc.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wwr.ppjwa.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qdz.chenjidiqi.icu

[D24] 字典 / Map 基本操作
来源：http://lce.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xea.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://tco.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yef.yj20258.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lyc.jlsjyb.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gfo.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://glc.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iyh.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rno.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://oec.yuanzhike.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://row.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qsz.sysykeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ete.vehdjk.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kmf.vqdsnc.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ggz.cqqwz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mju.hysaishi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lzs.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mum.kuanghao11.cn

[D26] 数组转字符串
来源：http://kib.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://jto.bjfxy.top

PHP:  implode(", ", $arr);
来源：http://lkn.haohaochexian.top

JS:   arr.join(", ")
来源：http://wct.zhixingplan.top

TS:   arr.join(", ")
来源：http://une.gotoacloud.top

Java: String.join(", ", list)
来源：http://lzm.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://auq.feifeiyinyue.top

Ruby: arr.join(", ")
来源：http://jav.shanyushiyangkeji.top

C#:   string.Join(", ", list)
来源：http://zzt.tarul.cn

================================================================================
来源：http://bmu.hongshengwenyu.top

E. 字符串处理
来源：http://mke.jianghu66.top

================================================================================
来源：http://xxi.meibo888.top

[E01] 拼接字符串
来源：http://omv.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lkm.zdbjq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://huj.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nsr.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ewt.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hus.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pgq.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jzu.cashguo.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rzy.jinyuanbaomall.cn

[E02] 重复字符串
来源：http://rpx.guannengcc.top

Py:   "ab" * 3
来源：http://tjt.zhijiandao.cn

PHP:  str_repeat("ab", 3);
来源：http://ymp.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://inq.xuetiantiany.cn

TS:   "ab".repeat(3)
来源：http://xxh.jinqigufen.top

Java: "ab".repeat(3)
来源：http://fzy.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://ajy.jinqigufen.top

Ruby: "ab" * 3
来源：http://ndw.yangfankeji.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wvk.tarul.cn

[E03] 截取子串
来源：http://cxg.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://noe.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ukn.fehbvm.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nuc.zhaomingkeji.xyz

TS:   s.slice(1, 4)
来源：http://jrh.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://vyr.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zdq.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ohr.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://ukj.ybcxt.top

[E04] 查找子串位置
来源：http://lcv.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://kha.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://etw.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://icp.dianchejie.cn

TS:   s.indexOf("x")
来源：http://guw.hysaishi.cn

Java: s.indexOf("x")
来源：http://jvs.redwolf501.top

Go:   strings.Index(s, "x")
来源：http://ipb.cucudq.cn

Ruby: s.index("x")
来源：http://qcf.guannengcc.top

C#:   s.IndexOf("x")
来源：http://jbd.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://vdt.zhixingplan.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iap.ywan-chungtsiang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jdb.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://drf.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cfh.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yua.yangfankeji.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dgn.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vtd.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uwq.cdnleiting.top

[E06] 替换子串
来源：http://asj.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rkl.jianghu66.top

PHP:  str_replace("a", "b", $s);
来源：http://ith.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vzi.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://qqz.fktsv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qcv.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://exw.chenjidiqi.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://haa.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://lea.ehwqpu.com

[E07] 按分隔符拆分
来源：http://jlk.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jfa.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ayp.daria6918.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bpf.c1oappe.top

TS:   s.split(",")
来源：http://tzv.gotoacloud.top

Java: s.split(",");  s.split("\\s+")
来源：http://tft.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gnn.gaohongyu789.top

Ruby: s.split(",");  s.split
来源：http://ycc.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kpj.yongpay.top

[E08] 数组按分隔符合并
来源：http://poe.sufxvd.cn

Py:   ",".join(items)
来源：http://vlm.hammf.cn

PHP:  implode(",", $items);
来源：http://mrp.yj202588.top

JS:   items.join(",")
来源：http://bnl.shuidangran.top

TS:   items.join(",")
来源：http://mdm.yj20258888.top

Java: String.join(",", items)
来源：http://ecm.aizwys.cn

Go:   strings.Join(items, ",")
来源：http://wbp.nanxinkj.top

Ruby: items.join(",")
来源：http://emn.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://bex.gotoacloud.top

[E09] 去除所有空白字符
来源：http://xbr.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qzu.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qvr.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://dhl.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://ahk.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://vdi.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://reg.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://jid.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yjm.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://yse.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aou.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ctt.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://gah.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://hgi.yonumen.top

Java: String.format("%03d", 7)
来源：http://xpq.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://swp.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bky.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qee.aizwys.cn

[E11] 反转字符串
来源：http://bvl.jinghuilouyu.cn

Py:   s[::-1]
来源：http://mmt.sysykeji.top

PHP:  strrev($s);
来源：http://oif.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://cet.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://scb.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tny.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kfh.fehbvm.com

Ruby: s.reverse
来源：http://smn.yonumen.top

C#:   new string(s.Reverse().ToArray())
来源：http://aol.sysykeji.top

[E12] 统计某字符出现次数
来源：http://kfe.jqgufenzy.top

Py:   s.count("a")
来源：http://eix.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://vjp.hammf.cn

JS:   s.split("a").length - 1
来源：http://lph.xuanzx.com

TS:   s.split("a").length - 1
来源：http://hwi.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hsu.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://byu.gzhubu.top

Ruby: s.count("a")
来源：http://jhk.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://jsx.sysykeji.top

[E13] 逐字符遍历
来源：http://ldv.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://xlo.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvg.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oml.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://arm.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uwy.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yyw.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iod.jiagoushi.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wrj.yvedp.cn

[E14] URL 编码与 Base64
来源：http://ulq.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vsv.yanxiufei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gdi.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ggd.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mal.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xuz.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yqz.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://paf.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://etu.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://qni.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lvy.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://stu.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tsh.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xzc.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kur.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xuh.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://otn.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mhl.fehbvm.com

[E16] 数字千分位
来源：http://mfp.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://ull.sysykeji.top

PHP:  number_format(1234567);
来源：http://ojm.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xye.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://brd.quarkkingdee.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xwd.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://czf.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xkk.cashguo.top

C#:   1234567.ToString("N0")
来源：http://jdr.zhoulong.xyz

[E17] 首字母大写
来源：http://ekc.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rzr.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gbr.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zgh.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bep.yuxming.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gel.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rwu.svipenyu.cn

Ruby: s.capitalize
来源：http://idf.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vev.nanxuanxn.top

[E18] 模板占位符替换
来源：http://tpm.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zdy.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mog.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pos.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mpu.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iyw.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wqw.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rtb.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fef.meibo888.top

[E19] 多行文本按行拆分
来源：http://pev.svipenyu.cn

Py:   s.splitlines()
来源：http://pho.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://djn.hnqzz.top

JS:   s.split(/\r?\n/)
来源：http://qez.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://mlx.sweek.top

Java: s.lines().toList()
来源：http://bem.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://vkd.fengsongda.top

Ruby: s.lines
来源：http://kvx.tanke756.top

C#:   s.Split('\n')
来源：http://gau.hesvh.cn

[E20] 判断字符串是否为空
来源：http://krs.ydzc1.top

Py:   if not s:
来源：http://gig.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fvk.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lff.shanyushiyangtech.top

TS:   if (s === "") {}
来源：http://qde.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://qbv.haohaochexian.top

Go:   if s == "" {}
来源：http://yga.snrcjt.cn

Ruby: if s.empty?
来源：http://lop.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kbu.uphjek.com

[E21] 超长截断加省略号
来源：http://ywy.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ews.wangshuangyany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://byk.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jey.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://arr.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gib.yj20258888.top

Go:   // 按 rune 判断长度后截断
来源：http://ooh.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://arb.gogol.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ajy.cdnleiting.top

[E22] 字节长度与字符长度
来源：http://btn.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ail.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yhk.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://klq.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwn.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oev.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wbe.aibaodan.cn

Ruby: s.bytesize;  s.length
来源：http://kya.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://udq.yanxiufei.cn

================================================================================
来源：http://dzk.sufxvd.cn

F. 文件与目录
来源：http://czf.shanyushiyangtech.top

================================================================================
来源：http://edf.jqgfzy.top

[F01] 读取整个文件
来源：http://pxg.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hlo.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://aqu.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://scx.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dop.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dqe.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qzs.pycfn.com

Ruby: File.read("a.txt")
来源：http://qvp.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://cpb.ivvv.top

[F02] 逐行读取文件
来源：http://smo.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lky.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://deh.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yas.ydzc1.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yme.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mqk.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yqz.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kvw.feifeiyinyue.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hew.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://jum.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hdd.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bnv.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbw.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qaq.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uws.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://msi.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://uqo.zhiwuduotai.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://owz.haohaochexian.top

[F04] 追加写入文件
来源：http://oha.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lvf.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ucw.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lea.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vep.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cvh.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wgs.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ykb.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kna.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://uyo.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dlk.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://icw.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://iul.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://ego.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://utd.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kby.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://ivw.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://ndd.feifeiyinyue.top

[F06] 删除文件
来源：http://xru.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://srb.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://nqj.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ymu.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://rgu.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ged.birdmap.top

Go:   os.Remove("a.txt")
来源：http://syt.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://geg.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://qak.gzhubu.top

[F07] 创建目录（含多级）
来源：http://rlj.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vur.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qfw.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyn.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lbx.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pia.ppjwa.cn


<!-- 参考信息 -->