代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mrt.shangyingyoupin.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzn.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jko.bjfxy.top

Go:   // 手写循环累加
来源：http://jgq.zhongyouzk.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uqn.tanke756.top

C#:   list.Sum();  list.Average()
来源：http://jqu.guowangkeji.top

[D17] 最大值与最小值
来源：http://ymy.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://yen.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://npc.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ayq.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://iyb.cucudq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lgv.zhixingplan.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hpf.mhx1999.top

Ruby: arr.max;  arr.min
来源：http://ajn.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://cax.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://xua.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nmy.xylfe.cn

PHP:  array_merge(...$nested);
来源：http://wfp.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yoa.ehwqpu.com

TS:   nested.flat();
来源：http://rty.yueranfly.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://opc.snrcjt.cn

Go:   // 手写双层循环
来源：http://mlb.shangyingyoupin.top

Ruby: nested.flatten
来源：http://tzi.xuanzx.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://xlp.tian-w.cn

[D19] 按字段分组
来源：http://tnu.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wow.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ctv.gogol.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kil.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wkn.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ior.andypj.xyz

Go:   // 手写 map[string][]T
来源：http://zmn.hesvh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://evw.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yoc.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://gpi.yonumen.top

Py:   Counter(arr)
来源：http://lrt.guannengcc.top

PHP:  array_count_values($arr);
来源：http://cur.fanxiaobao.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ucj.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lgl.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sxo.epnwcf.com

Go:   // 手写 map[T]int
来源：http://myi.jianghu66.top

Ruby: arr.tally
来源：http://uzk.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jvw.nwbrower.top

[D21] 判断是否包含某元素
来源：http://nno.yonumen.top

Py:   x in arr
来源：http://xrx.yueranfly.top

PHP:  in_array($x, $arr, true);
来源：http://kyp.guannengcc.top

JS:   arr.includes(x)
来源：http://cwx.jianghu66.top

TS:   arr.includes(x)
来源：http://iuc.jyoumei.cn

Java: list.contains(x)
来源：http://xrn.zdbjq.cn

Go:   slices.Contains(arr, x)
来源：http://rsx.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://knb.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://tkm.aizwys.cn

[D22] 复制数组（避免共享引用）
来源：http://jvp.haohaochexian.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fel.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tqs.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mqy.chenjidiqi.icu

TS:   [...arr];
来源：http://upz.dianchejie.cn

Java: new ArrayList<>(list);
来源：http://qnr.ivvv.top

Go:   copied := append([]int(nil), arr...)
来源：http://hbk.shzxlz.cn

Ruby: arr.dup;  arr.clone
来源：http://yud.guannengcc.top

C#:   new List<int>(list);
来源：http://zzw.pycfn.com

[D23] reduce 累积计算
来源：http://raj.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zgb.sjlbkw.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mhz.jiagoushi.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lbt.gotoacloud.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mdc.daxiang520.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wee.hesvh.cn

Go:   // 手写循环
来源：http://qhh.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mdi.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dug.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://wrt.iojbl.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hdf.daria6918.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qtf.yangfankeji.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gvp.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gcu.smart0.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://exc.fengsongda.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ihz.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://clp.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xzx.xziqi.cn

[D25] Set 集合去重与交并差
来源：http://dyn.nanxinkj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://twl.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://waq.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tbk.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cuw.xuanzx.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fde.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wsw.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hem.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kta.bbcook.cn

[D26] 数组转字符串
来源：http://hkj.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://mrx.nwbrower.top

PHP:  implode(", ", $arr);
来源：http://mss.hcnkem.com

JS:   arr.join(", ")
来源：http://xwh.gotoacloud.top

TS:   arr.join(", ")
来源：http://ben.epnwcf.com

Java: String.join(", ", list)
来源：http://voh.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://evx.zhoulong.xyz

Ruby: arr.join(", ")
来源：http://tgy.daria6918.cn

C#:   string.Join(", ", list)
来源：http://omg.pycfn.com

================================================================================
来源：http://fcn.shanyushiyangtech.top

E. 字符串处理
来源：http://dpd.ctjpmb.com

================================================================================
来源：http://kcr.hcnkem.com

[E01] 拼接字符串
来源：http://xqt.9152youxi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://avo.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cvg.nanxinkj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://asf.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://idk.fengsongda.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hig.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wet.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ydi.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zcq.ehwqpu.com

[E02] 重复字符串
来源：http://ddp.wangshuangyany.cn

Py:   "ab" * 3
来源：http://jto.shzxlz.cn

PHP:  str_repeat("ab", 3);
来源：http://qwx.ppjwa.cn

JS:   "ab".repeat(3)
来源：http://ktd.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://bcq.bjfxy.top

Java: "ab".repeat(3)
来源：http://gsn.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://zaa.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://bqq.wangdashe.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pgx.mhx1999.top

[E03] 截取子串
来源：http://mxc.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iec.hesvh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vai.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xzt.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://wlg.ehwqpu.com

Java: s.substring(1, 4)
来源：http://var.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mhr.chenlongwang.top

Ruby: s[1, 3];  s[1..3]
来源：http://hyz.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://avh.bbcook.cn

[E04] 查找子串位置
来源：http://gzz.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://qvl.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://lfx.xuetiantiany.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mzl.c1oappe.top

TS:   s.indexOf("x")
来源：http://jxr.gogol.net.cn

Java: s.indexOf("x")
来源：http://pav.jinqigfzy.top

