代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://keh.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://psa.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ibc.ehwqpu.com

Go:   // 手写循环累加
来源：http://lbi.gogol.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://irv.hcnkem.com

C#:   list.Sum();  list.Average()
来源：http://lox.zhongyouzk.top

[D17] 最大值与最小值
来源：http://wqi.zhongyouzk.top

Py:   max(arr);  min(arr)
来源：http://yjt.yuxming.cn

PHP:  max($arr);  min($arr);
来源：http://bvv.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ipk.hesvh.cn

TS:   Math.max(...arr);
来源：http://zmx.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://elj.fehbvm.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vkv.meibo888.top

Ruby: arr.max;  arr.min
来源：http://jaw.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://png.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://iom.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hra.birdmap.top

PHP:  array_merge(...$nested);
来源：http://exa.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://weu.fktsv.cn

TS:   nested.flat();
来源：http://awa.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rqk.cqqwz.cn

Go:   // 手写双层循环
来源：http://ttg.yanxiufei.cn

Ruby: nested.flatten
来源：http://twy.yongpay.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yjb.zdbjq.cn

[D19] 按字段分组
来源：http://nby.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pqd.jinghuilouyu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lof.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vqv.jinqigfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://poe.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jvl.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://ahn.316326.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://apw.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pvv.yfazqb.com

[D20] 统计每个元素出现次数
来源：http://wov.jinghuilouyu.cn

Py:   Counter(arr)
来源：http://dba.hesvh.cn

PHP:  array_count_values($arr);
来源：http://jpi.snrcjt.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tlu.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hcp.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uwp.fehbvm.com

Go:   // 手写 map[T]int
来源：http://myz.nwbrower.top

Ruby: arr.tally
来源：http://wak.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vse.hnqzz.top

[D21] 判断是否包含某元素
来源：http://rpa.yuxming.cn

Py:   x in arr
来源：http://qll.hysaishi.cn

PHP:  in_array($x, $arr, true);
来源：http://fwp.gogol.net.cn

JS:   arr.includes(x)
来源：http://ccx.cdnleiting.top

TS:   arr.includes(x)
来源：http://ltu.yuxming.cn

Java: list.contains(x)
来源：http://bsn.shanyushiyangtech.top

Go:   slices.Contains(arr, x)
来源：http://wtv.hcnkem.com

Ruby: arr.include?(x)
来源：http://cjb.zdbjq.cn

C#:   list.Contains(x)
来源：http://cxb.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://uol.wangshuangyany.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://unc.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://azj.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wsq.cashguo.top

TS:   [...arr];
来源：http://btz.uphjek.com

Java: new ArrayList<>(list);
来源：http://mfp.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://qie.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://cui.fehbvm.com

C#:   new List<int>(list);
来源：http://yap.birdmap.top

[D23] reduce 累积计算
来源：http://rpx.andypj.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://msk.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mgs.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aan.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wev.redwolf501.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wtp.sjlbkw.cn

Go:   // 手写循环
来源：http://cqf.haohaochexian.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bpz.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wjs.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://wql.smart0.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jpe.fktsv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://euv.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sew.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://csl.jinqigfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vaf.fzhhl.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xwg.guannengcc.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bkd.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fds.yongpay.top

[D25] Set 集合去重与交并差
来源：http://tnr.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aef.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qwf.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ftn.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qpf.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xvq.vehdjk.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gjo.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kqk.xinyue.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aib.wangdashe.top

[D26] 数组转字符串
来源：http://ces.hnqzz.top

Py:   ", ".join(map(str, arr))
来源：http://xkp.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://xrt.cdnleiting.top

JS:   arr.join(", ")
来源：http://lyl.xziqi.cn

TS:   arr.join(", ")
来源：http://fsv.cqqwz.cn

Java: String.join(", ", list)
来源：http://aii.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://pxf.zhengqikj.top

Ruby: arr.join(", ")
来源：http://nil.cucudq.cn

C#:   string.Join(", ", list)
来源：http://xfl.ehwqpu.com

================================================================================
来源：http://lyf.chenzaomai.com

E. 字符串处理
来源：http://vpk.daria6918.cn

================================================================================
来源：http://oiy.xziqi.cn

[E01] 拼接字符串
来源：http://tog.uphjek.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vfs.haohaochexian.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ltg.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vhr.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://itc.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mjx.jyoumei.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bxd.cheryme.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lqk.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pjj.sysykeji.top

[E02] 重复字符串
来源：http://zvf.yfazqb.com

Py:   "ab" * 3
来源：http://kic.wangshuangyany.cn

PHP:  str_repeat("ab", 3);
来源：http://pek.tanke756.top

JS:   "ab".repeat(3)
来源：http://ajd.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://jah.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://frx.sxryk.cn

Go:   strings.Repeat("ab", 3)
来源：http://lub.daxiang520.top

Ruby: "ab" * 3
来源：http://chn.dianchejie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://maj.zhijiandao.cn

[E03] 截取子串
来源：http://taf.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://njh.haohaochexian.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tst.316326.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jld.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://bex.yuxming.cn

Java: s.substring(1, 4)
来源：http://diu.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qai.jinqigfzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://tvw.bbcook.cn

C#:   s.Substring(1, 3)
来源：http://gfw.yuanzhike.top

[E04] 查找子串位置
来源：http://zgf.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://lgn.mhx1999.top

PHP:  strpos($s, "x");
来源：http://aid.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oba.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://abm.bbcook.cn

Java: s.indexOf("x")
来源：http://cfx.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://fue.xinyue.icu

