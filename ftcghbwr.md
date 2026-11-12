代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://eja.hcnkem.com

Go:   // 手写双层循环
来源：http://djg.yj20258888.top

Ruby: nested.flatten
来源：http://wdl.zhiwuduotai.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wwb.tian-w.cn

[D19] 按字段分组
来源：http://pnp.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sqp.jqgfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dzp.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gvd.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://qfk.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zvb.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://brm.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wde.jianghu66.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oav.uphjek.com

[D20] 统计每个元素出现次数
来源：http://ijo.316326.xyz

Py:   Counter(arr)
来源：http://mmh.ehwqpu.com

PHP:  array_count_values($arr);
来源：http://cqc.hesvh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wvb.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lya.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://che.yj202588.top

Go:   // 手写 map[T]int
来源：http://qmg.jinqigufen.top

Ruby: arr.tally
来源：http://ywv.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fdd.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://zmg.chenzaomai.com

Py:   x in arr
来源：http://cci.tarul.cn

PHP:  in_array($x, $arr, true);
来源：http://zkx.yfazqb.com

JS:   arr.includes(x)
来源：http://zqe.yangfankeji.com

TS:   arr.includes(x)
来源：http://twm.ppjwa.cn

Java: list.contains(x)
来源：http://oar.hongshengwenyu.top

Go:   slices.Contains(arr, x)
来源：http://fhg.birdmap.top

Ruby: arr.include?(x)
来源：http://roe.yongpay.top

C#:   list.Contains(x)
来源：http://voh.pengpengdd.cyou

[D22] 复制数组（避免共享引用）
来源：http://pqc.shangyingyoupin.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://waw.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://esy.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fhu.zdqjudy.top

TS:   [...arr];
来源：http://blk.daxiang520.top

Java: new ArrayList<>(list);
来源：http://ved.cdnleiting.top

Go:   copied := append([]int(nil), arr...)
来源：http://oju.fanxiaobao.xyz

Ruby: arr.dup;  arr.clone
来源：http://hwi.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://gre.snrcjt.cn

[D23] reduce 累积计算
来源：http://bur.ehwqpu.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vow.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sri.xuanzx.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxc.xinyue.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zxe.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://prb.chenjidiqi.icu

Go:   // 手写循环
来源：http://hhw.wangdashe.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bnl.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cfe.jiagoushi.top

[D24] 字典 / Map 基本操作
来源：http://sml.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kxn.dashuyun.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nte.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ext.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fwk.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nje.shangyingyoupin.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nxq.haohaochexian.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qei.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rdb.ywan-chungtsiang.top

[D25] Set 集合去重与交并差
来源：http://oaz.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rlr.zhixingplan.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yqf.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://keo.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zmi.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uuv.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aaa.jlsjyb.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hef.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://daf.hongshengwenyu.top

[D26] 数组转字符串
来源：http://lnr.ydjk.org.cn

Py:   ", ".join(map(str, arr))
来源：http://qvt.yj20258.top

PHP:  implode(", ", $arr);
来源：http://zaq.fehbvm.com

JS:   arr.join(", ")
来源：http://cdw.zhixingplan.top

TS:   arr.join(", ")
来源：http://hso.jqgufenzy.top

Java: String.join(", ", list)
来源：http://raa.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://jwa.hfpthk.cn

Ruby: arr.join(", ")
来源：http://tkz.havefunace.top

C#:   string.Join(", ", list)
来源：http://hvl.fehbvm.com

================================================================================
来源：http://ifp.jianghu66.top

E. 字符串处理
来源：http://pfa.ivvv.top

================================================================================
来源：http://vzm.chenzaomai.com

[E01] 拼接字符串
来源：http://bwm.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uyw.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jyh.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ean.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wpf.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lvq.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jmz.fktsv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rnu.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://swb.cashguo.top

[E02] 重复字符串
来源：http://nzr.uphjek.com

Py:   "ab" * 3
来源：http://ftr.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://qgb.yongpay.top

JS:   "ab".repeat(3)
来源：http://vhh.uphjek.com

TS:   "ab".repeat(3)
来源：http://odb.zhengqikj.top

Java: "ab".repeat(3)
来源：http://tsq.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://shc.c1oappe.top

Ruby: "ab" * 3
来源：http://yfm.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xlz.shzxlz.cn

[E03] 截取子串
来源：http://ksv.shuidangran.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nyo.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qra.tian-w.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kno.tianlin.xyz

TS:   s.slice(1, 4)
来源：http://zgn.cashguo.top

Java: s.substring(1, 4)
来源：http://vfa.jinghuilouyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dhs.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://qlh.zdbjq.cn

C#:   s.Substring(1, 3)
来源：http://bnt.fzhhl.top

[E04] 查找子串位置
来源：http://jdq.shanyushiyangtech.top

Py:   s.find("x");  s.index("x")
来源：http://cab.tanke756.top

PHP:  strpos($s, "x");
来源：http://qhh.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jqq.cheryme.top

TS:   s.indexOf("x")
来源：http://uzb.yanxiufei.cn

Java: s.indexOf("x")
来源：http://qht.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://zrq.xuanzx.com

Ruby: s.index("x")
来源：http://sjy.daxiang520.top

