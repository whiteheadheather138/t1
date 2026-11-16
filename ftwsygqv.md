代发 wailian999

[D15] 去重
来源：http://gpm.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vql.ppjwa.cn

PHP:  array_unique($arr);
来源：http://zmo.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://dpr.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://epg.fanxiaobao.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hkz.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://two.ctjpmb.com

Ruby: arr.uniq
来源：http://fap.yj20258.top

C#:   list.Distinct().ToList()
来源：http://mjy.sjlbkw.cn

[D16] 求和与平均值
来源：http://eec.xinyue.icu

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://twd.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pnn.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfj.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oqj.tanke756.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://seb.yueranfly.top

Go:   // 手写循环累加
来源：http://rcw.316326.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jjt.yj202588.top

C#:   list.Sum();  list.Average()
来源：http://tes.zdbjq.cn

[D17] 最大值与最小值
来源：http://pdv.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://vfd.xylfe.cn

PHP:  max($arr);  min($arr);
来源：http://wzy.gzhubu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzy.xylfe.cn

TS:   Math.max(...arr);
来源：http://xit.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nhr.xingfuxueyuan.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ymu.ybcxt.top

Ruby: arr.max;  arr.min
来源：http://lgf.cashguo.top

C#:   list.Max();  list.Min()
来源：http://lrm.smart0.xyz

[D18] 扁平化嵌套数组
来源：http://hxa.chenzaomai.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cra.yj20258888.top

PHP:  array_merge(...$nested);
来源：http://wbz.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://stg.shangyingyoupin.top

TS:   nested.flat();
来源：http://hek.c1oappe.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://llx.hcnkem.com

Go:   // 手写双层循环
来源：http://aze.daxiang520.top

Ruby: nested.flatten
来源：http://djz.jqgfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gap.pengpengdd.cyou

[D19] 按字段分组
来源：http://dag.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mbh.fengsongda.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://igb.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://anu.yonumen.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hms.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bop.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://qmv.hcnkem.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mud.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iir.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://eaw.zdbjq.cn

Py:   Counter(arr)
来源：http://bpv.daxiang520.top

PHP:  array_count_values($arr);
来源：http://wyp.ybcxt.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bwr.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zsx.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://awg.wangshuangyany.cn

Go:   // 手写 map[T]int
来源：http://dxm.tianlin.xyz

Ruby: arr.tally
来源：http://ipu.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xpu.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://lhx.sweek.top

Py:   x in arr
来源：http://ren.ehwqpu.com

PHP:  in_array($x, $arr, true);
来源：http://gxh.c1oappe.top

JS:   arr.includes(x)
来源：http://aze.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://svy.shuidangran.top

Java: list.contains(x)
来源：http://jks.hysaishi.cn

Go:   slices.Contains(arr, x)
来源：http://vxw.svipenyu.cn

Ruby: arr.include?(x)
来源：http://vbc.daxiang520.top

C#:   list.Contains(x)
来源：http://rgv.hammf.cn

[D22] 复制数组（避免共享引用）
来源：http://ftt.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mtq.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cnj.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tls.jianghu66.top

TS:   [...arr];
来源：http://xqr.chenlongwang.top

Java: new ArrayList<>(list);
来源：http://zeb.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://sly.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://srd.9152youxi.cn

C#:   new List<int>(list);
来源：http://vba.iojbl.cn

[D23] reduce 累积计算
来源：http://gqy.jianghu66.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zrl.zdqjudy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wpz.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abt.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dsf.chenjidiqi.icu

Java: list.stream().reduce(0, Integer::sum)
来源：http://ioe.hfpthk.cn

Go:   // 手写循环
来源：http://xse.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oue.havefunace.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cnk.meibo888.top

