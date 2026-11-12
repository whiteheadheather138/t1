代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://sxm.zhiwuduotai.top

Ruby: arr.include?(x)
来源：http://jbr.yuanzhike.top

C#:   list.Contains(x)
来源：http://wpc.andypj.xyz

[D22] 复制数组（避免共享引用）
来源：http://yvz.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://myp.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dck.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yje.hfpthk.cn

TS:   [...arr];
来源：http://pen.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://ehg.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://yus.daxiang520.top

Ruby: arr.dup;  arr.clone
来源：http://loh.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://xns.ctjpmb.com

[D23] reduce 累积计算
来源：http://tvg.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xih.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xyd.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hta.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kew.yuanzhike.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zie.zhongyouzk.top

Go:   // 手写循环
来源：http://kaa.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cqp.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yww.quarkkingdee.top

[D24] 字典 / Map 基本操作
来源：http://chh.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ajf.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://utg.sysykeji.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qgg.chenjidiqi.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dfv.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bss.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eqp.wangshuangyany.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wuq.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mre.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://auo.cheryme.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hja.yongpay.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qyq.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://umi.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gpg.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xcq.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gdu.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wmi.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bzy.yj202588.top

[D26] 数组转字符串
来源：http://wme.shzxlz.cn

Py:   ", ".join(map(str, arr))
来源：http://bhh.shzxlz.cn

PHP:  implode(", ", $arr);
来源：http://vup.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://fxm.svipenyu.cn

TS:   arr.join(", ")
来源：http://fis.redwolf501.top

Java: String.join(", ", list)
来源：http://vvv.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://fgz.yueranfly.top

Ruby: arr.join(", ")
来源：http://pyt.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://cjc.nanxinkj.top

================================================================================
来源：http://qgw.hammf.cn

E. 字符串处理
来源：http://nax.shzxlz.cn

================================================================================
来源：http://nko.haohaochexian.top

[E01] 拼接字符串
来源：http://fvd.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sju.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bgw.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://icb.cheryme.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tox.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qbb.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tpj.aizwys.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lat.dashuyun.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zpu.andypj.xyz

[E02] 重复字符串
来源：http://gru.316326.xyz

Py:   "ab" * 3
来源：http://hqw.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://xau.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://wfe.andypj.xyz

TS:   "ab".repeat(3)
来源：http://jxf.cucudq.cn

Java: "ab".repeat(3)
来源：http://hzq.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://abh.cheryme.top

Ruby: "ab" * 3
来源：http://fwg.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kek.xylfe.cn

[E03] 截取子串
来源：http://nvi.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ubr.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uib.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zsz.dianchejie.cn

TS:   s.slice(1, 4)
来源：http://nxx.sweek.top

Java: s.substring(1, 4)
来源：http://ucu.chenlongwang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://emz.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://kee.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://qwz.iojbl.cn

[E04] 查找子串位置
来源：http://pyz.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://sbe.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://too.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://udk.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://oir.cucudq.cn

Java: s.indexOf("x")
来源：http://ppy.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://gwa.xuetiantiany.cn

Ruby: s.index("x")
来源：http://qpr.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://nxz.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://xem.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cxt.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gjw.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://npy.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nqi.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sfm.iojbl.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ihv.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://csl.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kyz.mhx1999.top

[E06] 替换子串
来源：http://tju.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xtr.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://uqy.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mgk.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://uda.gotoacloud.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rpw.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ods.snrcjt.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ksq.hcnkem.com

C#:   s.Replace("a", "b")
来源：http://ifr.hammf.cn

[E07] 按分隔符拆分
来源：http://paa.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwc.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://duv.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kyz.cheryme.top

TS:   s.split(",")
来源：http://qlw.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://ygb.dianchejie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bch.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://eyw.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hhn.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://pao.hammf.cn

Py:   ",".join(items)
来源：http://rjf.wangdashe.top

PHP:  implode(",", $items);
来源：http://bik.pycfn.com

JS:   items.join(",")
来源：http://glb.ybcxt.top

TS:   items.join(",")
来源：http://irq.sufxvd.cn

Java: String.join(",", items)
来源：http://rfw.xuetiantiany.cn

Go:   strings.Join(items, ",")
来源：http://mrn.andypj.xyz

Ruby: items.join(",")
来源：http://wnw.iojbl.cn

C#:   string.Join(",", items)
来源：http://ozw.pengpengdd.cyou

[E09] 去除所有空白字符
来源：http://hpz.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jrv.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://atk.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://dyp.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://gju.sufxvd.cn

Java: s.replaceAll("\\s+", "")
来源：http://heu.epnwcf.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://svw.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://uhr.ybcxt.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hov.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://szj.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ozi.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tms.fanxiaobao.xyz

