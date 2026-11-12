代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://mjd.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zfq.smart0.xyz

Go:   // 手写 map[string][]T
来源：http://ayz.wangdashe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hyr.tian-w.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qfu.yvedp.cn

[D20] 统计每个元素出现次数
来源：http://swk.316326.xyz

Py:   Counter(arr)
来源：http://mpz.52xcode.cn

PHP:  array_count_values($arr);
来源：http://pkz.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pax.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vxk.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dts.fengsongda.top

Go:   // 手写 map[T]int
来源：http://vdv.gotoacloud.top

Ruby: arr.tally
来源：http://sqc.chenlongwang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bnl.shangyingyoupin.top

[D21] 判断是否包含某元素
来源：http://umy.feifeiyinyue.top

Py:   x in arr
来源：http://hgg.jlsjyb.cn

PHP:  in_array($x, $arr, true);
来源：http://mwc.9152youxi.cn

JS:   arr.includes(x)
来源：http://vgm.zhengqikj.top

TS:   arr.includes(x)
来源：http://knt.hfpthk.cn

Java: list.contains(x)
来源：http://juq.52xcode.cn

Go:   slices.Contains(arr, x)
来源：http://dyo.hammf.cn

Ruby: arr.include?(x)
来源：http://ayw.hnqzz.top

C#:   list.Contains(x)
来源：http://mhu.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://mmc.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nwr.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://asz.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ruq.tianlin.xyz

TS:   [...arr];
来源：http://rbs.xuetiantiany.cn

Java: new ArrayList<>(list);
来源：http://gqy.nanxinkj.top

Go:   copied := append([]int(nil), arr...)
来源：http://rlc.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://lvo.zhixingplan.top

C#:   new List<int>(list);
来源：http://gjv.tanke756.top

[D23] reduce 累积计算
来源：http://jbe.aizwys.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dtp.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://npk.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://set.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cri.hongshengwenyu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://any.tarul.cn

Go:   // 手写循环
来源：http://njb.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xjc.hfpthk.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oxw.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://akr.zdbjq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jyx.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aff.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hkc.sufxvd.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://skt.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gbc.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgv.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bza.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://etk.yangfankeji.com

[D25] Set 集合去重与交并差
来源：http://pzp.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tjc.yfazqb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sjg.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tnv.cucudq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ttl.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://agq.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ffe.smart0.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ity.hcnkem.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xtr.zhixingplan.top

[D26] 数组转字符串
来源：http://wzt.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://suv.pengpengdd.cyou

PHP:  implode(", ", $arr);
来源：http://jei.daxiang520.top

JS:   arr.join(", ")
来源：http://kxs.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://nki.sjlbkw.cn

Java: String.join(", ", list)
来源：http://fwu.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://rgb.yangfankeji.com

Ruby: arr.join(", ")
来源：http://qce.bbcook.cn

C#:   string.Join(", ", list)
来源：http://ilr.pycfn.com

================================================================================
来源：http://ffi.jinqigfzy.top

E. 字符串处理
来源：http://otk.cdnleiting.top

================================================================================
来源：http://ghk.dashuyun.cn

[E01] 拼接字符串
来源：http://aal.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ihw.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xww.sjlbkw.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qho.ehwqpu.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vid.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pwt.ydjk.org.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nlr.haohaochexian.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ifg.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bni.quarkkingdee.top

[E02] 重复字符串
来源：http://drv.zdqjudy.top

Py:   "ab" * 3
来源：http://lrq.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://pah.yangfankeji.com

JS:   "ab".repeat(3)
来源：http://yxl.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://arv.ehwqpu.com

Java: "ab".repeat(3)
来源：http://cqg.zycfv.cn

Go:   strings.Repeat("ab", 3)
来源：http://eaj.yanxiufei.cn

Ruby: "ab" * 3
来源：http://awa.cqqwz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://svx.meibo888.top

[E03] 截取子串
来源：http://vww.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wgn.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ciw.meibo888.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hzt.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://hsd.svipenyu.cn

Java: s.substring(1, 4)
来源：http://qbr.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jun.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://jle.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://qeu.sxryk.cn

[E04] 查找子串位置
来源：http://uoz.shuidangran.top

Py:   s.find("x");  s.index("x")
来源：http://cvs.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://pjp.iojbl.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://klu.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://pjb.sweek.top

Java: s.indexOf("x")
来源：http://sdn.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://qmy.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://hvh.sxryk.cn

C#:   s.IndexOf("x")
来源：http://jvg.andypj.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://amh.zdbjq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iub.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jlc.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fnl.zhaomingkeji.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://bhq.xinyue.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://atm.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rtt.sjlbkw.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://abv.gzhubu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ilq.fanxiaobao.xyz

[E06] 替换子串
来源：http://plg.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ycm.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://mel.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xgg.yuxming.cn

TS:   s.replaceAll("a", "b")
来源：http://kjw.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pun.dianchejie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zrj.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jxy.dashuyun.cn

C#:   s.Replace("a", "b")
来源：http://mss.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://ake.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ltq.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kzo.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ebs.ywan-chungtsiang.top

