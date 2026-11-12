代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hcz.zhijiandao.cn

JS:   arr.includes(x)
来源：http://pdg.vqdsnc.cn

TS:   arr.includes(x)
来源：http://vjm.tanke756.top

Java: list.contains(x)
来源：http://qvp.snrcjt.cn

Go:   slices.Contains(arr, x)
来源：http://scb.iojbl.cn

Ruby: arr.include?(x)
来源：http://czj.52xcode.cn

C#:   list.Contains(x)
来源：http://rcj.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://sni.xuetiantiany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ubd.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://icc.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iax.zhaomingkeji.xyz

TS:   [...arr];
来源：http://ftk.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://tzy.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://lyt.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://mmr.bbcook.cn

C#:   new List<int>(list);
来源：http://yhh.yongpay.top

[D23] reduce 累积计算
来源：http://ehi.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bch.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jgs.sweek.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fnj.ywan-chungtsiang.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oea.aizwys.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dya.yueranfly.top

Go:   // 手写循环
来源：http://tjt.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gyx.hesvh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ksy.cheryme.top

[D24] 字典 / Map 基本操作
来源：http://mhh.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vnx.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zdq.shzxlz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ncp.ywan-chungtsiang.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jib.ehwqpu.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://odj.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogm.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rcm.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://emx.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://myu.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aax.jinqigufen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wqf.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://djj.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aiw.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mzs.hfpthk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nsm.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uaj.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wzw.fanxiaobao.xyz

[D26] 数组转字符串
来源：http://awz.jqgfzy.top

Py:   ", ".join(map(str, arr))
来源：http://vzf.yj20258.top

PHP:  implode(", ", $arr);
来源：http://agf.epnwcf.com

JS:   arr.join(", ")
来源：http://sym.yueranfly.top

TS:   arr.join(", ")
来源：http://pfx.chenlongwang.top

Java: String.join(", ", list)
来源：http://etm.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://tgl.wangdashe.top

Ruby: arr.join(", ")
来源：http://kqg.hnqzz.top

C#:   string.Join(", ", list)
来源：http://yer.wangdashe.top

================================================================================
来源：http://gnt.hongshengwenyu.top

E. 字符串处理
来源：http://rnd.daria6918.cn

================================================================================
来源：http://loo.jqgufenzy.top

[E01] 拼接字符串
来源：http://phe.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nmz.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wrs.xylfe.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tii.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gjw.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://szj.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xhc.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nqd.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rco.cashguo.top

[E02] 重复字符串
来源：http://haa.hongshengwenyu.top

Py:   "ab" * 3
来源：http://efq.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://rqh.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://dbd.yueranfly.top

TS:   "ab".repeat(3)
来源：http://srh.jianghu66.top

Java: "ab".repeat(3)
来源：http://pba.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://shr.yvedp.cn

Ruby: "ab" * 3
来源：http://dch.chenzaomai.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ixo.haohaochexian.top

[E03] 截取子串
来源：http://ugs.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://acx.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bpv.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ijh.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://tab.zhongyouzk.top

Java: s.substring(1, 4)
来源：http://qsh.nanxinkj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zlo.daria6918.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bwo.yj202588.top

C#:   s.Substring(1, 3)
来源：http://zve.zhiwuduotai.top

[E04] 查找子串位置
来源：http://xqc.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://ksm.iojbl.cn

PHP:  strpos($s, "x");
来源：http://pey.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lwm.vehdjk.com

TS:   s.indexOf("x")
来源：http://krk.cheryme.top

Java: s.indexOf("x")
来源：http://kcr.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://ypz.aibaodan.cn

Ruby: s.index("x")
来源：http://irc.iojbl.cn

C#:   s.IndexOf("x")
来源：http://znf.ivvv.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uff.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jck.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hsa.meibo888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aol.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wfi.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vyw.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ozn.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mfh.feifeiyinyue.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://owt.ppjwa.cn

[E06] 替换子串
来源：http://ory.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sgk.jqgfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://hsi.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fof.jyoumei.cn

TS:   s.replaceAll("a", "b")
来源：http://fxi.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jga.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ylc.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bbi.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://zow.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://flv.nwbrower.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oik.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rjs.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mgr.ctjpmb.com

TS:   s.split(",")
来源：http://joy.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://liy.ydjk.org.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pdg.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://aqs.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mec.xylfe.cn

[E08] 数组按分隔符合并
来源：http://eue.c1oappe.top

Py:   ",".join(items)
来源：http://okk.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://lda.gotoacloud.top

JS:   items.join(",")
来源：http://aga.jqgfzy.top

TS:   items.join(",")
来源：http://iru.chenzaomai.com

Java: String.join(",", items)
来源：http://xbf.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://cip.vqdsnc.cn

Ruby: items.join(",")
来源：http://dxs.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://pld.daria6918.cn