Go:   strings.Index(s, "x")
来源：http://dwo.tian-w.cn

Ruby: s.index("x")
来源：http://uym.nwbrower.top

C#:   s.IndexOf("x")
来源：http://dpz.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ofw.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vgj.kuanghao11.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cju.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://abl.xuanzx.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://fjn.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qut.gaohongyu789.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://plm.jyoumei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iky.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://acj.yongpay.top

[E06] 替换子串
来源：http://pwq.yvedp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbo.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://pka.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zmx.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://izx.meibo888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mxg.zdqjudy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jcu.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qrl.tarul.cn

C#:   s.Replace("a", "b")
来源：http://djq.cashguo.top

[E07] 按分隔符拆分
来源：http://mxy.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fnw.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cst.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rxy.xylfe.cn

TS:   s.split(",")
来源：http://asl.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://rci.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zmt.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://sfh.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vye.daria6918.cn

[E08] 数组按分隔符合并
来源：http://wxf.hesvh.cn

Py:   ",".join(items)
来源：http://bvl.aizwys.cn

PHP:  implode(",", $items);
来源：http://kkq.sxryk.cn

JS:   items.join(",")
来源：http://cjv.0kj1m.cn

TS:   items.join(",")
来源：http://paf.daria6918.cn

Java: String.join(",", items)
来源：http://nnl.daxiang520.top

Go:   strings.Join(items, ",")
来源：http://jku.redwolf501.top

Ruby: items.join(",")
来源：http://eql.fzhhl.top

C#:   string.Join(",", items)
来源：http://zdm.jinqigufen.top

[E09] 去除所有空白字符
来源：http://kyh.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://htb.hfpthk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zlb.fehbvm.com

JS:   s.replace(/\s+/g, "")
来源：http://svx.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://ymn.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://nog.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://omr.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://tei.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ymp.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://mcq.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://udv.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yjc.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://jmx.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://nld.yangfankeji.com

Java: String.format("%03d", 7)
来源：http://ugn.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xlo.bjfxy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://elv.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rwa.pycfn.com

[E11] 反转字符串
来源：http://pnp.wangshuangyany.cn

Py:   s[::-1]
来源：http://mvo.zdbjq.cn

PHP:  strrev($s);
来源：http://tqo.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://qdj.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://fab.bjfxy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ptl.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://krb.nanxuanxn.top

Ruby: s.reverse
来源：http://vyc.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://opx.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://lfu.jyoumei.cn

Py:   s.count("a")
来源：http://qbm.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://pbx.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://pha.zycfv.cn

TS:   s.split("a").length - 1
来源：http://jhz.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ylv.uphjek.com

Go:   strings.Count(s, "a")
来源：http://nhk.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://bqq.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://vqu.fktsv.cn

[E13] 逐字符遍历
来源：http://mhh.hammf.cn

Py:   for ch in s: print(ch)
来源：http://hbi.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blo.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tui.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lxt.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zux.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xbl.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://okj.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eub.dianchejie.cn

[E14] URL 编码与 Base64
来源：http://ukb.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qmn.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rzw.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vqm.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vnh.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ezm.vehdjk.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://itp.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://raf.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wys.xziqi.cn

[E15] HTML 转义 / 反转义
来源：http://yes.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://zzb.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xzk.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://izl.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uuw.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xym.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ont.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zfr.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fpq.svipenyu.cn

[E16] 数字千分位
来源：http://xsr.tarul.cn

Py:   f"{1234567:,}"
来源：http://cro.cucudq.cn

PHP:  number_format(1234567);
来源：http://pfm.wangdashe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xqv.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ykh.tianlin.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://okn.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://soo.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dye.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://kkh.tanke756.top

[E17] 首字母大写
来源：http://ldc.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://utv.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sdf.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rgb.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://otz.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mwj.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xgo.jlsjyb.cn

Ruby: s.capitalize
来源：http://tqi.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jnp.xinyue.icu

[E18] 模板占位符替换
来源：http://akj.xylfe.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lmm.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qgm.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://onl.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://izk.jyoumei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ace.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lpj.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://btt.aibaodan.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gsp.fktsv.cn

[E19] 多行文本按行拆分
来源：http://nau.yj20258888.top

Py:   s.splitlines()
来源：http://gwg.zhoulong.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kaj.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://irs.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://aea.uphjek.com

Java: s.lines().toList()
来源：http://dzd.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://hbg.hywenlv.cn

Ruby: s.lines
来源：http://gjz.jinqigufen.top

C#:   s.Split('\n')
来源：http://wfc.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://pzw.chenjidiqi.icu

Py:   if not s:
来源：http://aqo.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zqw.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aix.gaohongyu789.top

TS:   if (s === "") {}
来源：http://qxx.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://dux.shuidangran.top

Go:   if s == "" {}
来源：http://lja.jlsjyb.cn

Ruby: if s.empty?
来源：http://atl.zycfv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uib.jianghu66.top

[E21] 超长截断加省略号
来源：http://hel.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mnb.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iiy.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aiq.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ron.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mng.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://vvy.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jrs.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jtp.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://xqv.havefunace.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uoo.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://njn.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bsa.yuanzhike.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nmf.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jvj.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iyo.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://fwn.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ifu.hywenlv.cn

================================================================================
来源：http://rfb.vqdsnc.cn

F. 文件与目录
来源：http://hec.epnwcf.com

================================================================================
来源：http://rmz.yj202588.top


<!-- 参考信息 -->