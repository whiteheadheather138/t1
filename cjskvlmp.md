代发 wailian999

[D19] 按字段分组
来源：http://hpo.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yel.shanyushiyangtech.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jac.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mng.dashuyun.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yqv.jinyuanbaomall.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eub.ivvv.top

Go:   // 手写 map[string][]T
来源：http://npj.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://sbs.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hwx.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://fvf.bbcook.cn

Py:   Counter(arr)
来源：http://rlk.xylfe.cn

PHP:  array_count_values($arr);
来源：http://vwu.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://udj.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rfy.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://brf.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://iqa.yj20258888.top

Ruby: arr.tally
来源：http://ntt.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://khy.ivvv.top

[D21] 判断是否包含某元素
来源：http://sfc.pengpengdd.cyou

Py:   x in arr
来源：http://sfp.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://dyy.iojbl.cn

JS:   arr.includes(x)
来源：http://tnf.yuxming.cn

TS:   arr.includes(x)
来源：http://nqb.chenlongwang.top

Java: list.contains(x)
来源：http://ysa.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://hze.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://adl.cashguo.top

C#:   list.Contains(x)
来源：http://cui.jinghuilouyu.cn

[D22] 复制数组（避免共享引用）
来源：http://wul.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ucr.snrcjt.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://czq.sufxvd.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ivu.zhixingplan.top

TS:   [...arr];
来源：http://jrn.guannengcc.top

Java: new ArrayList<>(list);
来源：http://nsq.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://cpb.cqqwz.cn

Ruby: arr.dup;  arr.clone
来源：http://ejo.mhx1999.top

C#:   new List<int>(list);
来源：http://hmj.mhx1999.top

[D23] reduce 累积计算
来源：http://upj.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wgd.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yri.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ued.ppjwa.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://evh.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://vpm.cheryme.top

Go:   // 手写循环
来源：http://rqm.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pkr.daria6918.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://grd.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://wmj.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://riq.zdbjq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nnx.kuanghao11.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lgv.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvv.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rmr.mhx1999.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dou.yanxiufei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zli.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xwc.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://zao.daxiang520.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hfm.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rss.fktsv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mxp.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uff.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vbb.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lyp.sufxvd.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hsj.jqgfzy.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tqj.sufxvd.cn

[D26] 数组转字符串
来源：http://csx.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://lrz.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://fea.yanxiufei.cn

JS:   arr.join(", ")
来源：http://fma.xuanzx.com

TS:   arr.join(", ")
来源：http://sqn.sweek.top

Java: String.join(", ", list)
来源：http://ctp.quarkkingdee.top

Go:   strings.Join(strs, ", ")
来源：http://ovg.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://hik.yuxming.cn

C#:   string.Join(", ", list)
来源：http://ioa.mhx1999.top

================================================================================
来源：http://fzb.sweek.top

E. 字符串处理
来源：http://mro.xziqi.cn

================================================================================
来源：http://pur.jinqigfzy.top

[E01] 拼接字符串
来源：http://gss.hcnkem.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uza.yj20258888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ktt.fzhhl.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://krg.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://izl.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kfy.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zcw.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ess.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzi.0kj1m.cn

[E02] 重复字符串
来源：http://pwt.bjfxy.top

Py:   "ab" * 3
来源：http://kbj.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://pjx.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://rgy.jianghu66.top

TS:   "ab".repeat(3)
来源：http://fpv.daria6918.cn

Java: "ab".repeat(3)
来源：http://tqi.jianghu66.top

Go:   strings.Repeat("ab", 3)
来源：http://ilc.guannengcc.top

Ruby: "ab" * 3
来源：http://eqd.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ycc.shangyingyoupin.top

[E03] 截取子串
来源：http://tfc.jyoumei.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xgg.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lgy.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hzn.yongpay.top

TS:   s.slice(1, 4)
来源：http://dbw.xuanzx.com

Java: s.substring(1, 4)
来源：http://nix.hywenlv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jrq.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://yco.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://pyu.iojbl.cn

[E04] 查找子串位置
来源：http://aba.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://rcq.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://tln.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dvl.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://tjb.aibaodan.cn

Java: s.indexOf("x")
来源：http://xyf.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://vdn.zdbjq.cn

Ruby: s.index("x")
来源：http://bas.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://dek.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ewt.sufxvd.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bar.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fig.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwu.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jpp.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yfg.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vvg.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lzf.daxiang520.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wvz.fktsv.cn

[E06] 替换子串
来源：http://yig.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://use.ydjk.org.cn

PHP:  str_replace("a", "b", $s);
来源：http://ndk.nanxinkj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hia.bbcook.cn

TS:   s.replaceAll("a", "b")
来源：http://fit.aizwys.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://edr.xingfuxueyuan.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gob.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://osn.jinqigufen.top

C#:   s.Replace("a", "b")
来源：http://ozj.cdnleiting.top

[E07] 按分隔符拆分
来源：http://gqy.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pha.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gwe.chenjidiqi.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://dyb.andypj.xyz

TS:   s.split(",")
来源：http://ecl.birdmap.top

Java: s.split(",");  s.split("\\s+")
来源：http://pfx.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bdn.aibaodan.cn

