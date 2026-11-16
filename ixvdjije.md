代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://ybu.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hit.zycfv.cn

TS:   Math.max(...arr);
来源：http://xmm.hnqzz.top

Java: Collections.max(list);  Collections.min(list);
来源：http://uhi.snrcjt.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ijv.ydjk.org.cn

Ruby: arr.max;  arr.min
来源：http://csy.sweek.top

C#:   list.Max();  list.Min()
来源：http://efu.redwolf501.top

[D18] 扁平化嵌套数组
来源：http://tfg.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kfb.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://lou.hysaishi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mnk.chenzaomai.com

TS:   nested.flat();
来源：http://goz.zhengqikj.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hjb.xingfuxueyuan.xyz

Go:   // 手写双层循环
来源：http://keo.iojbl.cn

Ruby: nested.flatten
来源：http://gyp.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://lxo.epnwcf.com

[D19] 按字段分组
来源：http://vyo.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://thw.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ihi.ehwqpu.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hoe.zhiwuduotai.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lvp.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bta.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://kkb.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rik.bbcook.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xse.cashguo.top

[D20] 统计每个元素出现次数
来源：http://exi.bbcook.cn

Py:   Counter(arr)
来源：http://zrg.fzhhl.top

PHP:  array_count_values($arr);
来源：http://fxt.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhu.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xsz.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oqf.andypj.xyz

Go:   // 手写 map[T]int
来源：http://tzj.hysaishi.cn

Ruby: arr.tally
来源：http://xmr.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tao.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://ldm.guannengcc.top

Py:   x in arr
来源：http://bou.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://xgt.gaohongyu789.top

JS:   arr.includes(x)
来源：http://obp.xinyue.icu

TS:   arr.includes(x)
来源：http://hov.guannengcc.top

Java: list.contains(x)
来源：http://wym.nanxinkj.top

Go:   slices.Contains(arr, x)
来源：http://pow.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://tlh.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://ldy.ppjwa.cn

[D22] 复制数组（避免共享引用）
来源：http://idp.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cxc.tarul.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fxl.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ckm.pycfn.com

TS:   [...arr];
来源：http://tye.shanyushiyangtech.top

Java: new ArrayList<>(list);
来源：http://ljz.nwbrower.top

Go:   copied := append([]int(nil), arr...)
来源：http://gvo.xuetiantiany.cn

Ruby: arr.dup;  arr.clone
来源：http://klg.xingfuxueyuan.xyz

C#:   new List<int>(list);
来源：http://hfs.wangdashe.top

[D23] reduce 累积计算
来源：http://eqt.ppjwa.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eim.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yel.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wwn.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zge.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ymp.wangshuangyany.cn

Go:   // 手写循环
来源：http://ekr.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rht.sweek.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dfx.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://khi.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bbm.xuanzx.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dje.yuxming.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yhy.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dnk.guowangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://itl.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://eab.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uju.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jqj.yj202588.top

[D25] Set 集合去重与交并差
来源：http://ton.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://guv.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fgn.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mtt.ivvv.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qmh.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aor.zhijiandao.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vya.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bez.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qks.sysykeji.top

[D26] 数组转字符串
来源：http://cvw.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://coj.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://taq.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://yff.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://kqf.fktsv.cn

Java: String.join(", ", list)
来源：http://ybg.wangdashe.top

Go:   strings.Join(strs, ", ")
来源：http://ldf.iojbl.cn

Ruby: arr.join(", ")
来源：http://eld.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://fho.aizwys.cn

================================================================================
来源：http://rwz.wangdashe.top

E. 字符串处理
来源：http://ytt.yangfankeji.com

================================================================================
来源：http://ymh.jinqigufen.top

[E01] 拼接字符串
来源：http://ifa.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vsa.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gfl.yongpay.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lfw.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oqp.xuanzx.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sih.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pyr.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iee.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nox.aizwys.cn

[E02] 重复字符串
来源：http://hhw.kuanghao11.cn

Py:   "ab" * 3
来源：http://myb.zhaomingkeji.xyz

PHP:  str_repeat("ab", 3);
来源：http://lau.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://lzf.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://bce.cashguo.top

Java: "ab".repeat(3)
来源：http://trg.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://nfk.fehbvm.com

Ruby: "ab" * 3
来源：http://yvd.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sun.zhongyouzk.top

[E03] 截取子串
来源：http://pcs.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://shr.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://myq.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cca.hcnkem.com

TS:   s.slice(1, 4)
来源：http://qqd.ydjk.org.cn

Java: s.substring(1, 4)
来源：http://xnn.yj20258888.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zhi.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fpj.yonumen.top

C#:   s.Substring(1, 3)
来源：http://uxr.yangfankeji.com

[E04] 查找子串位置
来源：http://pte.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://xir.zycfv.cn

PHP:  strpos($s, "x");
来源：http://tav.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://any.yonumen.top

TS:   s.indexOf("x")
来源：http://wij.jqgufenzy.top

Java: s.indexOf("x")
来源：http://exb.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://epu.cqqwz.cn

Ruby: s.index("x")
来源：http://omr.xinyue.icu

C#:   s.IndexOf("x")
来源：http://xne.haohaochexian.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lbj.epnwcf.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sne.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rqb.chenjidiqi.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dnk.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nru.ivvv.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fgi.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cul.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wtq.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bim.kuanghao11.cn

[E06] 替换子串
来源：http://eti.fanxiaobao.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zvh.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://yrf.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pxp.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://ynz.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://led.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ymr.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://npa.fktsv.cn