[D24] 字典 / Map 基本操作
来源：http://jan.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ckt.fanxiaobao.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bbk.cqqwz.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gtt.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wwi.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vhr.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yjo.pengpengdd.cyou

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fxq.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dvh.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://tsi.bbcook.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rrh.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://krd.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ojb.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xuf.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bzf.bjfxy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yhh.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yqx.uphjek.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jwc.chenzaomai.com

[D26] 数组转字符串
来源：http://lrj.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://nal.zhijiandao.cn

PHP:  implode(", ", $arr);
来源：http://vrx.zhiwuduotai.top

JS:   arr.join(", ")
来源：http://rad.andypj.xyz

TS:   arr.join(", ")
来源：http://tli.sufxvd.cn

Java: String.join(", ", list)
来源：http://anr.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://dqb.bjfxy.top

Ruby: arr.join(", ")
来源：http://uov.c1oappe.top

C#:   string.Join(", ", list)
来源：http://egq.zycfv.cn

================================================================================
来源：http://sik.bbcook.cn

E. 字符串处理
来源：http://cii.wangdashe.top

================================================================================
来源：http://saq.haohaochexian.top

[E01] 拼接字符串
来源：http://osq.daxiang520.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zyt.jqgfzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bnl.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qlg.chenlongwang.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lyq.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kob.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pld.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ccg.xziqi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wds.meibo888.top

[E02] 重复字符串
来源：http://ham.yj202588.top

Py:   "ab" * 3
来源：http://rox.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://jwf.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://fmt.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://efr.jyoumei.cn

Java: "ab".repeat(3)
来源：http://mqh.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://yil.ctjpmb.com

Ruby: "ab" * 3
来源：http://mjm.ywan-chungtsiang.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lad.haohaochexian.top

[E03] 截取子串
来源：http://ixs.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://egf.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xxe.hywenlv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hsz.ybcxt.top

TS:   s.slice(1, 4)
来源：http://eys.zdqjudy.top

Java: s.substring(1, 4)
来源：http://axw.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ewd.quarkkingdee.top

Ruby: s[1, 3];  s[1..3]
来源：http://ibi.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://qcu.yj20258888.top

[E04] 查找子串位置
来源：http://ipe.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://ghb.bbcook.cn

PHP:  strpos($s, "x");
来源：http://vbb.yvedp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fqr.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://yqz.jlsjyb.cn

Java: s.indexOf("x")
来源：http://vwk.sweek.top

Go:   strings.Index(s, "x")
来源：http://gjs.ydzc1.top

Ruby: s.index("x")
来源：http://zas.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://dih.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vwz.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oxp.yj202588.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hec.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wwg.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://czu.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ggp.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pou.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yni.cashguo.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dxa.hysaishi.cn

[E06] 替换子串
来源：http://jnq.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ydx.zdbjq.cn

PHP:  str_replace("a", "b", $s);
来源：http://wpo.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mul.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://aqi.feifeiyinyue.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wvk.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://anc.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qin.shzxlz.cn

C#:   s.Replace("a", "b")
来源：http://jtl.zycfv.cn

[E07] 按分隔符拆分
来源：http://twk.yangfankeji.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nky.sweek.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://smg.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bdi.fengsongda.top

TS:   s.split(",")
来源：http://fhh.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bhi.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fey.daxiang520.top

Ruby: s.split(",");  s.split
来源：http://rgt.nanxuanxn.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xsi.jqgfzy.top

[E08] 数组按分隔符合并
来源：http://uxc.hfpthk.cn

Py:   ",".join(items)
来源：http://loq.fzhhl.top

PHP:  implode(",", $items);
来源：http://ktz.jiagoushi.top

JS:   items.join(",")
来源：http://zwc.wangshuangyany.cn

TS:   items.join(",")
来源：http://kdw.hfpthk.cn

Java: String.join(",", items)
来源：http://fhs.ywan-chungtsiang.top

Go:   strings.Join(items, ",")
来源：http://rzz.ydjk.org.cn