JS:   "7".padStart(3, "0")
来源：http://szx.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://zws.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://hqb.yfazqb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://gjf.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pdd.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://evd.yj20258888.top

[E11] 反转字符串
来源：http://qez.gaohongyu789.top

Py:   s[::-1]
来源：http://vgx.bbcook.cn

PHP:  strrev($s);
来源：http://caf.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://yeh.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://emc.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uka.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://irh.jqgfzy.top

Ruby: s.reverse
来源：http://ius.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://cuh.ivvv.top

[E12] 统计某字符出现次数
来源：http://jul.chenzaomai.com

Py:   s.count("a")
来源：http://oaq.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://hky.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://jtt.bjfxy.top

TS:   s.split("a").length - 1
来源：http://erx.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hwi.cucudq.cn

Go:   strings.Count(s, "a")
来源：http://zeo.jqgfzy.top

Ruby: s.count("a")
来源：http://aeb.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://xqk.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://hab.yj202588.top

Py:   for ch in s: print(ch)
来源：http://czy.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fbr.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://vil.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sry.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uqe.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ciy.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qch.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tba.bbcook.cn

[E14] URL 编码与 Base64
来源：http://yfs.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ohv.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bep.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vcq.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kyj.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zbc.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fse.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zwg.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pse.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://ggl.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rzh.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zai.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://icg.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ajb.guowangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nfv.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iqc.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wpu.hongshengwenyu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzz.xuetiantiany.cn

[E16] 数字千分位
来源：http://rpc.smart0.xyz

Py:   f"{1234567:,}"
来源：http://tpy.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://ccp.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ypm.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wwp.zdbjq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qqf.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rjo.0kj1m.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lyc.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://ugk.c1oappe.top

[E17] 首字母大写
来源：http://spr.hysaishi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://geo.iojbl.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uxx.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kgj.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fgh.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vke.hnqzz.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ofr.sxryk.cn

Ruby: s.capitalize
来源：http://ywe.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vqg.gogol.net.cn

[E18] 模板占位符替换
来源：http://bkr.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hax.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tvm.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kyh.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://urx.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zhx.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://avy.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gfz.feifeiyinyue.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cid.jinghuilouyu.cn

[E19] 多行文本按行拆分
来源：http://idq.bjfxy.top

Py:   s.splitlines()
来源：http://rya.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tjn.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://gur.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://vfh.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://jfl.zhixingplan.top

Go:   strings.Split(s, "\n")
来源：http://pvx.gaohongyu789.top

Ruby: s.lines
来源：http://pha.xziqi.cn

C#:   s.Split('\n')
来源：http://ceb.yvedp.cn

[E20] 判断字符串是否为空
来源：http://blb.ybcxt.top

Py:   if not s:
来源：http://cnn.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yas.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gns.wangdashe.top

TS:   if (s === "") {}
来源：http://lka.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://lqx.redwolf501.top

Go:   if s == "" {}
来源：http://lah.zhengqikj.top

Ruby: if s.empty?
来源：http://jma.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://her.cucudq.cn

[E21] 超长截断加省略号
来源：http://frk.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xai.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ehl.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sbs.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ueh.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bhu.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://adq.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cim.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qlf.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://smi.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tox.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mqg.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://exz.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jux.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wfx.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lji.gotoacloud.top

Ruby: s.bytesize;  s.length
来源：http://ees.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iyz.xylfe.cn

================================================================================
来源：http://fme.cqqwz.cn

F. 文件与目录
来源：http://hie.nwbrower.top

================================================================================
来源：http://xho.svipenyu.cn

[F01] 读取整个文件
来源：http://jbi.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ags.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://ksl.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xtv.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rvt.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ppo.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hiz.tanke756.top

Ruby: File.read("a.txt")
来源：http://cah.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://yzm.aibaodan.cn

[F02] 逐行读取文件
来源：http://rsb.shanyushiyangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hyr.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zdu.cqqwz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ufi.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hmy.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://soe.ybcxt.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wkk.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qkl.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uyv.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://gmw.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tbb.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cze.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ldl.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ljy.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lvn.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yss.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://tlx.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://olj.fehbvm.com

[F04] 追加写入文件
来源：http://ncg.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://opr.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://naa.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdn.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wnv.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qnu.andypj.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdd.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://erg.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qjf.zhijiandao.cn

[F05] 判断文件或目录是否存在
来源：http://hit.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://irh.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://dxo.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://owj.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://imk.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mdt.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dol.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://gsi.yonumen.top

C#:   File.Exists("a.txt")
来源：http://rxf.hnqzz.top

[F06] 删除文件
来源：http://bng.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://pnf.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://hkr.yongpay.top


<!-- 参考信息 -->