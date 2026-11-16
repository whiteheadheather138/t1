代发 wailian999

C#:   list.Distinct().ToList()
来源：http://ufi.ivvv.top

[D16] 求和与平均值
来源：http://onu.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fzb.epnwcf.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mmh.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qwb.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ows.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mjx.mhx1999.top

Go:   // 手写循环累加
来源：http://kzd.chenlongwang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kpc.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://zgf.jianghu66.top

[D17] 最大值与最小值
来源：http://inn.yj20258.top

Py:   max(arr);  min(arr)
来源：http://ese.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://czr.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mvq.xinyue.icu

TS:   Math.max(...arr);
来源：http://mrf.zhaomingkeji.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://qxi.zycfv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ddv.c1oappe.top

Ruby: arr.max;  arr.min
来源：http://meu.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://dxv.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://lvf.gotoacloud.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pzx.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://ycp.xziqi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mbk.redwolf501.top

TS:   nested.flat();
来源：http://ayf.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hfc.sufxvd.cn

Go:   // 手写双层循环
来源：http://jsa.chenzaomai.com

Ruby: nested.flatten
来源：http://ypf.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://ozr.fehbvm.com

[D19] 按字段分组
来源：http://ewt.yongpay.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pvy.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://law.quarkkingdee.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tzg.cashguo.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://fig.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qjh.cheryme.top

Go:   // 手写 map[string][]T
来源：http://dyt.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sre.9152youxi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rwo.vehdjk.com

[D20] 统计每个元素出现次数
来源：http://zqa.jinqigufen.top

Py:   Counter(arr)
来源：http://oog.pengpengdd.cyou

PHP:  array_count_values($arr);
来源：http://odb.jinyuanbaomall.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sos.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mji.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dnu.nanxinkj.top

Go:   // 手写 map[T]int
来源：http://xcq.cqqwz.cn

Ruby: arr.tally
来源：http://hcb.gaohongyu789.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pfl.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://efk.ybcxt.top

Py:   x in arr
来源：http://pma.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://mfm.pycfn.com

JS:   arr.includes(x)
来源：http://fuc.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://sxt.shanyushiyangtech.top

Java: list.contains(x)
来源：http://ypn.dianchejie.cn

Go:   slices.Contains(arr, x)
来源：http://qtv.sysykeji.top

Ruby: arr.include?(x)
来源：http://nnf.dianchejie.cn

C#:   list.Contains(x)
来源：http://lyk.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://qfw.nanxinkj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wxs.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hnz.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fje.sysykeji.top

TS:   [...arr];
来源：http://xtp.vehdjk.com

Java: new ArrayList<>(list);
来源：http://rkw.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rte.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://qan.cqqwz.cn

C#:   new List<int>(list);
来源：http://fkg.svipenyu.cn

[D23] reduce 累积计算
来源：http://yun.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://myk.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fda.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cdz.haohaochexian.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vyi.nanxuanxn.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ana.jinghuilouyu.cn

Go:   // 手写循环
来源：http://uvd.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dve.shangyingyoupin.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zlu.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://ccw.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hnn.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zyc.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://joj.zdbjq.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://myu.mhx1999.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://itn.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://njz.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xbk.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qtw.epnwcf.com

[D25] Set 集合去重与交并差
来源：http://ojy.zhijiandao.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dye.zhengqikj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eva.yj202588.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jii.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://smm.chenjidiqi.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vvt.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mnz.guannengcc.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kcx.pengpengdd.cyou

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://opr.sufxvd.cn

[D26] 数组转字符串
来源：http://cqz.yueranfly.top

Py:   ", ".join(map(str, arr))
来源：http://irb.shanyushiyangtech.top

PHP:  implode(", ", $arr);
来源：http://icz.bbcook.cn

JS:   arr.join(", ")
来源：http://dbo.hywenlv.cn

TS:   arr.join(", ")
来源：http://kya.yueranfly.top

Java: String.join(", ", list)
来源：http://omx.xingfuxueyuan.xyz

Go:   strings.Join(strs, ", ")
来源：http://tdy.fzhhl.top

Ruby: arr.join(", ")
来源：http://mdu.hongshengwenyu.top

C#:   string.Join(", ", list)
来源：http://idg.yonumen.top

================================================================================
来源：http://azt.epnwcf.com

E. 字符串处理
来源：http://sqi.cheryme.top

================================================================================
来源：http://ijm.hnqzz.top

[E01] 拼接字符串
来源：http://yss.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tnx.mhx1999.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://knw.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ang.ybcxt.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sgr.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://asq.c1oappe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fbn.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://irw.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://exq.xuetiantiany.cn

[E02] 重复字符串
来源：http://ikz.yuanzhike.top

Py:   "ab" * 3
来源：http://pxz.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://ake.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://fyc.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://wid.cdnleiting.top

Java: "ab".repeat(3)
来源：http://gmr.hcnkem.com

Go:   strings.Repeat("ab", 3)
来源：http://qix.yj20258.top

Ruby: "ab" * 3
来源：http://uws.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vvh.zhiwuduotai.top

[E03] 截取子串
来源：http://upy.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pds.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ivr.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lcj.yongpay.top

TS:   s.slice(1, 4)
来源：http://myj.tarul.cn

Java: s.substring(1, 4)
来源：http://pct.yanxiufei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rov.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sfg.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://kuv.jqgfzy.top

