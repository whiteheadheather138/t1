代发 wailian999

[D19] 按字段分组
来源：http://hsd.jqgfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wkd.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kok.daria6918.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://svp.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ijt.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qbk.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://ddg.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://abc.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hgb.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://fbh.yangfankeji.com

Py:   Counter(arr)
来源：http://iqb.guannengcc.top

PHP:  array_count_values($arr);
来源：http://ore.hongshengwenyu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tsv.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mnx.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mab.fehbvm.com

Go:   // 手写 map[T]int
来源：http://bku.epnwcf.com

Ruby: arr.tally
来源：http://bhq.nwbrower.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://twy.shanyushiyangtech.top

[D21] 判断是否包含某元素
来源：http://hky.gzhubu.top

Py:   x in arr
来源：http://rit.zhiwuduotai.top

PHP:  in_array($x, $arr, true);
来源：http://bid.zycfv.cn

JS:   arr.includes(x)
来源：http://int.xuanzx.com

TS:   arr.includes(x)
来源：http://bqa.yvedp.cn

Java: list.contains(x)
来源：http://rhy.xuetiantiany.cn

Go:   slices.Contains(arr, x)
来源：http://lcu.ehwqpu.com

Ruby: arr.include?(x)
来源：http://jmz.zdbjq.cn

C#:   list.Contains(x)
来源：http://zqo.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://gtj.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gsn.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nll.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://icy.feifeiyinyue.top

TS:   [...arr];
来源：http://xkt.fzhhl.top

Java: new ArrayList<>(list);
来源：http://jkn.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://jfd.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://lsl.hesvh.cn

C#:   new List<int>(list);
来源：http://uid.daxiang520.top

[D23] reduce 累积计算
来源：http://vhs.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uwz.jqgufenzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wgz.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ssc.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hcz.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fie.zycfv.cn

Go:   // 手写循环
来源：http://rfr.vqdsnc.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://icx.hcnkem.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ydz.daxiang520.top

[D24] 字典 / Map 基本操作
来源：http://prm.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lkc.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rpi.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lxn.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dvh.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lgp.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rkt.xuanzx.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://btn.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ipj.meibo888.top

[D25] Set 集合去重与交并差
来源：http://nde.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wtg.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pru.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ook.epnwcf.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bcs.jinqigfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vel.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://czo.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zud.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ngk.sjlbkw.cn

[D26] 数组转字符串
来源：http://imo.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://pct.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://ezf.snrcjt.cn

JS:   arr.join(", ")
来源：http://mbg.zdbjq.cn

TS:   arr.join(", ")
来源：http://vpf.meibo888.top

Java: String.join(", ", list)
来源：http://xkh.zdbjq.cn

Go:   strings.Join(strs, ", ")
来源：http://voi.haohaochexian.top

Ruby: arr.join(", ")
来源：http://wtm.hesvh.cn

C#:   string.Join(", ", list)
来源：http://zko.cucudq.cn

================================================================================
来源：http://efy.havefunace.top

E. 字符串处理
来源：http://kut.shanyushiyangkeji.top

================================================================================
来源：http://gjj.yfazqb.com

[E01] 拼接字符串
来源：http://tvg.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wxm.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jmb.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dmq.yvedp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zrg.sysykeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://olw.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jwj.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vjc.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jwl.iojbl.cn

[E02] 重复字符串
来源：http://nkh.jianghu66.top

Py:   "ab" * 3
来源：http://jxj.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://wlr.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://bmh.tian-w.cn

TS:   "ab".repeat(3)
来源：http://fph.ppjwa.cn

Java: "ab".repeat(3)
来源：http://tdt.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://lhh.fengsongda.top

Ruby: "ab" * 3
来源：http://eru.jianghu66.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://heq.zhijiandao.cn

[E03] 截取子串
来源：http://hcr.jiagoushi.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xrb.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fov.shuidangran.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://axg.wangshuangyany.cn

TS:   s.slice(1, 4)
来源：http://yat.sxryk.cn

Java: s.substring(1, 4)
来源：http://ddw.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ezb.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xoz.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://qhx.yuanzhike.top

[E04] 查找子串位置
来源：http://gms.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://ocg.yj202588.top

PHP:  strpos($s, "x");
来源：http://qyn.c1oappe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ola.epnwcf.com

TS:   s.indexOf("x")
来源：http://hjk.sxryk.cn

Java: s.indexOf("x")
来源：http://lkr.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://lkn.chenjidiqi.icu

Ruby: s.index("x")
来源：http://inc.52xcode.cn

C#:   s.IndexOf("x")
来源：http://wuz.xziqi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eni.cheryme.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oam.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://irh.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://smn.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qxh.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ook.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mgn.zhengqikj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qdp.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lhz.chenlongwang.top

[E06] 替换子串
来源：http://fjb.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ipw.tianlin.xyz

PHP:  str_replace("a", "b", $s);
来源：http://guv.hammf.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://igc.gotoacloud.top

TS:   s.replaceAll("a", "b")
来源：http://kgi.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ixn.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cvt.hcnkem.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hzb.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://vnl.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://bst.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vyc.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mpu.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gks.sufxvd.cn

