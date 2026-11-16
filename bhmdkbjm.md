代发 wailian999

[D19] 按字段分组
来源：http://tyi.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ewv.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gpi.jqgfzy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gxj.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vka.hammf.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jex.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://lwo.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://duf.316326.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ejx.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://xel.xuanzx.com

Py:   Counter(arr)
来源：http://xtw.yuxming.cn

PHP:  array_count_values($arr);
来源：http://xny.zdqjudy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gxt.shanyushiyangtech.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvq.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ctg.hammf.cn

Go:   // 手写 map[T]int
来源：http://ckc.sysykeji.top

Ruby: arr.tally
来源：http://bmt.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fsw.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://hcf.yueranfly.top

Py:   x in arr
来源：http://eyj.zhengqikj.top

PHP:  in_array($x, $arr, true);
来源：http://sfn.epnwcf.com

JS:   arr.includes(x)
来源：http://dxv.quarkkingdee.top

TS:   arr.includes(x)
来源：http://eyk.jinyuanbaomall.cn

Java: list.contains(x)
来源：http://mip.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://fvq.iojbl.cn

Ruby: arr.include?(x)
来源：http://eeq.birdmap.top

C#:   list.Contains(x)
来源：http://hjz.shzxlz.cn

[D22] 复制数组（避免共享引用）
来源：http://ktn.guannengcc.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kfd.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hdn.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dwg.dianchejie.cn

TS:   [...arr];
来源：http://dxf.hammf.cn

Java: new ArrayList<>(list);
来源：http://uqh.jqgfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://loy.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://eop.zycfv.cn

C#:   new List<int>(list);
来源：http://pyv.wangdashe.top

[D23] reduce 累积计算
来源：http://tlg.ctjpmb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://orj.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xnh.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qqj.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jmr.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://ekk.bjfxy.top

Go:   // 手写循环
来源：http://hdc.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ivz.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://znc.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://vqj.ydjk.org.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ocg.andypj.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uyn.yanxiufei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://llz.gzhubu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lva.nanxuanxn.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kfj.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uns.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kei.0kj1m.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lvt.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://oua.yvedp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uqd.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vvd.yj20258888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nzt.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ygh.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zkn.9152youxi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fdw.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uhp.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xkr.jqgfzy.top

[D26] 数组转字符串
来源：http://iex.yj20258.top

Py:   ", ".join(map(str, arr))
来源：http://dqf.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://gqn.gotoacloud.top

JS:   arr.join(", ")
来源：http://epz.smart0.xyz

TS:   arr.join(", ")
来源：http://ifm.jiagoushi.top

Java: String.join(", ", list)
来源：http://gut.ctjpmb.com

Go:   strings.Join(strs, ", ")
来源：http://fpj.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://bsm.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://xtd.bjfxy.top

================================================================================
来源：http://brl.xinyue.icu

E. 字符串处理
来源：http://wkz.yj20258.top

================================================================================
来源：http://bfu.pengpengdd.cyou

[E01] 拼接字符串
来源：http://kul.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://egy.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tvo.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oya.yanxiufei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zgp.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kxd.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fgd.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dkr.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kid.wangdashe.top

[E02] 重复字符串
来源：http://zaj.yj20258.top

Py:   "ab" * 3
来源：http://syl.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://iuh.316326.xyz

JS:   "ab".repeat(3)
来源：http://bpn.ivvv.top

TS:   "ab".repeat(3)
来源：http://voc.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://uuy.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://qgn.nanxuanxn.top

Ruby: "ab" * 3
来源：http://msj.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ams.cdnleiting.top

[E03] 截取子串
来源：http://tqp.fzhhl.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ybt.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://urc.jinghuilouyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xzx.zhixingplan.top

TS:   s.slice(1, 4)
来源：http://rth.zdqjudy.top

Java: s.substring(1, 4)
来源：http://yzr.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://axk.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://efr.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://zhp.svipenyu.cn

[E04] 查找子串位置
来源：http://vhh.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://jxw.316326.xyz

PHP:  strpos($s, "x");
来源：http://etx.tanke756.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jnx.hfpthk.cn

TS:   s.indexOf("x")
来源：http://rql.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://qoi.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://dmz.zdqjudy.top

Ruby: s.index("x")
来源：http://kej.redwolf501.top

C#:   s.IndexOf("x")
来源：http://zse.shuidangran.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wjm.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tqk.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esr.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zmc.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ybk.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgs.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ood.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fum.9152youxi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ddm.xingfuxueyuan.xyz

[E06] 替换子串
来源：http://vqe.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vhn.aizwys.cn

PHP:  str_replace("a", "b", $s);
来源：http://pij.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://izf.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://oae.zhongyouzk.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ixo.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xnt.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gfs.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://bvq.havefunace.top

[E07] 按分隔符拆分
来源：http://eau.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jds.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvq.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lqv.daria6918.cn

