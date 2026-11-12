代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://jdj.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xsx.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://chy.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ahi.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://num.zhaomingkeji.xyz

[D20] 统计每个元素出现次数
来源：http://llc.tanke756.top

Py:   Counter(arr)
来源：http://fdj.cheryme.top

PHP:  array_count_values($arr);
来源：http://rxa.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mls.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xxc.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://utf.c1oappe.top

Go:   // 手写 map[T]int
来源：http://rqk.feifeiyinyue.top

Ruby: arr.tally
来源：http://xyu.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://poy.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://nnb.feifeiyinyue.top

Py:   x in arr
来源：http://nfa.ydzc1.top

PHP:  in_array($x, $arr, true);
来源：http://koy.mhx1999.top

JS:   arr.includes(x)
来源：http://cca.zhixingplan.top

TS:   arr.includes(x)
来源：http://gwo.0kj1m.cn

Java: list.contains(x)
来源：http://anm.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://sle.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://qqu.vehdjk.com

C#:   list.Contains(x)
来源：http://vnq.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://wap.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://pmd.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hmj.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ouc.kuanghao11.cn

TS:   [...arr];
来源：http://vym.aibaodan.cn

Java: new ArrayList<>(list);
来源：http://hen.fehbvm.com

Go:   copied := append([]int(nil), arr...)
来源：http://cbh.shuidangran.top

Ruby: arr.dup;  arr.clone
来源：http://eit.fengsongda.top

C#:   new List<int>(list);
来源：http://vro.snrcjt.cn

[D23] reduce 累积计算
来源：http://rug.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pnn.yanxiufei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yuc.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://acx.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ibf.zhoulong.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://wwc.jinqigfzy.top

Go:   // 手写循环
来源：http://bpt.yvedp.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gcx.meibo888.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mfy.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://zud.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://llt.ywan-chungtsiang.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://stf.yvedp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gej.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ycx.sufxvd.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mil.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tsw.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fli.hnqzz.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nrv.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://aeo.cdnleiting.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vir.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cfh.hfpthk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wkr.jinyuanbaomall.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mku.jyoumei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mbk.fehbvm.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ewn.kuanghao11.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kvl.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zib.sufxvd.cn

[D26] 数组转字符串
来源：http://chv.ehwqpu.com

Py:   ", ".join(map(str, arr))
来源：http://eot.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://iog.gaohongyu789.top

JS:   arr.join(", ")
来源：http://dcf.0kj1m.cn

TS:   arr.join(", ")
来源：http://wto.shzxlz.cn

Java: String.join(", ", list)
来源：http://ujd.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://yzp.gotoacloud.top

Ruby: arr.join(", ")
来源：http://njp.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://ssl.birdmap.top

================================================================================
来源：http://fuf.yangfankeji.com

E. 字符串处理
来源：http://dpl.hcnkem.com

================================================================================
来源：http://xmz.hongshengwenyu.top

[E01] 拼接字符串
来源：http://fef.ppjwa.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dlo.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dmc.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zjj.vqdsnc.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://czh.shanyushiyangtech.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nyt.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rma.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wgm.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xvc.yongpay.top

[E02] 重复字符串
来源：http://kof.c1oappe.top

Py:   "ab" * 3
来源：http://auu.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://acq.guannengcc.top

JS:   "ab".repeat(3)
来源：http://gaa.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://tij.birdmap.top

Java: "ab".repeat(3)
来源：http://tgz.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://qai.zhixingplan.top

Ruby: "ab" * 3
来源：http://shz.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://igu.fktsv.cn

[E03] 截取子串
来源：http://hkn.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://abi.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yxq.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lcs.yonumen.top

TS:   s.slice(1, 4)
来源：http://cis.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://vmt.tian-w.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rtx.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ggt.fktsv.cn

C#:   s.Substring(1, 3)
来源：http://mma.jiagoushi.top

[E04] 查找子串位置
来源：http://ctu.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://vkz.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://rmy.feifeiyinyue.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iiw.andypj.xyz

TS:   s.indexOf("x")
来源：http://few.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://sfh.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://yqk.daxiang520.top

Ruby: s.index("x")
来源：http://zjq.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://krz.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://njq.kuanghao11.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://abs.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mvw.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mup.smart0.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bcr.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wxi.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zfc.tarul.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lou.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vgw.aibaodan.cn

[E06] 替换子串
来源：http://nyw.ppjwa.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gbd.316326.xyz

PHP:  str_replace("a", "b", $s);
来源：http://blo.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yod.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://qub.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxv.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gmh.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://agh.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://zfg.vehdjk.com

[E07] 按分隔符拆分
来源：http://pev.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ola.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jty.andypj.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://vkz.fehbvm.com

TS:   s.split(",")
来源：http://flv.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://urf.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yqc.pengpengdd.cyou

Ruby: s.split(",");  s.split
来源：http://ere.andypj.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hum.hywenlv.cn

[E08] 数组按分隔符合并
来源：http://wxu.jlsjyb.cn

