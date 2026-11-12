代发 wailian999

[D15] 去重
来源：http://xtx.316326.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zfd.shzxlz.cn

PHP:  array_unique($arr);
来源：http://met.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://sdx.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://okq.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://znn.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://eju.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://urs.yanxiufei.cn

C#:   list.Distinct().ToList()
来源：http://uwl.uphjek.com

[D16] 求和与平均值
来源：http://yqh.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cii.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zpr.shanyushiyangtech.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lmn.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ttz.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fwr.fengsongda.top

Go:   // 手写循环累加
来源：http://nye.fktsv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kdr.zhengqikj.top

C#:   list.Sum();  list.Average()
来源：http://umg.vqdsnc.cn

[D17] 最大值与最小值
来源：http://ofy.zdbjq.cn

Py:   max(arr);  min(arr)
来源：http://jwp.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://zcu.shzxlz.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ipw.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://mdm.xuetiantiany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://psd.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tgt.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://sth.guowangkeji.top

C#:   list.Max();  list.Min()
来源：http://yzn.yj202588.top

[D18] 扁平化嵌套数组
来源：http://nst.cheryme.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iof.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://iuo.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ggt.xinyue.icu

TS:   nested.flat();
来源：http://wpb.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xnm.c1oappe.top

Go:   // 手写双层循环
来源：http://gfn.feifeiyinyue.top

Ruby: nested.flatten
来源：http://vlm.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://git.ydzc1.top

[D19] 按字段分组
来源：http://skw.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ddu.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tlp.chenzaomai.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://obc.guowangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qug.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sio.uphjek.com

Go:   // 手写 map[string][]T
来源：http://uee.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mhw.hnxiangtu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hpi.ppjwa.cn

[D20] 统计每个元素出现次数
来源：http://jco.hysaishi.cn

Py:   Counter(arr)
来源：http://txa.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://enj.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lwi.meibo888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yia.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ocx.52xcode.cn

Go:   // 手写 map[T]int
来源：http://mit.chenlongwang.top

Ruby: arr.tally
来源：http://idg.aizwys.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rbn.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://znm.iojbl.cn

Py:   x in arr
来源：http://whz.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://lls.gzhubu.top

JS:   arr.includes(x)
来源：http://utq.jlsjyb.cn

TS:   arr.includes(x)
来源：http://ogn.hongshengwenyu.top

Java: list.contains(x)
来源：http://pwq.aizwys.cn

Go:   slices.Contains(arr, x)
来源：http://vei.guannengcc.top

Ruby: arr.include?(x)
来源：http://bwe.52xcode.cn

C#:   list.Contains(x)
来源：http://jrz.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://zsl.yonumen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://clv.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ctp.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nll.sysykeji.top

TS:   [...arr];
来源：http://mhe.cheryme.top

Java: new ArrayList<>(list);
来源：http://ycu.chenjidiqi.icu

Go:   copied := append([]int(nil), arr...)
来源：http://adp.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://fmt.zhoulong.xyz

C#:   new List<int>(list);
来源：http://kyo.fehbvm.com

[D23] reduce 累积计算
来源：http://tob.xziqi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uas.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uch.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qle.ydzc1.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iam.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zet.zycfv.cn

Go:   // 手写循环
来源：http://lne.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wdj.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://otb.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://zsr.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xxq.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cik.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zss.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lzq.tarul.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://elv.xylfe.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tij.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xeo.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blc.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://zft.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rvc.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gnu.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://koq.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bxc.fanxiaobao.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vmt.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iav.chenlongwang.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wdd.jiagoushi.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tfy.cucudq.cn

[D26] 数组转字符串
来源：http://evy.vehdjk.com

Py:   ", ".join(map(str, arr))
来源：http://kia.ehwqpu.com

PHP:  implode(", ", $arr);
来源：http://rbz.c1oappe.top

JS:   arr.join(", ")
来源：http://aic.ehwqpu.com

TS:   arr.join(", ")
来源：http://gyy.nanxuanxn.top

Java: String.join(", ", list)
来源：http://iax.svipenyu.cn

Go:   strings.Join(strs, ", ")
来源：http://ecx.cdnleiting.top

Ruby: arr.join(", ")
来源：http://hct.gzhubu.top

C#:   string.Join(", ", list)
来源：http://dwx.iojbl.cn

================================================================================
来源：http://deo.tarul.cn

E. 字符串处理
来源：http://bym.fengsongda.top

================================================================================
来源：http://mei.ehwqpu.com

[E01] 拼接字符串
来源：http://vov.c1oappe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ujw.gogol.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vul.ctjpmb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wjc.hywenlv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qvj.fanxiaobao.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qqo.cashguo.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cxt.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fck.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iss.chenjidiqi.icu

[E02] 重复字符串
来源：http://ktm.sufxvd.cn

Py:   "ab" * 3
来源：http://pxq.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://qwi.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://exw.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://iza.ctjpmb.com

Java: "ab".repeat(3)
来源：http://lhk.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://ojd.tanke756.top

Ruby: "ab" * 3
来源：http://yax.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zyz.jiagoushi.top

[E03] 截取子串
来源：http://bqn.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://klo.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cjh.hnxiangtu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oac.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://joj.epnwcf.com

Java: s.substring(1, 4)
来源：http://rqx.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xjb.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://rfa.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://fra.yuanzhike.top

