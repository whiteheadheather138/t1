代发 wailian999

[D19] 按字段分组
来源：http://awo.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xji.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nap.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://thn.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://mak.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ddh.yuanzhike.top

Go:   // 手写 map[string][]T
来源：http://mqx.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oog.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pld.hysaishi.cn

[D20] 统计每个元素出现次数
来源：http://wgb.zhaomingkeji.xyz

Py:   Counter(arr)
来源：http://zem.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://jbs.feifeiyinyue.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cle.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rsx.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lrf.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://kqp.fengsongda.top

Ruby: arr.tally
来源：http://som.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://omk.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://dcz.iojbl.cn

Py:   x in arr
来源：http://nir.wangshuangyany.cn

PHP:  in_array($x, $arr, true);
来源：http://juq.316326.xyz

JS:   arr.includes(x)
来源：http://sjl.jinqigfzy.top

TS:   arr.includes(x)
来源：http://sui.xuanzx.com

Java: list.contains(x)
来源：http://eve.bjfxy.top

Go:   slices.Contains(arr, x)
来源：http://cpj.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://den.ydzc1.top

C#:   list.Contains(x)
来源：http://dzc.snrcjt.cn

[D22] 复制数组（避免共享引用）
来源：http://bll.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bho.daxiang520.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qlh.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ziu.aizwys.cn

TS:   [...arr];
来源：http://jyg.fzhhl.top

Java: new ArrayList<>(list);
来源：http://xrf.guowangkeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://hrv.vqdsnc.cn

Ruby: arr.dup;  arr.clone
来源：http://ecr.hywenlv.cn

C#:   new List<int>(list);
来源：http://obz.ydjk.org.cn

[D23] reduce 累积计算
来源：http://zyf.shuidangran.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kfk.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nzi.cucudq.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://btv.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zri.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jrc.ydjk.org.cn

Go:   // 手写循环
来源：http://enn.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rds.aizwys.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mfy.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://ebo.cdnleiting.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yui.hysaishi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://udv.xziqi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ewc.fzhhl.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dmt.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rsw.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pkb.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cmz.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uon.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://gsx.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bte.fanxiaobao.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ali.c1oappe.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vrc.yongpay.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tsi.yuanzhike.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jff.aizwys.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jzc.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ktn.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fbl.tian-w.cn

[D26] 数组转字符串
来源：http://bcy.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://bpa.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://mbr.tanke756.top

JS:   arr.join(", ")
来源：http://cjt.yueranfly.top

TS:   arr.join(", ")
来源：http://mct.hnxiangtu.top

Java: String.join(", ", list)
来源：http://jvf.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://yvg.cucudq.cn

Ruby: arr.join(", ")
来源：http://aia.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://ukq.daria6918.cn

================================================================================
来源：http://cwn.cheryme.top

E. 字符串处理
来源：http://ust.bbcook.cn

================================================================================
来源：http://kff.birdmap.top

[E01] 拼接字符串
来源：http://nmd.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ell.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zmp.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uba.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uvk.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hiz.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pmz.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xxy.havefunace.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://huj.gotoacloud.top

[E02] 重复字符串
来源：http://mmh.fengsongda.top

Py:   "ab" * 3
来源：http://gxb.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://djo.sjlbkw.cn

JS:   "ab".repeat(3)
来源：http://krl.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://kfj.daxiang520.top

Java: "ab".repeat(3)
来源：http://tvf.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://jxr.yj20258.top

Ruby: "ab" * 3
来源：http://wjs.c1oappe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zcc.birdmap.top

[E03] 截取子串
来源：http://mja.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ibz.fktsv.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tmh.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ikq.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://oil.yj20258888.top

Java: s.substring(1, 4)
来源：http://wmm.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rpx.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://mcw.jianghu66.top

C#:   s.Substring(1, 3)
来源：http://dio.chenjidiqi.icu

[E04] 查找子串位置
来源：http://lpr.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://bxf.gzhubu.top

PHP:  strpos($s, "x");
来源：http://lox.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mxo.smart0.xyz

TS:   s.indexOf("x")
来源：http://niq.jqgufenzy.top

Java: s.indexOf("x")
来源：http://liu.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://cob.fzhhl.top

Ruby: s.index("x")
来源：http://koe.fzhhl.top

C#:   s.IndexOf("x")
来源：http://ogi.hammf.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://toy.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iil.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rvd.yj20258.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://knm.yfazqb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ram.hywenlv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lsw.sysykeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zxl.zhaomingkeji.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uka.pengpengdd.cyou

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iuu.cucudq.cn

[E06] 替换子串
来源：http://stm.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dds.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://bwk.fanxiaobao.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zcd.hywenlv.cn

TS:   s.replaceAll("a", "b")
来源：http://zza.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://grc.ivvv.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bms.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tmw.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://vqk.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://bcx.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qbp.zycfv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nyn.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://upc.316326.xyz