TS:   s.split(",")
来源：http://kla.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zjs.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dlz.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://qic.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dwv.andypj.xyz

[E08] 数组按分隔符合并
来源：http://zrg.pycfn.com

Py:   ",".join(items)
来源：http://viw.ehwqpu.com

PHP:  implode(",", $items);
来源：http://ozc.yuanzhike.top

JS:   items.join(",")
来源：http://mzr.zdbjq.cn

TS:   items.join(",")
来源：http://nuz.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://hgd.yuanzhike.top

Go:   strings.Join(items, ",")
来源：http://ber.zycfv.cn

Ruby: items.join(",")
来源：http://czr.iojbl.cn

C#:   string.Join(",", items)
来源：http://dwp.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://swp.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yvy.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ffv.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://mxh.jlsjyb.cn

TS:   s.replace(/\s+/g, "")
来源：http://hul.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://qmp.fzhhl.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gob.fktsv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dhm.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://biw.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://mjc.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hup.birdmap.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kkc.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://zsa.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://jkc.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://kzp.ivvv.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://fra.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cxj.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eyb.vehdjk.com

[E11] 反转字符串
来源：http://yhv.jianghu66.top

Py:   s[::-1]
来源：http://kvq.svipenyu.cn

PHP:  strrev($s);
来源：http://ecm.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://wqx.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://hvp.guowangkeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://itf.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bbi.fengsongda.top

Ruby: s.reverse
来源：http://afz.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://lvn.cheryme.top

[E12] 统计某字符出现次数
来源：http://gsc.iojbl.cn

Py:   s.count("a")
来源：http://qxd.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://edg.zhixingplan.top

JS:   s.split("a").length - 1
来源：http://doi.hcnkem.com

TS:   s.split("a").length - 1
来源：http://xoo.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yrr.hammf.cn

Go:   strings.Count(s, "a")
来源：http://rxh.jianghu66.top

Ruby: s.count("a")
来源：http://ohn.uphjek.com

C#:   s.Count(c => c == 'a')
来源：http://sjn.smart0.xyz

[E13] 逐字符遍历
来源：http://cfw.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://mzp.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://alj.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://npf.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://slu.hongshengwenyu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qfz.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ozg.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lun.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ygp.hcnkem.com

[E14] URL 编码与 Base64
来源：http://ltw.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lki.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ter.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nrf.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ryi.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hwl.bbcook.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wpv.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gca.cucudq.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lnz.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://lvs.sxryk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tmp.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ucm.hywenlv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://djx.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fdm.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cvv.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xlv.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zbz.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rnt.cheryme.top

[E16] 数字千分位
来源：http://ulu.yj20258888.top

Py:   f"{1234567:,}"
来源：http://ugk.yonumen.top

PHP:  number_format(1234567);
来源：http://vca.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uum.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://znc.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pyq.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qqo.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pie.316326.xyz

C#:   1234567.ToString("N0")
来源：http://njv.epnwcf.com

[E17] 首字母大写
来源：http://lqm.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dya.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ona.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jjs.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nvh.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yre.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xgt.zhiwuduotai.top

Ruby: s.capitalize
来源：http://xfv.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ywe.jiagoushi.top

[E18] 模板占位符替换
来源：http://qfd.sysykeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://umu.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nah.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kdo.yj202588.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hqo.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tqi.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kot.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ysx.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vzz.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://uhl.ppjwa.cn

Py:   s.splitlines()
来源：http://rsp.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hnv.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://bzk.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://wyy.daria6918.cn

Java: s.lines().toList()
来源：http://iwv.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://lbm.hysaishi.cn

Ruby: s.lines
来源：http://lwk.chenlongwang.top

C#:   s.Split('\n')
来源：http://lvu.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://bcv.cashguo.top

Py:   if not s:
来源：http://jeo.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zja.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://afk.nwbrower.top

TS:   if (s === "") {}
来源：http://naz.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://nxo.sweek.top

Go:   if s == "" {}
来源：http://zxw.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://lfl.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wgf.gzhubu.top

[E21] 超长截断加省略号
来源：http://rrn.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://chq.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hie.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://stc.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vlr.nwbrower.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fmi.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://yqe.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://inn.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eyg.xuanzx.com

[E22] 字节长度与字符长度
来源：http://myj.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kxm.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yqa.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://odh.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvg.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pmh.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oha.gogol.net.cn

Ruby: s.bytesize;  s.length
来源：http://deo.dashuyun.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eit.zdqjudy.top

================================================================================
来源：http://moz.ywan-chungtsiang.top

F. 文件与目录
来源：http://kyj.cheryme.top

================================================================================
来源：http://jsx.zycfv.cn

[F01] 读取整个文件
来源：http://heb.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zum.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://jtp.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qzs.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fis.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://wah.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kkc.havefunace.top

Ruby: File.read("a.txt")
来源：http://olx.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://qit.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://zqg.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://usr.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tos.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnw.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://owp.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dqu.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rno.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nsk.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yew.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://ght.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://myu.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mhx.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sil.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://osc.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://izc.fktsv.cn


<!-- 参考信息 -->