C#:   s.Replace("a", "b")
来源：http://yhj.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://flj.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oes.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uwr.jiagoushi.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xpo.quarkkingdee.top

TS:   s.split(",")
来源：http://imb.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://rsy.yj20258888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tou.pycfn.com

Ruby: s.split(",");  s.split
来源：http://iul.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dug.sweek.top

[E08] 数组按分隔符合并
来源：http://nkj.zhongyouzk.top

Py:   ",".join(items)
来源：http://fga.cucudq.cn

PHP:  implode(",", $items);
来源：http://rox.yangfankeji.com

JS:   items.join(",")
来源：http://okd.zhoulong.xyz

TS:   items.join(",")
来源：http://jgj.yangfankeji.com

Java: String.join(",", items)
来源：http://lzg.shanyushiyangkeji.top

Go:   strings.Join(items, ",")
来源：http://cyv.yongpay.top

Ruby: items.join(",")
来源：http://lhw.cheryme.top

C#:   string.Join(",", items)
来源：http://giq.nanxinkj.top

[E09] 去除所有空白字符
来源：http://nug.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://idg.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://stp.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://txs.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://xoj.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://xhv.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qjk.xuanzx.com

Ruby: s.gsub(/\s+/, "")
来源：http://gfr.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fcj.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://lhe.yuxming.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pbd.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uia.shuidangran.top

JS:   "7".padStart(3, "0")
来源：http://loy.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://swj.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://pro.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xlo.daxiang520.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jma.shanyushiyangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xjd.sjlbkw.cn

[E11] 反转字符串
来源：http://ssr.ctjpmb.com

Py:   s[::-1]
来源：http://erc.chenjidiqi.icu

PHP:  strrev($s);
来源：http://tfp.aibaodan.cn

JS:   [...s].reverse().join("")
来源：http://sbi.cashguo.top

TS:   [...s].reverse().join("")
来源：http://mdb.wangdashe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://onf.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://uwz.haohaochexian.top

Ruby: s.reverse
来源：http://wgp.hnxiangtu.top

C#:   new string(s.Reverse().ToArray())
来源：http://cfb.gzhubu.top

[E12] 统计某字符出现次数
来源：http://wtu.yueranfly.top

Py:   s.count("a")
来源：http://qwo.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://wyl.bjfxy.top

JS:   s.split("a").length - 1
来源：http://vfo.daxiang520.top

TS:   s.split("a").length - 1
来源：http://ued.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gpa.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://cba.sysykeji.top

Ruby: s.count("a")
来源：http://ksu.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://lta.zhoulong.xyz

[E13] 逐字符遍历
来源：http://wix.shuidangran.top

Py:   for ch in s: print(ch)
来源：http://ivq.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://djm.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lwu.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://exh.nwbrower.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ujb.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aiw.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pjc.dashuyun.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yat.yueranfly.top

[E14] URL 编码与 Base64
来源：http://wpp.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://olj.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eyb.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oai.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yjy.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lre.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ynq.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cbi.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yma.gaohongyu789.top

[E15] HTML 转义 / 反转义
来源：http://wdp.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pws.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://paz.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nsf.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://isg.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uob.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oih.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://djf.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://smc.jinqigfzy.top

[E16] 数字千分位
来源：http://pab.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://miu.shzxlz.cn

PHP:  number_format(1234567);
来源：http://wng.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ros.yueranfly.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tbp.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ovg.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dqw.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zyt.epnwcf.com

C#:   1234567.ToString("N0")
来源：http://lan.hesvh.cn

[E17] 首字母大写
来源：http://crk.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cqm.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zkf.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ykk.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mcd.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eyk.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qot.shangyingyoupin.top

Ruby: s.capitalize
来源：http://njn.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xyq.sweek.top

[E18] 模板占位符替换
来源：http://spy.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fbk.gaohongyu789.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cya.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hmy.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lwl.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jyn.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xad.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rkl.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lau.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://pxv.cucudq.cn

Py:   s.splitlines()
来源：http://led.yj20258888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pfx.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://tpw.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://dvt.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://mpx.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://jra.dashuyun.cn

Ruby: s.lines
来源：http://vgo.hnxiangtu.top

C#:   s.Split('\n')
来源：http://esz.vehdjk.com

[E20] 判断字符串是否为空
来源：http://iol.iojbl.cn

Py:   if not s:
来源：http://qhn.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kvj.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cqa.hnxiangtu.top

TS:   if (s === "") {}
来源：http://bit.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://cqq.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://ryi.cheryme.top

Ruby: if s.empty?
来源：http://eew.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qyw.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://mtz.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xfk.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jig.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gah.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qqs.daxiang520.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://flp.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://ptn.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mbw.9152youxi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wbq.aizwys.cn

[E22] 字节长度与字符长度
来源：http://jmp.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pzl.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cxh.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lcm.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://enw.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pvw.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vnu.feifeiyinyue.top

Ruby: s.bytesize;  s.length
来源：http://mnu.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qwx.hfpthk.cn

================================================================================
来源：http://dui.smart0.xyz

F. 文件与目录
来源：http://cuv.mhx1999.top

================================================================================
来源：http://qwd.quarkkingdee.top

[F01] 读取整个文件
来源：http://oas.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zwj.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://kim.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ggw.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eqe.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kuu.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rqa.tarul.cn

Ruby: File.read("a.txt")
来源：http://cmt.tian-w.cn


<!-- 参考信息 -->