[E04] 查找子串位置
来源：http://gkh.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://abk.yonumen.top

PHP:  strpos($s, "x");
来源：http://jbi.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cnt.zycfv.cn

TS:   s.indexOf("x")
来源：http://cpe.aizwys.cn

Java: s.indexOf("x")
来源：http://nbd.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://flg.hesvh.cn

Ruby: s.index("x")
来源：http://bvu.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://ylv.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qnf.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kdx.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tql.daxiang520.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tja.meibo888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wfg.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vpw.hysaishi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ikz.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://svl.xziqi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yjl.sysykeji.top

[E06] 替换子串
来源：http://saq.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ajv.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://lvi.zdqjudy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ctu.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://jyn.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jnc.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uas.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://flr.316326.xyz

C#:   s.Replace("a", "b")
来源：http://tox.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://usr.hongshengwenyu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tmr.wangdashe.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wpz.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://fzi.gzhubu.top

TS:   s.split(",")
来源：http://xkl.yonumen.top

Java: s.split(",");  s.split("\\s+")
来源：http://ueu.smart0.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ytt.yj20258.top

Ruby: s.split(",");  s.split
来源：http://izx.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://iam.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://qfg.sufxvd.cn

Py:   ",".join(items)
来源：http://mhc.mhx1999.top

PHP:  implode(",", $items);
来源：http://mfa.zhengqikj.top

JS:   items.join(",")
来源：http://efz.chenjidiqi.icu

TS:   items.join(",")
来源：http://vle.jiagoushi.top

Java: String.join(",", items)
来源：http://lyo.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://dwv.kuanghao11.cn

Ruby: items.join(",")
来源：http://mwr.yanxiufei.cn

C#:   string.Join(",", items)
来源：http://isl.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://nmh.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rir.ppjwa.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sea.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://imi.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://kur.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://nwq.shzxlz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fgi.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://zmm.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yzn.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://rew.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mup.xuetiantiany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xvo.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://jej.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://ugk.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://bqe.pycfn.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cfg.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jgq.hnqzz.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://brg.fehbvm.com

[E11] 反转字符串
来源：http://dei.cucudq.cn

Py:   s[::-1]
来源：http://asy.sufxvd.cn

PHP:  strrev($s);
来源：http://whh.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://res.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://tkg.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ksk.vehdjk.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://fdj.hnqzz.top

Ruby: s.reverse
来源：http://xqw.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://kga.daria6918.cn

[E12] 统计某字符出现次数
来源：http://mrl.chenzaomai.com

Py:   s.count("a")
来源：http://cjk.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://aws.bbcook.cn

JS:   s.split("a").length - 1
来源：http://uwv.gzhubu.top

TS:   s.split("a").length - 1
来源：http://nek.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://era.hcnkem.com

Go:   strings.Count(s, "a")
来源：http://ibv.tarul.cn

Ruby: s.count("a")
来源：http://vvn.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://yro.zhengqikj.top

[E13] 逐字符遍历
来源：http://ehi.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://lny.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vbe.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ivk.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rtb.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://smj.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iiv.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qlf.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qit.snrcjt.cn

[E14] URL 编码与 Base64
来源：http://cxm.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nay.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yyq.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tgr.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mrr.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://osc.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vnh.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ieh.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mze.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://beh.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://btn.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lnn.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://brq.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yll.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tqj.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ulw.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nbz.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tow.ydzc1.top

[E16] 数字千分位
来源：http://tok.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://jfm.fzhhl.top

PHP:  number_format(1234567);
来源：http://ksg.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xcx.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://sjp.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rxo.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzp.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cnc.vehdjk.com

C#:   1234567.ToString("N0")
来源：http://apz.hysaishi.cn

[E17] 首字母大写
来源：http://eyj.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://waj.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dul.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vvr.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kdt.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eia.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bgc.chenzaomai.com

Ruby: s.capitalize
来源：http://ggg.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bvl.zhoulong.xyz

[E18] 模板占位符替换
来源：http://wou.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jmu.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wfg.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cde.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dqj.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ggk.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jdl.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hjv.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ssd.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://bjs.nanxinkj.top

Py:   s.splitlines()
来源：http://ugi.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mxk.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://azi.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://jol.vqdsnc.cn

Java: s.lines().toList()
来源：http://saw.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://bsm.zhengqikj.top

Ruby: s.lines
来源：http://uko.ehwqpu.com

C#:   s.Split('\n')
来源：http://okp.hesvh.cn

[E20] 判断字符串是否为空
来源：http://gwu.cucudq.cn

Py:   if not s:
来源：http://nas.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bhy.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ume.shanyushiyangkeji.top

TS:   if (s === "") {}
来源：http://shx.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://kzq.xziqi.cn

Go:   if s == "" {}
来源：http://orz.yj20258.top

Ruby: if s.empty?
来源：http://upe.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://guc.yvedp.cn

[E21] 超长截断加省略号
来源：http://dbu.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fht.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qan.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dto.nanxinkj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zll.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nfc.shangyingyoupin.top

Go:   // 按 rune 判断长度后截断
来源：http://cxm.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jdd.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mma.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://yem.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qwq.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kae.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xig.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iyl.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://maj.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yqf.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://lzb.shangyingyoupin.top


<!-- 参考信息 -->