TS:   s.split(",")
来源：http://cox.hongshengwenyu.top

Java: s.split(",");  s.split("\\s+")
来源：http://mnp.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://prl.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://tqy.yueranfly.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyp.epnwcf.com

[E08] 数组按分隔符合并
来源：http://nkt.zdqjudy.top

Py:   ",".join(items)
来源：http://yam.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://jna.jinqigufen.top

JS:   items.join(",")
来源：http://ifi.zhixingplan.top

TS:   items.join(",")
来源：http://axd.chenzaomai.com

Java: String.join(",", items)
来源：http://vmx.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://pqd.dashuyun.cn

Ruby: items.join(",")
来源：http://pix.hysaishi.cn

C#:   string.Join(",", items)
来源：http://wud.hfpthk.cn

[E09] 去除所有空白字符
来源：http://nkk.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hgy.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gwj.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://guc.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://gmx.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://god.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pdu.gzhubu.top

Ruby: s.gsub(/\s+/, "")
来源：http://vsn.jinqigufen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ese.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://kot.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ntv.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qwj.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://drr.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://yjw.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://igp.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://bsa.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rps.hcnkem.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zye.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://sly.fengsongda.top

Py:   s[::-1]
来源：http://qgv.dashuyun.cn

PHP:  strrev($s);
来源：http://qqt.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://bdx.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://reg.yfazqb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://peb.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wfo.fktsv.cn

Ruby: s.reverse
来源：http://apb.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://elg.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://boi.xziqi.cn

Py:   s.count("a")
来源：http://ezx.yongpay.top

PHP:  substr_count($s, "a");
来源：http://zbs.vehdjk.com

JS:   s.split("a").length - 1
来源：http://mps.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://qut.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://guf.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://vtq.ehwqpu.com

Ruby: s.count("a")
来源：http://jfa.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://vjg.yfazqb.com

[E13] 逐字符遍历
来源：http://ipd.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://apo.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zqo.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iqn.9152youxi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ypt.0kj1m.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hcp.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cay.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://wmd.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lwb.sufxvd.cn

[E14] URL 编码与 Base64
来源：http://hgj.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hwv.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ewf.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tqi.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uwe.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zkg.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ozj.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uzr.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zqt.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://zir.sysykeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lsb.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bnd.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fbf.fengsongda.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lfm.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ejf.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sxc.dianchejie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wab.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://idl.jinyuanbaomall.cn

[E16] 数字千分位
来源：http://bda.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://jdk.sysykeji.top

PHP:  number_format(1234567);
来源：http://svr.hnqzz.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jxt.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kep.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xyt.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dqp.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wsk.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://gil.xinyue.icu

[E17] 首字母大写
来源：http://qai.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gqz.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://lat.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isf.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mnp.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bxe.yfazqb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sle.hnqzz.top

Ruby: s.capitalize
来源：http://rja.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://brr.9152youxi.cn

[E18] 模板占位符替换
来源：http://ewg.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ypb.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dvi.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://blq.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://jjk.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qxu.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eql.aibaodan.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bpj.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tcq.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://fuw.cdnleiting.top

Py:   s.splitlines()
来源：http://pqy.vehdjk.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lkp.meibo888.top

JS:   s.split(/\r?\n/)
来源：http://pom.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://caq.xuetiantiany.cn

Java: s.lines().toList()
来源：http://siz.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://ams.bbcook.cn

Ruby: s.lines
来源：http://ena.chenjidiqi.icu

C#:   s.Split('\n')
来源：http://egu.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://udy.pengpengdd.cyou

Py:   if not s:
来源：http://bwy.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vag.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kcs.yvedp.cn

TS:   if (s === "") {}
来源：http://ihl.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://spj.wangdashe.top

Go:   if s == "" {}
来源：http://ngm.wangshuangyany.cn

Ruby: if s.empty?
来源：http://cmi.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lrc.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://rxc.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dqq.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cip.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vsi.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cuu.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kve.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://opk.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://byk.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aye.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://vja.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pva.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jtc.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iaj.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qyr.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ftd.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bpn.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://mwd.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hxz.ywan-chungtsiang.top

================================================================================
来源：http://qhm.wangshuangyany.cn

F. 文件与目录
来源：http://rff.jqgfzy.top

================================================================================
来源：http://yrq.nanxinkj.top

[F01] 读取整个文件
来源：http://uds.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dxh.wangshuangyany.cn

PHP:  file_get_contents("a.txt");
来源：http://uqh.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xcj.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rkv.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eyz.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://viz.epnwcf.com

Ruby: File.read("a.txt")
来源：http://cjo.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://est.svipenyu.cn

[F02] 逐行读取文件
来源：http://xhm.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dfr.52xcode.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lsc.shzxlz.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rmo.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ers.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fjy.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pnu.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://btr.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yrt.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://mzc.vqdsnc.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vuo.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xca.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epo.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ctn.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://otv.gotoacloud.top


<!-- 参考信息 -->