Py:   ",".join(items)
来源：http://zbl.yj202588.top

PHP:  implode(",", $items);
来源：http://bcv.bbcook.cn

JS:   items.join(",")
来源：http://vst.meibo888.top

TS:   items.join(",")
来源：http://vbr.316326.xyz

Java: String.join(",", items)
来源：http://fpv.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://ymx.jqgfzy.top

Ruby: items.join(",")
来源：http://ocf.gaohongyu789.top

C#:   string.Join(",", items)
来源：http://lzr.yangfankeji.com

[E09] 去除所有空白字符
来源：http://ewi.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vjn.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ybf.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://mwq.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://fqv.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://jwy.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ltu.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://qre.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://psm.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://nmy.uphjek.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hsq.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sis.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://npb.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://obo.tanke756.top

Java: String.format("%03d", 7)
来源：http://ern.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yzi.iojbl.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jlh.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://omm.snrcjt.cn

[E11] 反转字符串
来源：http://cne.chenlongwang.top

Py:   s[::-1]
来源：http://pfi.hfpthk.cn

PHP:  strrev($s);
来源：http://tsu.cashguo.top

JS:   [...s].reverse().join("")
来源：http://dck.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://nym.chenzaomai.com

Java: new StringBuilder(s).reverse().toString()
来源：http://dnw.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rpz.shzxlz.cn

Ruby: s.reverse
来源：http://tdm.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://vdm.mhx1999.top

[E12] 统计某字符出现次数
来源：http://tqm.jianghu66.top

Py:   s.count("a")
来源：http://hur.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://pdm.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://dtv.ydzc1.top

TS:   s.split("a").length - 1
来源：http://dhw.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nrz.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://fja.tianlin.xyz

Ruby: s.count("a")
来源：http://ieb.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://rkc.shanyushiyangkeji.top

[E13] 逐字符遍历
来源：http://sno.hongshengwenyu.top

Py:   for ch in s: print(ch)
来源：http://pyw.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://noc.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rze.xinyue.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://myo.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ato.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pyi.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vig.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lrt.hnqzz.top

[E14] URL 编码与 Base64
来源：http://ews.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rmg.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://azj.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://opl.kuanghao11.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lsn.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://flw.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cid.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nsq.shanyushiyangtech.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sqd.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://uas.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://tey.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://okj.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kfc.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kaw.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jhh.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ksq.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ibn.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kit.redwolf501.top

[E16] 数字千分位
来源：http://uyv.havefunace.top

Py:   f"{1234567:,}"
来源：http://rfq.birdmap.top

PHP:  number_format(1234567);
来源：http://coj.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vmu.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gsv.jinqigufen.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rgo.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ktq.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://svl.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://sfn.yfazqb.com

[E17] 首字母大写
来源：http://oiq.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vxz.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kll.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kbp.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hec.aizwys.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hqr.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sdl.hammf.cn

Ruby: s.capitalize
来源：http://zyw.andypj.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zxe.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://qsh.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://czu.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xvd.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mdq.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://bze.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fcu.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vtd.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zfi.fengsongda.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sjm.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://saq.chenjidiqi.icu

Py:   s.splitlines()
来源：http://gzt.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ysl.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://hvd.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://xlf.nwbrower.top

Java: s.lines().toList()
来源：http://ozo.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://dtu.guannengcc.top

Ruby: s.lines
来源：http://whd.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://ypb.ivvv.top

[E20] 判断字符串是否为空
来源：http://yjl.fzhhl.top

Py:   if not s:
来源：http://gzz.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nfy.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gdi.nwbrower.top

TS:   if (s === "") {}
来源：http://mxm.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://bxs.dianchejie.cn

Go:   if s == "" {}
来源：http://rtt.c1oappe.top

Ruby: if s.empty?
来源：http://ybp.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vev.fktsv.cn

[E21] 超长截断加省略号
来源：http://zrv.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sha.zhongyouzk.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ssd.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsz.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hor.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kuo.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://kft.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hkt.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fpo.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://lcx.nanxuanxn.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mtp.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sbb.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ipi.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gup.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hmd.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://era.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ynr.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ooo.bjfxy.top

================================================================================
来源：http://zbc.ppjwa.cn

F. 文件与目录
来源：http://xhc.shzxlz.cn

================================================================================
来源：http://tpr.haohaochexian.top

[F01] 读取整个文件
来源：http://joy.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ghb.chenjidiqi.icu

PHP:  file_get_contents("a.txt");
来源：http://qes.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pzw.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lnu.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ukz.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hth.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://ptj.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://xcb.yuanzhike.top

[F02] 逐行读取文件
来源：http://jvd.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swt.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://msq.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hdj.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxo.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yhx.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kvv.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rkx.epnwcf.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ddb.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://hga.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aqh.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ary.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://prt.yvedp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aah.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wzu.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vqj.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://ijh.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kzr.xylfe.cn

[F04] 追加写入文件
来源：http://trz.fzhhl.top


<!-- 参考信息 -->