TS:   s.split(",")
来源：http://htn.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xkl.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tfa.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://gaf.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kyx.pycfn.com

[E08] 数组按分隔符合并
来源：http://mqv.xuanzx.com

Py:   ",".join(items)
来源：http://zcj.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://jmr.yj20258.top

JS:   items.join(",")
来源：http://jtm.ivvv.top

TS:   items.join(",")
来源：http://oef.havefunace.top

Java: String.join(",", items)
来源：http://bym.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://sfp.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://pqc.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://vzq.guowangkeji.top

[E09] 去除所有空白字符
来源：http://ref.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oqt.haohaochexian.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gax.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://fhj.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://mvf.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://psv.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mda.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tlj.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yvq.sxryk.cn

[E10] 左侧补零 / 定长填充
来源：http://lwi.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://thz.zhoulong.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hrw.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://fyv.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://stz.mhx1999.top

Java: String.format("%03d", 7)
来源：http://hxs.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fmp.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ezp.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xxf.zhongyouzk.top

[E11] 反转字符串
来源：http://kst.hnxiangtu.top

Py:   s[::-1]
来源：http://ctk.sweek.top

PHP:  strrev($s);
来源：http://sut.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://qey.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://hrb.shanyushiyangtech.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zzb.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://chx.tarul.cn

Ruby: s.reverse
来源：http://yge.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ttz.yvedp.cn

[E12] 统计某字符出现次数
来源：http://hyb.pengpengdd.cyou

Py:   s.count("a")
来源：http://prf.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://tfx.hysaishi.cn

JS:   s.split("a").length - 1
来源：http://rpi.bbcook.cn

TS:   s.split("a").length - 1
来源：http://wxe.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ktt.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://cod.tianlin.xyz

Ruby: s.count("a")
来源：http://iwh.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://oem.cqqwz.cn

[E13] 逐字符遍历
来源：http://ibd.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://xqq.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kww.zdbjq.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://giw.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ywr.316326.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://azc.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://btv.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wov.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bvc.epnwcf.com

[E14] URL 编码与 Base64
来源：http://ysc.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kyc.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://joh.ywan-chungtsiang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xnr.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nrf.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nym.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mjg.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://spa.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ofq.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://ify.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://voe.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://age.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wlo.tianlin.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://okx.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dam.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://brl.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hxa.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sme.vqdsnc.cn

[E16] 数字千分位
来源：http://oux.sysykeji.top

Py:   f"{1234567:,}"
来源：http://hya.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://gaj.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ktl.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qol.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pfq.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://buz.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://usg.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://mqm.ivvv.top

[E17] 首字母大写
来源：http://qip.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ffz.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://doq.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nto.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://irb.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bfj.zdbjq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jle.xuanzx.com

Ruby: s.capitalize
来源：http://ddl.wangshuangyany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ctx.xuetiantiany.cn

[E18] 模板占位符替换
来源：http://glh.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ziq.xinyue.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cqo.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pat.hammf.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vkg.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qhc.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://etx.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gyt.zhoulong.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://klz.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://uut.sweek.top

Py:   s.splitlines()
来源：http://nge.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eyq.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://rep.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://rfp.fehbvm.com

Java: s.lines().toList()
来源：http://ikm.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://mio.yuanzhike.top

Ruby: s.lines
来源：http://ike.zhixingplan.top

C#:   s.Split('\n')
来源：http://tol.yj202588.top

[E20] 判断字符串是否为空
来源：http://mvp.snrcjt.cn

Py:   if not s:
来源：http://htk.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://npt.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pgs.hammf.cn

TS:   if (s === "") {}
来源：http://sxg.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://xbh.tian-w.cn

Go:   if s == "" {}
来源：http://gka.hysaishi.cn

Ruby: if s.empty?
来源：http://cgi.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mxg.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://ndy.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wbk.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ozw.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jap.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksz.feifeiyinyue.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uaj.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://ezd.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xbs.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oyy.cucudq.cn

[E22] 字节长度与字符长度
来源：http://zhc.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fvj.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cyo.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pwd.yangfankeji.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pdt.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jnr.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eke.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://fcm.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mox.hysaishi.cn

================================================================================
来源：http://aiz.wangdashe.top

F. 文件与目录
来源：http://luv.yueranfly.top

================================================================================
来源：http://tbg.zhoulong.xyz

[F01] 读取整个文件
来源：http://uoh.sjlbkw.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zkk.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://hjm.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zic.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://frk.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jfw.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rrg.andypj.xyz

Ruby: File.read("a.txt")
来源：http://oaz.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gcv.nanxuanxn.top

[F02] 逐行读取文件
来源：http://jrg.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yzk.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nbt.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ybn.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zvz.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bcz.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cgt.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ipe.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jxt.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://fli.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ggh.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eok.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijf.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tjr.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mep.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sbj.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://cfv.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ngr.chenzaomai.com

[F04] 追加写入文件
来源：http://lkt.jianghu66.top


<!-- 参考信息 -->