Ruby: items.join(",")
来源：http://vej.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://idk.jyoumei.cn

[E09] 去除所有空白字符
来源：http://byz.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cju.nanxuanxn.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sfu.quarkkingdee.top

JS:   s.replace(/\s+/g, "")
来源：http://xax.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://wkl.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://btd.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ndq.yj20258.top

Ruby: s.gsub(/\s+/, "")
来源：http://nhk.ivvv.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hpr.jinyuanbaomall.cn

[E10] 左侧补零 / 定长填充
来源：http://kdq.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pcm.jiagoushi.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fpj.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://rxt.xziqi.cn

TS:   "7".padStart(3, "0")
来源：http://jlg.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://bgc.xziqi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ugs.nanxinkj.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xsf.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kdh.zhengqikj.top

[E11] 反转字符串
来源：http://trh.ehwqpu.com

Py:   s[::-1]
来源：http://vwb.zhiwuduotai.top

PHP:  strrev($s);
来源：http://vxo.haohaochexian.top

JS:   [...s].reverse().join("")
来源：http://gja.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://yxh.vqdsnc.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://scg.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yko.haohaochexian.top

Ruby: s.reverse
来源：http://onm.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://vty.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://wmj.xuanzx.com

Py:   s.count("a")
来源：http://sdu.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://vbv.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://hxz.yvedp.cn

TS:   s.split("a").length - 1
来源：http://bog.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gst.shanyushiyangkeji.top

Go:   strings.Count(s, "a")
来源：http://dqj.xinyue.icu

Ruby: s.count("a")
来源：http://ofj.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://flq.mhx1999.top

[E13] 逐字符遍历
来源：http://ozm.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://oqc.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yec.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://eap.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pid.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zol.c1oappe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rmm.ybcxt.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fyx.feifeiyinyue.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://szp.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://exg.yanxiufei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vuc.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mxi.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tki.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xio.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fmn.jlsjyb.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cnz.quarkkingdee.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://okr.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hmo.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://non.jinqigfzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://meq.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ozl.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fjm.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qab.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pjk.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dxk.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jyb.hnxiangtu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://csn.chenjidiqi.icu

[E16] 数字千分位
来源：http://ovx.yueranfly.top

Py:   f"{1234567:,}"
来源：http://dqm.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://ipq.shanyushiyangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fyc.shangyingyoupin.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qsm.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://asl.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cqa.nanxinkj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ygz.fehbvm.com

C#:   1234567.ToString("N0")
来源：http://nut.jlsjyb.cn

[E17] 首字母大写
来源：http://msw.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vwp.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hsr.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cmf.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evf.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wwu.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lra.zhongyouzk.top

Ruby: s.capitalize
来源：http://vyk.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qeb.fehbvm.com

[E18] 模板占位符替换
来源：http://iml.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://osh.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vmp.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xvx.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rec.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dhp.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://noe.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gkx.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oxw.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://qcx.hesvh.cn

Py:   s.splitlines()
来源：http://hzs.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tqa.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://vbg.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://ifq.chenlongwang.top

Java: s.lines().toList()
来源：http://qke.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://bme.fktsv.cn

Ruby: s.lines
来源：http://lnh.vqdsnc.cn

C#:   s.Split('\n')
来源：http://tpc.ybcxt.top

[E20] 判断字符串是否为空
来源：http://csn.yvedp.cn

Py:   if not s:
来源：http://hcl.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ump.quarkkingdee.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://may.nwbrower.top

TS:   if (s === "") {}
来源：http://hzq.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://xri.uphjek.com

Go:   if s == "" {}
来源：http://etq.jqgufenzy.top

Ruby: if s.empty?
来源：http://awq.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gks.yonumen.top

[E21] 超长截断加省略号
来源：http://nvi.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kty.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://adl.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sij.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://amh.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cah.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://uhj.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sgx.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ggc.ydjk.org.cn


<!-- 参考信息 -->