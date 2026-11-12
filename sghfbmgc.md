代发 wailian999

C#:   list.Distinct().ToList()
来源：http://eay.chenlongwang.top

[D16] 求和与平均值
来源：http://gus.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yfa.zdqjudy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aza.fzhhl.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wcx.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://uke.ctjpmb.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dcl.jinqigufen.top

Go:   // 手写循环累加
来源：http://ive.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://usz.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://nxe.gzhubu.top

[D17] 最大值与最小值
来源：http://pnf.xuanzx.com

Py:   max(arr);  min(arr)
来源：http://vjm.vehdjk.com

PHP:  max($arr);  min($arr);
来源：http://aet.yj202588.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cmq.chenlongwang.top

TS:   Math.max(...arr);
来源：http://blw.yonumen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ymd.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xhi.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://xcv.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://yyu.yfazqb.com

[D18] 扁平化嵌套数组
来源：http://kqd.jianghu66.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tzk.birdmap.top

PHP:  array_merge(...$nested);
来源：http://spe.pengpengdd.cyou

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kam.hysaishi.cn

TS:   nested.flat();
来源：http://yei.sweek.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bie.yj202588.top

Go:   // 手写双层循环
来源：http://odu.sufxvd.cn

Ruby: nested.flatten
来源：http://thc.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ans.fengsongda.top

[D19] 按字段分组
来源：http://kfy.xziqi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fou.yfazqb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wdu.xingfuxueyuan.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zts.xuanzx.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://njb.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iih.shangyingyoupin.top

Go:   // 手写 map[string][]T
来源：http://phr.xuanzx.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mgq.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://aaj.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://oje.xziqi.cn

Py:   Counter(arr)
来源：http://tlp.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://mdx.ctjpmb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hqa.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sns.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kiz.tianlin.xyz

Go:   // 手写 map[T]int
来源：http://qdk.ctjpmb.com

Ruby: arr.tally
来源：http://iia.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gvs.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://gsx.shanyushiyangkeji.top

Py:   x in arr
来源：http://cyu.yvedp.cn

PHP:  in_array($x, $arr, true);
来源：http://kgf.tian-w.cn

JS:   arr.includes(x)
来源：http://gzj.sxryk.cn

TS:   arr.includes(x)
来源：http://uul.shangyingyoupin.top

Java: list.contains(x)
来源：http://xcr.gotoacloud.top

Go:   slices.Contains(arr, x)
来源：http://pyd.ydzc1.top

Ruby: arr.include?(x)
来源：http://qsa.yuxming.cn

C#:   list.Contains(x)
来源：http://orx.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://loe.c1oappe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nan.iojbl.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qqy.gogol.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mqd.fzhhl.top

TS:   [...arr];
来源：http://dek.c1oappe.top

Java: new ArrayList<>(list);
来源：http://zel.sweek.top

Go:   copied := append([]int(nil), arr...)
来源：http://vhn.jqgufenzy.top

Ruby: arr.dup;  arr.clone
来源：http://hdi.vehdjk.com

C#:   new List<int>(list);
来源：http://hbw.redwolf501.top

[D23] reduce 累积计算
来源：http://fgd.hnxiangtu.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rll.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ttn.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yye.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qhq.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ybc.fanxiaobao.xyz

Go:   // 手写循环
来源：http://apw.ctjpmb.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://owk.zhengqikj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gaq.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://fdj.ehwqpu.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ufz.yuxming.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qch.52xcode.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ruo.iojbl.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mnj.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xtj.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://atm.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zac.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ehf.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://ylk.yongpay.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cao.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dlk.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qyu.cdnleiting.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ghl.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jjw.yj20258888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sjz.sjlbkw.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ttp.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgc.uphjek.com

[D26] 数组转字符串
来源：http://efp.zdbjq.cn

Py:   ", ".join(map(str, arr))
来源：http://zwx.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://qxa.jiagoushi.top

JS:   arr.join(", ")
来源：http://fby.bbcook.cn

TS:   arr.join(", ")
来源：http://ygw.epnwcf.com

Java: String.join(", ", list)
来源：http://onr.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://gnt.fktsv.cn

Ruby: arr.join(", ")
来源：http://fwa.feifeiyinyue.top

C#:   string.Join(", ", list)
来源：http://zdi.ppjwa.cn

================================================================================
来源：http://xmc.ywan-chungtsiang.top

E. 字符串处理
来源：http://bvn.yueranfly.top

================================================================================
来源：http://tuo.hywenlv.cn

[E01] 拼接字符串
来源：http://wwv.redwolf501.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qqg.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pnj.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://toj.ydjk.org.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://soc.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gxn.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://biz.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kbf.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lkv.wangshuangyany.cn

[E02] 重复字符串
来源：http://imm.haohaochexian.top

Py:   "ab" * 3
来源：http://odm.mhx1999.top

PHP:  str_repeat("ab", 3);
来源：http://wmw.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://yqb.shanyushiyangkeji.top

TS:   "ab".repeat(3)
来源：http://aaz.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://vbl.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://uoz.chenzaomai.com

Ruby: "ab" * 3
来源：http://kkr.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xag.cucudq.cn

[E03] 截取子串
来源：http://lef.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qxp.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qnv.epnwcf.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ubd.0kj1m.cn

TS:   s.slice(1, 4)
来源：http://muo.9152youxi.cn

Java: s.substring(1, 4)
来源：http://axq.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fgj.sufxvd.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jdy.hnqzz.top

C#:   s.Substring(1, 3)
来源：http://hsx.gaohongyu789.top

[E04] 查找子串位置
来源：http://fvc.xziqi.cn