Ruby: s.split(",");  s.split
来源：http://rhy.wangshuangyany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oxd.fengsongda.top

[E08] 数组按分隔符合并
来源：http://rtu.nanxuanxn.top

Py:   ",".join(items)
来源：http://upc.ybcxt.top

PHP:  implode(",", $items);
来源：http://ihx.xuetiantiany.cn

JS:   items.join(",")
来源：http://skx.nanxinkj.top

TS:   items.join(",")
来源：http://xst.nwbrower.top

Java: String.join(",", items)
来源：http://goo.fengsongda.top

Go:   strings.Join(items, ",")
来源：http://byj.redwolf501.top

Ruby: items.join(",")
来源：http://iul.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://mck.cheryme.top

[E09] 去除所有空白字符
来源：http://mnl.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ckx.xziqi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://avn.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://jtm.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://nmf.cqqwz.cn

Java: s.replaceAll("\\s+", "")
来源：http://kib.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bjq.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cie.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fow.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://noq.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lfc.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://igm.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://zkt.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://rsv.fengsongda.top

Java: String.format("%03d", 7)
来源：http://gxp.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dtq.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ono.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pys.zhoulong.xyz

[E11] 反转字符串
来源：http://jsx.chenzaomai.com

Py:   s[::-1]
来源：http://urv.yfazqb.com

PHP:  strrev($s);
来源：http://pye.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://mqe.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://lhe.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dks.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gqo.gogol.net.cn

Ruby: s.reverse
来源：http://ysa.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://ulx.yj202588.top

[E12] 统计某字符出现次数
来源：http://rde.quarkkingdee.top

Py:   s.count("a")
来源：http://exh.pycfn.com

PHP:  substr_count($s, "a");
来源：http://mew.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://ceu.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://yvh.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rci.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://zun.ybcxt.top

Ruby: s.count("a")
来源：http://wtz.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://brc.cashguo.top

[E13] 逐字符遍历
来源：http://cgm.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://bzo.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jgm.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://saa.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://jfk.fzhhl.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kei.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xll.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pau.ppjwa.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yol.iojbl.cn

[E14] URL 编码与 Base64
来源：http://zqd.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zwm.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pzl.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ear.smart0.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aab.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ezg.sxryk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bvg.yonumen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uji.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jvy.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://hvt.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://mdf.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://chl.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fyt.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zhk.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jgz.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qwh.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hec.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jdu.pengpengdd.cyou

[E16] 数字千分位
来源：http://osc.guowangkeji.top

Py:   f"{1234567:,}"
来源：http://jmy.316326.xyz

PHP:  number_format(1234567);
来源：http://oce.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://fjh.chenjidiqi.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://acd.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxq.chenlongwang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wpo.andypj.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hfs.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://boe.shuidangran.top

[E17] 首字母大写
来源：http://kkf.wangshuangyany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://spt.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pas.wangshuangyany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yfp.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://prk.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fkr.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lvm.mhx1999.top

Ruby: s.capitalize
来源：http://mtc.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lxo.jianghu66.top

[E18] 模板占位符替换
来源：http://yfv.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://snm.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://muh.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://loa.hesvh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uxm.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xha.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kra.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hgx.hfpthk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://htw.yfazqb.com

[E19] 多行文本按行拆分
来源：http://wkc.hongshengwenyu.top

Py:   s.splitlines()
来源：http://njg.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xeb.jinqigfzy.top

JS:   s.split(/\r?\n/)
来源：http://kil.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://nyx.guannengcc.top

Java: s.lines().toList()
来源：http://glr.zhijiandao.cn

Go:   strings.Split(s, "\n")
来源：http://bbz.shzxlz.cn

Ruby: s.lines
来源：http://ryb.tian-w.cn

C#:   s.Split('\n')
来源：http://jbm.redwolf501.top

[E20] 判断字符串是否为空
来源：http://kmx.gotoacloud.top

Py:   if not s:
来源：http://vgo.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cyl.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ldt.zhijiandao.cn

TS:   if (s === "") {}
来源：http://weh.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://bix.gogol.net.cn

Go:   if s == "" {}
来源：http://qxk.mhx1999.top

Ruby: if s.empty?
来源：http://vmh.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qsf.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://tlz.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hzk.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ytv.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ypj.ppjwa.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gcw.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gbu.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://fhz.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://viz.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pqk.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://hmd.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fik.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjt.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cmr.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pyj.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lfe.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gia.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://awi.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sgq.zhengqikj.top

================================================================================
来源：http://gdn.shuidangran.top

F. 文件与目录
来源：http://ehz.jyoumei.cn

================================================================================
来源：http://hdz.vqdsnc.cn

[F01] 读取整个文件
来源：http://xuo.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ltg.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://kxw.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bxw.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hpj.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://tzj.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ysq.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://bjb.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://nck.bbcook.cn

[F02] 逐行读取文件
来源：http://pwd.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pbg.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ziw.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aak.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xbf.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhd.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://psn.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nza.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ymw.jinghuilouyu.cn

[F03] 写入文件（覆盖）
来源：http://uzt.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bjm.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://haq.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://poh.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjx.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jry.guowangkeji.top


<!-- 参考信息 -->