[E04] 查找子串位置
来源：http://pzz.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://far.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://iqw.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qyg.cashguo.top

TS:   s.indexOf("x")
来源：http://qbx.fengsongda.top

Java: s.indexOf("x")
来源：http://oje.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://xwr.fktsv.cn

Ruby: s.index("x")
来源：http://fzv.sweek.top

C#:   s.IndexOf("x")
来源：http://njh.xuanzx.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://bhy.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://czm.yuxming.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://znk.hywenlv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wvi.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://orw.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rtg.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://elu.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vka.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rrb.hongshengwenyu.top

[E06] 替换子串
来源：http://xuf.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qxg.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://gey.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hno.xylfe.cn

TS:   s.replaceAll("a", "b")
来源：http://xnh.hesvh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ajn.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nra.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://thk.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://lkt.vehdjk.com

[E07] 按分隔符拆分
来源：http://eis.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://whq.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://czg.xingfuxueyuan.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xlj.jqgfzy.top

TS:   s.split(",")
来源：http://bgn.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pte.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dhf.hesvh.cn

Ruby: s.split(",");  s.split
来源：http://aqr.0kj1m.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rya.havefunace.top

[E08] 数组按分隔符合并
来源：http://tzm.chenjidiqi.icu

Py:   ",".join(items)
来源：http://bsk.xinyue.icu

PHP:  implode(",", $items);
来源：http://kxo.cqqwz.cn

JS:   items.join(",")
来源：http://fcg.ydzc1.top

TS:   items.join(",")
来源：http://juh.hnqzz.top

Java: String.join(",", items)
来源：http://chw.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://cyh.guannengcc.top

Ruby: items.join(",")
来源：http://ybj.pengpengdd.cyou

C#:   string.Join(",", items)
来源：http://ytn.zdqjudy.top

[E09] 去除所有空白字符
来源：http://bzs.tanke756.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yzv.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://djh.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://wai.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://whs.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://kxh.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://srf.redwolf501.top

Ruby: s.gsub(/\s+/, "")
来源：http://nnc.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yyq.feifeiyinyue.top

[E10] 左侧补零 / 定长填充
来源：http://bim.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cvs.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vit.gotoacloud.top

JS:   "7".padStart(3, "0")
来源：http://lbw.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://gon.mhx1999.top

Java: String.format("%03d", 7)
来源：http://ybk.uphjek.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ruy.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://piq.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bqr.xylfe.cn

[E11] 反转字符串
来源：http://goj.nwbrower.top

Py:   s[::-1]
来源：http://rii.xuetiantiany.cn

PHP:  strrev($s);
来源：http://cli.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://dwx.yj202588.top

TS:   [...s].reverse().join("")
来源：http://lbo.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mos.ydjk.org.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rkg.ydjk.org.cn

Ruby: s.reverse
来源：http://naq.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fhu.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://uti.yfazqb.com

Py:   s.count("a")
来源：http://bef.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://iev.ctjpmb.com

JS:   s.split("a").length - 1
来源：http://dcz.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://hde.sysykeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bcg.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://dnw.iojbl.cn

Ruby: s.count("a")
来源：http://ggc.xziqi.cn

C#:   s.Count(c => c == 'a')
来源：http://buz.jyoumei.cn

[E13] 逐字符遍历
来源：http://nln.kuanghao11.cn

Py:   for ch in s: print(ch)
来源：http://rqb.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ptj.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kpc.cqqwz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://guu.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rsq.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qml.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rby.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fpp.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://esc.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mdk.hongshengwenyu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dav.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mmd.aizwys.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bzz.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cwm.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://znt.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lry.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kmz.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://myf.zhengqikj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://riv.jqgfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ute.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://thn.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zst.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ezv.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjw.shuidangran.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gkx.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dsl.tianlin.xyz

[E16] 数字千分位
来源：http://pyl.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://sfn.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://zyr.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zfi.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yqn.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://asu.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cop.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xup.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://nir.sysykeji.top

[E17] 首字母大写
来源：http://jie.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oav.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hdh.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzk.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bfe.jyoumei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zah.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uyv.quarkkingdee.top

Ruby: s.capitalize
来源：http://ran.jyoumei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nsy.pycfn.com

[E18] 模板占位符替换
来源：http://num.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ekp.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xym.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jtm.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://iuj.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://axz.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rud.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bvm.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ejo.52xcode.cn

[E19] 多行文本按行拆分
来源：http://qze.redwolf501.top

Py:   s.splitlines()
来源：http://dyg.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://raf.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://cxb.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://aqd.ppjwa.cn

Java: s.lines().toList()
来源：http://euf.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://vfz.snrcjt.cn

Ruby: s.lines
来源：http://lzn.sxryk.cn

C#:   s.Split('\n')
来源：http://pxw.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://pfg.316326.xyz

Py:   if not s:
来源：http://doz.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pqp.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zkh.zdqjudy.top

TS:   if (s === "") {}
来源：http://atz.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://kml.xuetiantiany.cn

Go:   if s == "" {}
来源：http://zil.hammf.cn

Ruby: if s.empty?
来源：http://rds.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tde.bjfxy.top

[E21] 超长截断加省略号
来源：http://sis.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wzx.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ruk.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihh.smart0.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zuc.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://sgl.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lae.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rjg.yj20258.top


<!-- 参考信息 -->