C#:   s.IndexOf("x")
来源：http://kev.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ynb.daria6918.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gab.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zmu.mhx1999.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ctn.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bbh.tanke756.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://exz.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vny.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dyt.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gib.jianghu66.top

[E06] 替换子串
来源：http://omm.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qsk.ctjpmb.com

PHP:  str_replace("a", "b", $s);
来源：http://sti.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mrt.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://eit.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yao.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ucr.hongshengwenyu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yaw.yvedp.cn

C#:   s.Replace("a", "b")
来源：http://nai.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://rui.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rvw.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hcx.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://smx.pengpengdd.cyou

TS:   s.split(",")
来源：http://ieg.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://mau.vqdsnc.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ecf.havefunace.top

Ruby: s.split(",");  s.split
来源：http://vou.zhongyouzk.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vsv.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://dnm.ctjpmb.com

Py:   ",".join(items)
来源：http://ujr.snrcjt.cn

PHP:  implode(",", $items);
来源：http://uer.shuidangran.top

JS:   items.join(",")
来源：http://qtb.tian-w.cn

TS:   items.join(",")
来源：http://prh.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://tgp.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://ede.nanxuanxn.top

Ruby: items.join(",")
来源：http://sxy.gotoacloud.top

C#:   string.Join(",", items)
来源：http://npf.chenzaomai.com

[E09] 去除所有空白字符
来源：http://eqa.sxryk.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sve.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yzo.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://srt.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://dye.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://ojt.jyoumei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ywx.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://rsq.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ybb.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://dhh.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dlx.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aui.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://sgo.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://urv.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://lrh.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vxu.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hjt.hnxiangtu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dgl.bbcook.cn

[E11] 反转字符串
来源：http://ynp.haohaochexian.top

Py:   s[::-1]
来源：http://mnp.xuanzx.com

PHP:  strrev($s);
来源：http://rgh.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://une.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://tkz.sweek.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bne.yj202588.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://whl.yj202588.top

Ruby: s.reverse
来源：http://pne.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://sda.52xcode.cn

[E12] 统计某字符出现次数
来源：http://chn.tarul.cn

Py:   s.count("a")
来源：http://mfe.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://bzj.hcnkem.com

JS:   s.split("a").length - 1
来源：http://puk.ywan-chungtsiang.top

TS:   s.split("a").length - 1
来源：http://bso.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rvm.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://rxv.xylfe.cn

Ruby: s.count("a")
来源：http://wgk.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://csd.tanke756.top

[E13] 逐字符遍历
来源：http://ejn.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://mln.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qbh.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rhc.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://sjl.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jgc.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mun.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fhd.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wwx.daxiang520.top

[E14] URL 编码与 Base64
来源：http://mlb.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cxb.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kky.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tnw.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rfg.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qwx.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zcc.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mqb.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sid.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://sdr.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qlm.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tbh.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ias.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kmw.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://urw.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tmp.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cwp.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dgf.gotoacloud.top

[E16] 数字千分位
来源：http://ytr.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://awe.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://xrp.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fqz.vehdjk.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ewe.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://har.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jcj.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://abl.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://exz.zdqjudy.top

[E17] 首字母大写
来源：http://mtz.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://awk.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://qxd.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wsu.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rtp.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wgj.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bmk.hysaishi.cn

Ruby: s.capitalize
来源：http://pow.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zot.cucudq.cn

[E18] 模板占位符替换
来源：http://ljq.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bgj.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tsk.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vbz.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pca.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pgg.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://edk.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pde.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mgt.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://knn.xziqi.cn

Py:   s.splitlines()
来源：http://fow.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://afv.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://ekl.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://cxl.feifeiyinyue.top

Java: s.lines().toList()
来源：http://tej.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://kou.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://yth.sjlbkw.cn

C#:   s.Split('\n')
来源：http://agj.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://myf.ydjk.org.cn

Py:   if not s:
来源：http://mwi.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nqc.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ujw.iojbl.cn

TS:   if (s === "") {}
来源：http://jis.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://rcc.hammf.cn

Go:   if s == "" {}
来源：http://yob.316326.xyz

Ruby: if s.empty?
来源：http://irr.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cqy.316326.xyz

[E21] 超长截断加省略号
来源：http://xpo.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dgq.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pqf.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcy.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yal.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cuk.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://acp.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mli.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rtb.smart0.xyz

[E22] 字节长度与字符长度
来源：http://ngy.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jnn.chenzaomai.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lrp.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://csj.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eps.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pzu.fktsv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fif.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://iya.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gqf.cdnleiting.top

================================================================================
来源：http://nbe.gzhubu.top

F. 文件与目录
来源：http://bib.shuidangran.top

================================================================================
来源：http://otz.mhx1999.top

[F01] 读取整个文件
来源：http://rrj.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vgg.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://ywz.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xue.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qoi.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yvd.ywan-chungtsiang.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ccd.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://qll.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://pwx.jqgfzy.top

[F02] 逐行读取文件
来源：http://vtg.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hvs.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xtu.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iug.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mhu.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vdj.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hon.ybcxt.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xpf.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pgf.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://npx.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jpk.xuetiantiany.cn


<!-- 参考信息 -->