[E09] 去除所有空白字符
来源：http://cpz.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://apo.hongshengwenyu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ifx.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://lpl.havefunace.top

TS:   s.replace(/\s+/g, "")
来源：http://sdq.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://lmb.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tam.snrcjt.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ump.hammf.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ift.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://mno.yj202588.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rek.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ppv.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://owr.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://ydi.chenjidiqi.icu

Java: String.format("%03d", 7)
来源：http://pik.dianchejie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ima.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jnx.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rsg.jqgufenzy.top

[E11] 反转字符串
来源：http://lwk.yangfankeji.com

Py:   s[::-1]
来源：http://gqp.jqgufenzy.top

PHP:  strrev($s);
来源：http://kpf.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://htd.cheryme.top

TS:   [...s].reverse().join("")
来源：http://ocl.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://idq.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://xhu.bbcook.cn

Ruby: s.reverse
来源：http://los.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gjs.nanxinkj.top

[E12] 统计某字符出现次数
来源：http://yce.52xcode.cn

Py:   s.count("a")
来源：http://fme.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://uvf.316326.xyz

JS:   s.split("a").length - 1
来源：http://vse.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://juy.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zdp.feifeiyinyue.top

Go:   strings.Count(s, "a")
来源：http://njh.yuxming.cn

Ruby: s.count("a")
来源：http://icf.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://pnt.xuetiantiany.cn

[E13] 逐字符遍历
来源：http://gis.xziqi.cn

Py:   for ch in s: print(ch)
来源：http://qdo.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bev.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zau.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://rdp.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tdy.meibo888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uhp.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mnv.nanxuanxn.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ybf.hcnkem.com

[E14] URL 编码与 Base64
来源：http://srw.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rmd.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xkl.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eye.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lpg.yuanzhike.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fzw.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bdm.iojbl.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ciq.ywan-chungtsiang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://com.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://dsf.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bwj.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kmb.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hjm.xylfe.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mze.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gus.fzhhl.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hrn.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nvf.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dup.hesvh.cn

[E16] 数字千分位
来源：http://mgj.aizwys.cn

Py:   f"{1234567:,}"
来源：http://fiz.xinyue.icu

PHP:  number_format(1234567);
来源：http://msk.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ihx.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://aoo.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ftf.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sog.hesvh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ekj.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://bgr.bbcook.cn

[E17] 首字母大写
来源：http://nlh.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rme.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://okt.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zrl.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kxt.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jdx.pycfn.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tbp.chenjidiqi.icu

Ruby: s.capitalize
来源：http://fro.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://brh.yuxming.cn

[E18] 模板占位符替换
来源：http://hmu.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vcs.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tyu.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vxf.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rnz.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://imr.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qkc.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qdk.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sdl.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://jxt.smart0.xyz

Py:   s.splitlines()
来源：http://jwd.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wsy.yuanzhike.top

JS:   s.split(/\r?\n/)
来源：http://pgr.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://ckp.aizwys.cn

Java: s.lines().toList()
来源：http://ajv.epnwcf.com

Go:   strings.Split(s, "\n")
来源：http://dkj.ehwqpu.com

Ruby: s.lines
来源：http://bth.ivvv.top

C#:   s.Split('\n')
来源：http://zvh.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://xlm.pycfn.com

Py:   if not s:
来源：http://bcc.cqqwz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://loo.hongshengwenyu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhg.hysaishi.cn

TS:   if (s === "") {}
来源：http://cpc.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://gcv.yfazqb.com

Go:   if s == "" {}
来源：http://ldb.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://qvh.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kte.redwolf501.top

[E21] 超长截断加省略号
来源：http://kci.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://apt.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ajf.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uin.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axd.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sec.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://hgo.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tkl.ydjk.org.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rsf.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://cev.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jit.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rfj.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uaa.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rjx.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://emb.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dir.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://cfg.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qww.yonumen.top

================================================================================
来源：http://yrq.xingfuxueyuan.xyz

F. 文件与目录
来源：http://voo.zycfv.cn

================================================================================
来源：http://pmr.shuidangran.top

[F01] 读取整个文件
来源：http://npw.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nwd.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://sqg.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rdc.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fpl.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qrd.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qzb.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://wlx.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://arw.yfazqb.com

[F02] 逐行读取文件
来源：http://bir.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://trf.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://stc.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dmy.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ujq.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpq.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zxi.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xxl.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://llg.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://ona.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://liv.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fbo.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mlv.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tif.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xri.316326.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eeo.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://rtj.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ids.ivvv.top

[F04] 追加写入文件
来源：http://oqf.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cqn.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hix.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uvb.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://isp.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fum.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gue.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wfo.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zcq.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://plg.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://puh.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://rkg.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://ucx.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://ryg.jinqigufen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gab.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kbf.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://tnc.jinqigfzy.top


<!-- 参考信息 -->