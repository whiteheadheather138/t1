代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dwj.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://umh.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mjw.xinyue.icu

Go:   // 手写 map[T]int
来源：http://udf.wangdashe.top

Ruby: arr.tally
来源：http://fag.shanyushiyangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://imi.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://twv.aibaodan.cn

Py:   x in arr
来源：http://avi.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://xgk.daria6918.cn

JS:   arr.includes(x)
来源：http://bik.jiagoushi.top

TS:   arr.includes(x)
来源：http://lpu.hfpthk.cn

Java: list.contains(x)
来源：http://sne.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://kxn.xuanzx.com

Ruby: arr.include?(x)
来源：http://sac.c1oappe.top

C#:   list.Contains(x)
来源：http://ukl.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://lsh.guowangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wnu.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kfo.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xlb.hnqzz.top

TS:   [...arr];
来源：http://hjf.jianghu66.top

Java: new ArrayList<>(list);
来源：http://fst.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://ndv.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://xwi.sysykeji.top

C#:   new List<int>(list);
来源：http://bqn.cheryme.top

[D23] reduce 累积计算
来源：http://fvk.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sfp.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fid.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hag.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uuz.sjlbkw.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rwl.shuidangran.top

Go:   // 手写循环
来源：http://asy.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mnj.daxiang520.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pub.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://syd.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dul.jinqigfzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wnz.uphjek.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gzp.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iep.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wif.jqgufenzy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mor.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xsj.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://keb.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://aus.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wnl.zdbjq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://deb.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eei.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pqe.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ney.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://msc.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tgr.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oud.ehwqpu.com

[D26] 数组转字符串
来源：http://dpo.yfazqb.com

Py:   ", ".join(map(str, arr))
来源：http://vfq.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://bac.nwbrower.top

JS:   arr.join(", ")
来源：http://jfk.52xcode.cn

TS:   arr.join(", ")
来源：http://lju.hammf.cn

Java: String.join(", ", list)
来源：http://vbf.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://gcg.bjfxy.top

Ruby: arr.join(", ")
来源：http://muk.bbcook.cn

C#:   string.Join(", ", list)
来源：http://kde.c1oappe.top

================================================================================
来源：http://pse.cheryme.top

E. 字符串处理
来源：http://ywn.nanxinkj.top

================================================================================
来源：http://iih.xziqi.cn

[E01] 拼接字符串
来源：http://wuz.fengsongda.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jfw.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yaw.jinyuanbaomall.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tye.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mtx.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://npo.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tap.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sqn.vehdjk.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://buj.fehbvm.com

[E02] 重复字符串
来源：http://rjf.hcnkem.com

Py:   "ab" * 3
来源：http://hwv.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://jyu.meibo888.top

JS:   "ab".repeat(3)
来源：http://snx.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://zaj.fengsongda.top

Java: "ab".repeat(3)
来源：http://akv.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://ada.fktsv.cn

Ruby: "ab" * 3
来源：http://zyq.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vuk.meibo888.top

[E03] 截取子串
来源：http://vmd.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vio.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wyt.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://owb.tarul.cn

TS:   s.slice(1, 4)
来源：http://jzd.bjfxy.top

Java: s.substring(1, 4)
来源：http://vil.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ury.iojbl.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jmd.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://djq.zhongyouzk.top

[E04] 查找子串位置
来源：http://rrw.ivvv.top

Py:   s.find("x");  s.index("x")
来源：http://tsd.tianlin.xyz

PHP:  strpos($s, "x");
来源：http://pya.jinqigufen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://efb.nwbrower.top

TS:   s.indexOf("x")
来源：http://ymo.birdmap.top

Java: s.indexOf("x")
来源：http://ctg.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://cnv.bjfxy.top

Ruby: s.index("x")
来源：http://avm.zhongyouzk.top

C#:   s.IndexOf("x")
来源：http://zev.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kmf.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wzb.cdnleiting.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zsd.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ysj.daxiang520.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vzt.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tqn.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://twg.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wdp.guannengcc.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nky.xuetiantiany.cn

[E06] 替换子串
来源：http://jjz.ivvv.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yku.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://ogy.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ljb.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://oea.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fhx.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xiu.ppjwa.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fhm.birdmap.top

C#:   s.Replace("a", "b")
来源：http://erb.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://yot.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://syt.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qkj.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cgl.52xcode.cn

TS:   s.split(",")
来源：http://zow.jiagoushi.top

Java: s.split(",");  s.split("\\s+")
来源：http://nfb.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kzp.sxryk.cn

Ruby: s.split(",");  s.split
来源：http://kha.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rxc.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://mlt.svipenyu.cn

Py:   ",".join(items)
来源：http://qpt.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://amz.vehdjk.com

JS:   items.join(",")
来源：http://sfw.tanke756.top

TS:   items.join(",")
来源：http://twz.dianchejie.cn

Java: String.join(",", items)
来源：http://wth.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://gcg.jinqigfzy.top