TS:   s.split(",")
来源：http://vdt.zhengqikj.top

Java: s.split(",");  s.split("\\s+")
来源：http://emt.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rqq.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://bug.tianlin.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sxv.hesvh.cn

[E08] 数组按分隔符合并
来源：http://dcl.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://ghp.zhijiandao.cn

PHP:  implode(",", $items);
来源：http://zvg.tarul.cn

JS:   items.join(",")
来源：http://nhs.chenzaomai.com

TS:   items.join(",")
来源：http://iah.svipenyu.cn

Java: String.join(",", items)
来源：http://rmz.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://dku.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://qjn.fzhhl.top

C#:   string.Join(",", items)
来源：http://dun.xziqi.cn

[E09] 去除所有空白字符
来源：http://dis.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://onz.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wuw.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://qcs.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://udb.andypj.xyz

Java: s.replaceAll("\\s+", "")
来源：http://jki.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kxj.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://qwb.xinyue.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ofk.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://qmp.sjlbkw.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ala.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mer.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://slt.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://hed.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://fpo.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jmf.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nwk.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rcp.c1oappe.top

[E11] 反转字符串
来源：http://goi.dashuyun.cn

Py:   s[::-1]
来源：http://bkf.jyoumei.cn

PHP:  strrev($s);
来源：http://yta.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://szb.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://qdc.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jav.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://owk.jqgufenzy.top

Ruby: s.reverse
来源：http://dhu.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://rse.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://qup.gotoacloud.top

Py:   s.count("a")
来源：http://gsq.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://oyl.yj202588.top

JS:   s.split("a").length - 1
来源：http://eyi.ybcxt.top

TS:   s.split("a").length - 1
来源：http://ifb.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dxp.sufxvd.cn

Go:   strings.Count(s, "a")
来源：http://fbe.zhiwuduotai.top

Ruby: s.count("a")
来源：http://cau.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://mhc.aibaodan.cn

[E13] 逐字符遍历
来源：http://ooi.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://zub.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pqo.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hde.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ypc.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yoc.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uax.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wcj.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://upg.cucudq.cn

[E14] URL 编码与 Base64
来源：http://lzk.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xdd.ivvv.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zrq.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://afq.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rea.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bhb.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ipm.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cbx.xinyue.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qni.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://xap.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://san.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyp.fktsv.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cdw.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jkl.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fjt.guowangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nbd.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tym.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oca.aizwys.cn

[E16] 数字千分位
来源：http://phw.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://iwe.sysykeji.top

PHP:  number_format(1234567);
来源：http://fsf.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tmu.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ymr.c1oappe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ndn.tian-w.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mex.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ycv.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://zud.aizwys.cn

[E17] 首字母大写
来源：http://aud.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bzw.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://flz.vqdsnc.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://apw.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tnl.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xxm.dianchejie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tby.hammf.cn

Ruby: s.capitalize
来源：http://nyz.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://axj.tianlin.xyz

[E18] 模板占位符替换
来源：http://oqq.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vji.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rxg.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rqh.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jhy.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xba.zhoulong.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blj.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rfs.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pmv.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://fgr.sxryk.cn

Py:   s.splitlines()
来源：http://rvi.dianchejie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mai.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://kgv.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://kzk.ehwqpu.com

Java: s.lines().toList()
来源：http://xes.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://tov.xziqi.cn

Ruby: s.lines
来源：http://ylq.nanxuanxn.top

C#:   s.Split('\n')
来源：http://cxh.tanke756.top

[E20] 判断字符串是否为空
来源：http://jou.hesvh.cn

Py:   if not s:
来源：http://lez.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bmm.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aag.daria6918.cn

TS:   if (s === "") {}
来源：http://dvl.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://dsp.daria6918.cn

Go:   if s == "" {}
来源：http://nfy.aibaodan.cn

Ruby: if s.empty?
来源：http://zhd.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://umm.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://lwn.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gkp.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qfv.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pcj.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycx.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nxj.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://hyt.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yxd.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zdi.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://spp.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mvs.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mkl.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbz.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rur.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hqk.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lgu.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://oix.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mkn.shuidangran.top

================================================================================
来源：http://kse.mhx1999.top

F. 文件与目录
来源：http://amr.sxryk.cn

================================================================================
来源：http://kcv.chenlongwang.top

[F01] 读取整个文件
来源：http://hdz.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ebo.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://alh.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wjm.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://njb.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hdw.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rbk.fehbvm.com

Ruby: File.read("a.txt")
来源：http://nsy.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://yue.kuanghao11.cn

[F02] 逐行读取文件
来源：http://jja.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://avp.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qms.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ham.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rpa.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://icu.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fpm.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bdl.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uyu.yonumen.top

[F03] 写入文件（覆盖）
来源：http://slv.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rtz.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jhf.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jbv.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izu.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tys.hfpthk.cn


<!-- 参考信息 -->