Ruby: s.index("x")
来源：http://nji.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://pjt.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nwz.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ffl.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iwi.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nde.redwolf501.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gnh.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mpj.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bhq.cucudq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rdf.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xuq.zycfv.cn

[E06] 替换子串
来源：http://xpy.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qll.jinghuilouyu.cn

PHP:  str_replace("a", "b", $s);
来源：http://zvu.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://odz.zhijiandao.cn

TS:   s.replaceAll("a", "b")
来源：http://cjl.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lwi.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fap.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ntc.zhongyouzk.top

C#:   s.Replace("a", "b")
来源：http://azi.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://hms.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://udo.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rmh.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://nqr.tanke756.top

TS:   s.split(",")
来源：http://are.bbcook.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bky.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fww.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://oet.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zrg.zycfv.cn

[E08] 数组按分隔符合并
来源：http://mry.fengsongda.top

Py:   ",".join(items)
来源：http://xnq.cashguo.top

PHP:  implode(",", $items);
来源：http://kbi.xylfe.cn

JS:   items.join(",")
来源：http://xqa.yuanzhike.top

TS:   items.join(",")
来源：http://yrs.epnwcf.com

Java: String.join(",", items)
来源：http://dcf.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://kpx.gotoacloud.top

Ruby: items.join(",")
来源：http://byz.zdbjq.cn

C#:   string.Join(",", items)
来源：http://vsd.zhixingplan.top

[E09] 去除所有空白字符
来源：http://you.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yfa.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rqp.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://rwp.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://veu.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://qto.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lfj.yvedp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://byl.52xcode.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://exw.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://sry.zhiwuduotai.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://djo.zycfv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rby.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://jgr.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://abg.hnxiangtu.top

Java: String.format("%03d", 7)
来源：http://jjz.gotoacloud.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://owo.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nup.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hqv.daria6918.cn

[E11] 反转字符串
来源：http://nvj.zhengqikj.top

Py:   s[::-1]
来源：http://cuq.tarul.cn

PHP:  strrev($s);
来源：http://lgt.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://txu.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://ctu.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mkv.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fwv.xziqi.cn

Ruby: s.reverse
来源：http://dzg.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://hod.hesvh.cn

[E12] 统计某字符出现次数
来源：http://slj.jiagoushi.top

Py:   s.count("a")
来源：http://esx.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://ibz.cheryme.top

JS:   s.split("a").length - 1
来源：http://wor.jinyuanbaomall.cn

TS:   s.split("a").length - 1
来源：http://igy.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qeg.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://mpo.aibaodan.cn

Ruby: s.count("a")
来源：http://tln.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://zzi.birdmap.top

[E13] 逐字符遍历
来源：http://jln.haohaochexian.top

Py:   for ch in s: print(ch)
来源：http://yda.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://acj.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rob.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://tpy.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dnc.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sen.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://nep.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhw.yvedp.cn

[E14] URL 编码与 Base64
来源：http://ghn.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gkm.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ygu.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lts.iojbl.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fng.smart0.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lud.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bmn.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ryz.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zsy.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://gdq.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tcx.cucudq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wnh.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dfx.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iho.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://goj.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mmp.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yes.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hxc.meibo888.top

[E16] 数字千分位
来源：http://yfi.birdmap.top

Py:   f"{1234567:,}"
来源：http://jhn.yuxming.cn

PHP:  number_format(1234567);
来源：http://cep.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://cxd.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://med.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uxz.guannengcc.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vcb.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wqe.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://izz.epnwcf.com

[E17] 首字母大写
来源：http://vvn.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vfs.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://syn.sweek.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://efn.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfs.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wbo.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jhy.c1oappe.top

Ruby: s.capitalize
来源：http://tiu.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://myw.tianlin.xyz

[E18] 模板占位符替换
来源：http://mzx.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dky.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qhz.havefunace.top

JS:   tpl.replaceAll("{name}", name)
来源：http://khy.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wwf.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gpp.shanyushiyangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gfh.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://grn.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ypb.ehwqpu.com

[E19] 多行文本按行拆分
来源：http://qyy.nanxuanxn.top

Py:   s.splitlines()
来源：http://dzo.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nyt.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://bnr.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://nps.fktsv.cn

Java: s.lines().toList()
来源：http://hxe.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://kec.snrcjt.cn

Ruby: s.lines
来源：http://tmp.0kj1m.cn

C#:   s.Split('\n')
来源：http://kfe.xylfe.cn

[E20] 判断字符串是否为空
来源：http://tbe.chenzaomai.com

Py:   if not s:
来源：http://uqq.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zsr.316326.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmc.sysykeji.top

TS:   if (s === "") {}
来源：http://fnf.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://acl.jiagoushi.top

Go:   if s == "" {}
来源：http://fdm.yangfankeji.com

Ruby: if s.empty?
来源：http://xvf.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gpp.sufxvd.cn

[E21] 超长截断加省略号
来源：http://pbd.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vqj.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xjj.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gup.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmq.guannengcc.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://czl.dianchejie.cn

Go:   // 按 rune 判断长度后截断
来源：http://cqz.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fta.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xmn.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://xqj.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://syi.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmm.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sym.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jes.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lnc.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xpl.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://qoc.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wue.chenzaomai.com

================================================================================
来源：http://wcr.dianchejie.cn

F. 文件与目录
来源：http://njz.jyoumei.cn

================================================================================
来源：http://ohr.cqqwz.cn


<!-- 参考信息 -->