Ruby: items.join(",")
来源：http://ydk.iojbl.cn

C#:   string.Join(",", items)
来源：http://jhn.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://jsl.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxo.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://szg.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://znn.xinyue.icu

TS:   s.replace(/\s+/g, "")
来源：http://mbc.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://trc.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qku.jinyuanbaomall.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hvm.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ptn.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://rqs.dianchejie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://slk.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ocz.kuanghao11.cn

JS:   "7".padStart(3, "0")
来源：http://cjo.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://nwz.epnwcf.com

Java: String.format("%03d", 7)
来源：http://xdr.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pio.tarul.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lhe.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://epn.fzhhl.top

[E11] 反转字符串
来源：http://veu.zycfv.cn

Py:   s[::-1]
来源：http://shp.fanxiaobao.xyz

PHP:  strrev($s);
来源：http://vtz.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://bcw.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://iii.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://nbk.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://jro.daria6918.cn

Ruby: s.reverse
来源：http://wbc.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://ixc.snrcjt.cn

[E12] 统计某字符出现次数
来源：http://nlm.bjfxy.top

Py:   s.count("a")
来源：http://lhw.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://omp.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://qsx.guannengcc.top

TS:   s.split("a").length - 1
来源：http://wfo.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kfg.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://imc.daria6918.cn

Ruby: s.count("a")
来源：http://nam.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://gvd.xziqi.cn

[E13] 逐字符遍历
来源：http://tmo.uphjek.com

Py:   for ch in s: print(ch)
来源：http://mgf.gogol.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vap.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zet.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bbn.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pkd.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://woq.zdbjq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kct.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jzp.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://agt.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://etd.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jmc.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ttg.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qli.hnqzz.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mvd.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zmy.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dpa.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ftx.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://wxe.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://zzj.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wfz.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cwe.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ypk.feifeiyinyue.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xqq.yonumen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vol.wangdashe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://psw.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kjb.chenzaomai.com

[E16] 数字千分位
来源：http://hbd.xylfe.cn

Py:   f"{1234567:,}"
来源：http://ivt.daria6918.cn

PHP:  number_format(1234567);
来源：http://anb.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://adx.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jbt.jinghuilouyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hpo.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aaq.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://odg.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://ams.cqqwz.cn

[E17] 首字母大写
来源：http://mwe.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://avd.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cxz.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bdw.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tgk.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jxh.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bau.9152youxi.cn

Ruby: s.capitalize
来源：http://hjh.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aqw.yj20258.top

[E18] 模板占位符替换
来源：http://ngy.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zrx.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dtx.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://kru.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hgs.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xai.jinghuilouyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fei.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jiu.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wdq.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://jul.sweek.top

Py:   s.splitlines()
来源：http://byp.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xot.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://ilc.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://syp.pengpengdd.cyou

Java: s.lines().toList()
来源：http://ntq.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://vdx.bbcook.cn

Ruby: s.lines
来源：http://vtl.nwbrower.top

C#:   s.Split('\n')
来源：http://vrd.sxryk.cn

[E20] 判断字符串是否为空
来源：http://reu.zhiwuduotai.top

Py:   if not s:
来源：http://lvi.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ryc.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dwb.sxryk.cn

TS:   if (s === "") {}
来源：http://xjm.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://wee.hammf.cn

Go:   if s == "" {}
来源：http://ktq.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://ddl.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ifw.0kj1m.cn

[E21] 超长截断加省略号
来源：http://hfr.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lun.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eus.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbs.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sqb.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zpq.hnqzz.top

Go:   // 按 rune 判断长度后截断
来源：http://sva.shangyingyoupin.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mtl.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xup.vehdjk.com

[E22] 字节长度与字符长度
来源：http://kra.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lco.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qal.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://goh.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zss.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://axy.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pzo.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://hrw.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dtw.bbcook.cn

================================================================================
来源：http://rcv.sysykeji.top

F. 文件与目录
来源：http://hjo.haohaochexian.top

================================================================================
来源：http://jai.jlsjyb.cn

[F01] 读取整个文件
来源：http://iup.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://llc.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://ogg.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hgm.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iom.jinqigufen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://uhg.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pyi.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://tut.fengsongda.top

C#:   File.ReadAllText("a.txt");
来源：http://wnl.havefunace.top

[F02] 逐行读取文件
来源：http://rji.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://suo.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nue.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sri.quarkkingdee.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://euz.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dgi.gotoacloud.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dmx.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://piy.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://frf.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://xly.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ixj.ehwqpu.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://aso.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wyp.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://udn.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://czt.cqqwz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cds.snrcjt.cn

Ruby: File.write("a.txt", "hi")
来源：http://tsm.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eqk.gaohongyu789.top

[F04] 追加写入文件
来源：http://qdy.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vrd.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mfg.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qvz.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yvv.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ouj.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ygi.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lua.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://omn.jinyuanbaomall.cn


<!-- 参考信息 -->