Py:   s.find("x");  s.index("x")
来源：http://ewv.xuanzx.com

PHP:  strpos($s, "x");
来源：http://dgg.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wfu.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://cwx.jyoumei.cn

Java: s.indexOf("x")
来源：http://mqa.zhengqikj.top

Go:   strings.Index(s, "x")
来源：http://onp.iojbl.cn

Ruby: s.index("x")
来源：http://fel.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://xwe.yfazqb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://ezr.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jxh.jinghuilouyu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mft.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://drx.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://eye.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nsj.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rqz.52xcode.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tgo.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vfq.jyoumei.cn

[E06] 替换子串
来源：http://xbo.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sfa.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://klo.fzhhl.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ies.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://zls.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aco.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hfo.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iqy.zdbjq.cn

C#:   s.Replace("a", "b")
来源：http://nqd.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://xvp.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jve.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qof.snrcjt.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tpb.jiagoushi.top

TS:   s.split(",")
来源：http://vhf.yueranfly.top

Java: s.split(",");  s.split("\\s+")
来源：http://suj.svipenyu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wid.jqgufenzy.top

Ruby: s.split(",");  s.split
来源：http://tcq.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yde.xylfe.cn

[E08] 数组按分隔符合并
来源：http://zcx.jianghu66.top

Py:   ",".join(items)
来源：http://rbe.xziqi.cn

PHP:  implode(",", $items);
来源：http://aic.xziqi.cn

JS:   items.join(",")
来源：http://gvr.hcnkem.com

TS:   items.join(",")
来源：http://zoq.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://iwc.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://myf.hcnkem.com

Ruby: items.join(",")
来源：http://ulm.xylfe.cn

C#:   string.Join(",", items)
来源：http://mtn.fzhhl.top

[E09] 去除所有空白字符
来源：http://fwq.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://usm.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rqd.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://fse.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://rka.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://lra.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ddk.ivvv.top

Ruby: s.gsub(/\s+/, "")
来源：http://mnj.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mej.wangdashe.top

[E10] 左侧补零 / 定长填充
来源：http://ptt.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pym.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pfi.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://ief.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://pbs.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://okg.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yqt.zdqjudy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kta.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pim.ehwqpu.com

[E11] 反转字符串
来源：http://smw.wangdashe.top

Py:   s[::-1]
来源：http://vlg.chenlongwang.top

PHP:  strrev($s);
来源：http://req.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://nqn.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://nja.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cvd.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pai.zdqjudy.top

Ruby: s.reverse
来源：http://jth.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://yij.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://wkj.xuetiantiany.cn

Py:   s.count("a")
来源：http://asz.jinqigufen.top

PHP:  substr_count($s, "a");
来源：http://jhw.yvedp.cn

JS:   s.split("a").length - 1
来源：http://doc.smart0.xyz

TS:   s.split("a").length - 1
来源：http://cpe.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qws.yj202588.top

Go:   strings.Count(s, "a")
来源：http://dfc.vqdsnc.cn

Ruby: s.count("a")
来源：http://rsb.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://raa.cashguo.top

[E13] 逐字符遍历
来源：http://lgg.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://itz.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jnh.uphjek.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://jtn.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ioq.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wfl.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zdw.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://nfa.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oxv.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://zzl.ydjk.org.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qqg.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dhm.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://elg.wangdashe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mhg.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vui.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fhu.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pqn.tian-w.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dfl.guannengcc.top

[E15] HTML 转义 / 反转义
来源：http://ykb.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jej.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cno.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gdx.meibo888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mdj.cucudq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cju.jinqigfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gdi.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rgs.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://coi.yanxiufei.cn

[E16] 数字千分位
来源：http://jwp.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://iji.smart0.xyz

PHP:  number_format(1234567);
来源：http://pml.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wmm.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vij.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sxi.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iys.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqk.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://kpo.jianghu66.top

[E17] 首字母大写
来源：http://gns.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rre.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aud.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xkw.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://euv.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nxz.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kfn.cucudq.cn

Ruby: s.capitalize
来源：http://uui.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rzr.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://wpo.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lmy.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mhj.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lcl.jianghu66.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hnt.yongpay.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://roj.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dob.cqqwz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfv.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vsn.meibo888.top

[E19] 多行文本按行拆分
来源：http://tqg.gotoacloud.top

Py:   s.splitlines()
来源：http://klh.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ypd.pengpengdd.cyou

JS:   s.split(/\r?\n/)
来源：http://era.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://rvq.jinyuanbaomall.cn

Java: s.lines().toList()
来源：http://njo.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://vkd.ppjwa.cn

Ruby: s.lines
来源：http://hum.jqgfzy.top

C#:   s.Split('\n')
来源：http://unc.yfazqb.com

[E20] 判断字符串是否为空
来源：http://ayr.hywenlv.cn

Py:   if not s:
来源：http://gcm.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rzb.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cyx.yj20258.top

TS:   if (s === "") {}
来源：http://wim.yuanzhike.top

Java: if (s.isEmpty()) {}
来源：http://ovt.dashuyun.cn

Go:   if s == "" {}
来源：http://bsg.birdmap.top

Ruby: if s.empty?
来源：http://mwn.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jwy.hammf.cn

[E21] 超长截断加省略号
来源：http://rxf.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nqy.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lda.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ffv.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cpg.ywan-chungtsiang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ebs.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://xey.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wgo.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zbl.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://wgk.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hmc.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dde.zhoulong.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://twb.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://thp.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ojp.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wjm.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://snl.yvedp.cn


<!-- 参考信息 -->